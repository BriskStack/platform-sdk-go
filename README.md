# BriskStack Platform SDK (Go)

Official Go SDK for the BriskStack Platform. Access all BriskStack services through a single unified SDK.

[![Go Reference](https://pkg.go.dev/badge/github.com/briskstack/platform-sdk-go.svg)](https://pkg.go.dev/github.com/briskstack/platform-sdk-go)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Go Version](https://img.shields.io/github/go-mod/go-version/briskstack/platform-sdk-go)](https://golang.org/dl/)

## Installation

```bash
go get github.com/briskstack/platform-sdk-go@latest
```

Or for a specific version:
```bash
go get github.com/briskstack/platform-sdk-go@v1.2.3
```

## Quick Start

```go
package main

import (
    "context"
    "fmt"
    briskstack "github.com/briskstack/platform-sdk-go"
)

func main() {
    // Configure once for all services
    config := briskstack.NewConfiguration()
    config.Host = "api.briskstack.com"
    config.Scheme = "https"
    config.AddDefaultHeader("Authorization", "Bearer your-jwt-token")

    client := briskstack.NewAPIClient(config)
    ctx := context.Background()

    // Use different services
    msgReq := briskstack.HelloWorldCreateMessageRequest{
        Content: "Hello!",
    }
    message, _, err := client.HelloWorldMessagesAPI.HelloWorldV1MessagesPost(ctx).
        HelloWorldCreateMessageRequest(msgReq).
        Execute()

    if err != nil {
        panic(err)
    }

    fmt.Println(message.GetContent())

    chatReq := briskstack.AiGatewayChatCompletionRequest{
        Model: "gpt-4",
        Messages: []briskstack.AiGatewayChatMessage{
            {Role: "user", Content: "Hello AI"},
        },
    }
    completion, _, err := client.AiGatewayChatAPI.AiGatewayV1ChatCompletionsPost(ctx).
        AiGatewayChatCompletionRequest(chatReq).
        Execute()

    if err != nil {
        panic(err)
    }

    fmt.Println(completion.Choices[0].Message.GetContent())
}
```

## Features

- 🚀 **Unified SDK** - Access all BriskStack services through a single module
- 🔐 **Multiple Auth Methods** - Support for JWT tokens and API keys
- 🌐 **Environment URLs** - Easy configuration for dev, staging, and production
- 📝 **Type Safety** - Full Go type definitions for all APIs
- 🔄 **Auto-generated** - Always up-to-date with the latest API changes
- 🎯 **Go 1.21+** - Modern Go support with generics

## Authentication

### Bearer Token (JWT)

For user authentication via Supabase:

```go
config := briskstack.NewConfiguration()
config.Host = "api.briskstack.com"
config.Scheme = "https"
config.AddDefaultHeader("Authorization", "Bearer your-jwt-token")

client := briskstack.NewAPIClient(config)
```

### API Key

For BYOK (Bring Your Own Key) scenarios:

```go
config := briskstack.NewConfiguration()
config.Host = "api.briskstack.com"
config.Scheme = "https"
config.AddDefaultHeader("X-API-Key", "your-api-key")

client := briskstack.NewAPIClient(config)
```

## Environment URLs

The SDK supports multiple environments:

```go
// Development
config := briskstack.NewConfiguration()
config.Host = "api-dev.briskstack.com"
config.Scheme = "https"

// Staging
config := briskstack.NewConfiguration()
config.Host = "api-staging.briskstack.com"
config.Scheme = "https"

// Production
config := briskstack.NewConfiguration()
config.Host = "api.briskstack.com"
config.Scheme = "https"
```

## Available Services

This SDK includes all BriskStack platform services:

- **Hello World** - Example service
- **AI Gateway** - AI model integrations
- *(More services added automatically)*

See the [API documentation](https://docs.briskstack.com) for complete service details.

## Usage Examples

### Hello World Service

```go
package main

import (
    "context"
    "fmt"
    briskstack "github.com/briskstack/platform-sdk-go"
)

func main() {
    config := briskstack.NewConfiguration()
    config.Host = "api.briskstack.com"
    config.Scheme = "https"
    config.AddDefaultHeader("Authorization", "Bearer your-jwt-token")

    client := briskstack.NewAPIClient(config)
    ctx := context.Background()

    // Create a message
    req := briskstack.HelloWorldCreateMessageRequest{
        Content: "Hello, World!",
    }

    message, resp, err := client.HelloWorldMessagesAPI.
        HelloWorldV1MessagesPost(ctx).
        HelloWorldCreateMessageRequest(req).
        Execute()

    if err != nil {
        fmt.Printf("Error: %v\n", err)
        return
    }
    defer resp.Body.Close()

    fmt.Printf("Message ID: %s\n", message.GetId())
    fmt.Printf("Content: %s\n", message.GetContent())
}
```

### AI Gateway Service

```go
package main

import (
    "context"
    "fmt"
    briskstack "github.com/briskstack/platform-sdk-go"
)

func main() {
    config := briskstack.NewConfiguration()
    config.Host = "api.briskstack.com"
    config.Scheme = "https"
    config.AddDefaultHeader("X-API-Key", "your-api-key") // Use API key for BYOK

    client := briskstack.NewAPIClient(config)
    ctx := context.Background()

    // Create a chat completion
    req := briskstack.AiGatewayChatCompletionRequest{
        Model: "gpt-4",
        Messages: []briskstack.AiGatewayChatMessage{
            {Role: "system", Content: "You are a helpful assistant."},
            {Role: "user", Content: "Tell me a joke about programming."},
        },
    }

    completion, resp, err := client.AiGatewayChatAPI.
        AiGatewayV1ChatCompletionsPost(ctx).
        AiGatewayChatCompletionRequest(req).
        Execute()

    if err != nil {
        fmt.Printf("Error: %v\n", err)
        return
    }
    defer resp.Body.Close()

    fmt.Println(completion.Choices[0].Message.GetContent())
}
```

## Error Handling

```go
message, resp, err := client.HelloWorldMessagesAPI.
    HelloWorldV1MessagesPost(ctx).
    HelloWorldCreateMessageRequest(req).
    Execute()

if err != nil {
    // Type assert to get detailed error information
    if apiErr, ok := err.(*briskstack.GenericOpenAPIError); ok {
        fmt.Printf("API Error: %s\n", apiErr.Error())
        fmt.Printf("Response Body: %s\n", apiErr.Body())
    } else {
        fmt.Printf("Error: %v\n", err)
    }
    return
}
defer resp.Body.Close()

// Check HTTP status code
if resp.StatusCode != 200 {
    fmt.Printf("Unexpected status code: %d\n", resp.StatusCode)
}
```

## Context and Cancellation

The SDK supports Go contexts for cancellation and timeouts:

```go
import (
    "context"
    "time"
)

// With timeout
ctx, cancel := context.WithTimeout(context.Background(), 5*time.Second)
defer cancel()

message, _, err := client.HelloWorldMessagesAPI.
    HelloWorldV1MessagesPost(ctx).
    HelloWorldCreateMessageRequest(req).
    Execute()

// With cancellation
ctx, cancel := context.WithCancel(context.Background())
go func() {
    // Cancel after some condition
    cancel()
}()

message, _, err := client.HelloWorldMessagesAPI.
    HelloWorldV1MessagesPost(ctx).
    HelloWorldCreateMessageRequest(req).
    Execute()
```

## Custom HTTP Client

You can provide a custom HTTP client:

```go
import (
    "net/http"
    "time"
)

config := briskstack.NewConfiguration()
config.HTTPClient = &http.Client{
    Timeout: 30 * time.Second,
    Transport: &http.Transport{
        MaxIdleConns:        100,
        MaxIdleConnsPerHost: 100,
    },
}

client := briskstack.NewAPIClient(config)
```

## Framework Integration

### HTTP Handler

```go
package main

import (
    "encoding/json"
    "net/http"
    briskstack "github.com/briskstack/platform-sdk-go"
)

func helloHandler(w http.ResponseWriter, r *http.Request) {
    config := briskstack.NewConfiguration()
    config.Host = "api.briskstack.com"
    config.Scheme = "https"

    // Get token from request header
    token := r.Header.Get("Authorization")
    config.AddDefaultHeader("Authorization", token)

    client := briskstack.NewAPIClient(config)

    var req briskstack.HelloWorldCreateMessageRequest
    if err := json.NewDecoder(r.Body).Decode(&req); err != nil {
        http.Error(w, err.Error(), http.StatusBadRequest)
        return
    }

    message, _, err := client.HelloWorldMessagesAPI.
        HelloWorldV1MessagesPost(r.Context()).
        HelloWorldCreateMessageRequest(req).
        Execute()

    if err != nil {
        http.Error(w, err.Error(), http.StatusInternalServerError)
        return
    }

    json.NewEncoder(w).Encode(message)
}

func main() {
    http.HandleFunc("/api/hello", helloHandler)
    http.ListenAndServe(":8080", nil)
}
```

### Gin Framework

```go
package main

import (
    "github.com/gin-gonic/gin"
    briskstack "github.com/briskstack/platform-sdk-go"
)

func main() {
    r := gin.Default()

    r.POST("/api/hello", func(c *gin.Context) {
        config := briskstack.NewConfiguration()
        config.Host = "api.briskstack.com"
        config.Scheme = "https"
        config.AddDefaultHeader("Authorization", c.GetHeader("Authorization"))

        client := briskstack.NewAPIClient(config)

        var req briskstack.HelloWorldCreateMessageRequest
        if err := c.BindJSON(&req); err != nil {
            c.JSON(400, gin.H{"error": err.Error()})
            return
        }

        message, _, err := client.HelloWorldMessagesAPI.
            HelloWorldV1MessagesPost(c.Request.Context()).
            HelloWorldCreateMessageRequest(req).
            Execute()

        if err != nil {
            c.JSON(500, gin.H{"error": err.Error()})
            return
        }

        c.JSON(200, message)
    })

    r.Run(":8080")
}
```

## Environment Variables

Best practice is to use environment variables for configuration:

```go
import "os"

config := briskstack.NewConfiguration()
config.Host = getEnv("BRISKSTACK_API_HOST", "api.briskstack.com")
config.Scheme = "https"
config.AddDefaultHeader("Authorization", "Bearer "+os.Getenv("BRISKSTACK_ACCESS_TOKEN"))

func getEnv(key, fallback string) string {
    if value := os.Getenv(key); value != "" {
        return value
    }
    return fallback
}
```

## Testing

The SDK is designed to be easily testable:

```go
package main

import (
    "testing"
    briskstack "github.com/briskstack/platform-sdk-go"
)

func TestHelloWorld(t *testing.T) {
    config := briskstack.NewConfiguration()
    config.Host = "api-dev.briskstack.com" // Use dev environment for testing
    config.Scheme = "https"
    config.AddDefaultHeader("Authorization", "Bearer test-token")

    client := briskstack.NewAPIClient(config)

    // Your test code here
}
```

## Requirements

- Go 1.21 or higher
- Dependencies managed via go.mod

## Contributing

This SDK is automatically generated from OpenAPI specifications. To contribute:

1. Make changes to the platform services in [briskstack-platform](https://github.com/briskstack/briskstack-platform)
2. The SDK will be automatically regenerated and published

## Documentation

- [API Documentation](https://docs.briskstack.com)
- [pkg.go.dev](https://pkg.go.dev/github.com/briskstack/platform-sdk-go)
- [Platform Repository](https://github.com/briskstack/briskstack-platform)
- [SDK Generation Guide](https://github.com/briskstack/briskstack-platform/tree/main/sdks)

## License

MIT

## Support

- GitHub Issues: [briskstack/platform-sdk-go/issues](https://github.com/briskstack/platform-sdk-go/issues)
- Email: support@briskstack.com
- Documentation: [docs.briskstack.com](https://docs.briskstack.com)

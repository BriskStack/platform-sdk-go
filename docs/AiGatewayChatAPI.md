# \AiGatewayChatAPI

All URIs are relative to *https://api.briskstack.com/ai-gateway/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AiGatewayV1ChatCompletionsPost**](AiGatewayChatAPI.md#AiGatewayV1ChatCompletionsPost) | **Post** /ai-gateway/v1/chat/completions | Create chat completion



## AiGatewayV1ChatCompletionsPost

> AiGatewayChatCompletionResponse AiGatewayV1ChatCompletionsPost(ctx).AiGatewayChatCompletionRequest(aiGatewayChatCompletionRequest).Execute()

Create chat completion



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/briskstack"
)

func main() {
	aiGatewayChatCompletionRequest := *openapiclient.NewAiGatewayChatCompletionRequest("openai/gpt-4", []openapiclient.AiGatewayChatMessage{*openapiclient.NewAiGatewayChatMessage("Role_example")}) // AiGatewayChatCompletionRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AiGatewayChatAPI.AiGatewayV1ChatCompletionsPost(context.Background()).AiGatewayChatCompletionRequest(aiGatewayChatCompletionRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AiGatewayChatAPI.AiGatewayV1ChatCompletionsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AiGatewayV1ChatCompletionsPost`: AiGatewayChatCompletionResponse
	fmt.Fprintf(os.Stdout, "Response from `AiGatewayChatAPI.AiGatewayV1ChatCompletionsPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAiGatewayV1ChatCompletionsPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **aiGatewayChatCompletionRequest** | [**AiGatewayChatCompletionRequest**](AiGatewayChatCompletionRequest.md) |  | 

### Return type

[**AiGatewayChatCompletionResponse**](AiGatewayChatCompletionResponse.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


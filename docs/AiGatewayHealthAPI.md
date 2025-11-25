# \AiGatewayHealthAPI

All URIs are relative to *https://api.briskstack.com/ai-gateway/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AiGatewayV1HealthzGet**](AiGatewayHealthAPI.md#AiGatewayV1HealthzGet) | **Get** /ai-gateway/v1/healthz | Health check endpoint



## AiGatewayV1HealthzGet

> AiGatewayHealthzResponse AiGatewayV1HealthzGet(ctx).Execute()

Health check endpoint



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AiGatewayHealthAPI.AiGatewayV1HealthzGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AiGatewayHealthAPI.AiGatewayV1HealthzGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AiGatewayV1HealthzGet`: AiGatewayHealthzResponse
	fmt.Fprintf(os.Stdout, "Response from `AiGatewayHealthAPI.AiGatewayV1HealthzGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAiGatewayV1HealthzGetRequest struct via the builder pattern


### Return type

[**AiGatewayHealthzResponse**](AiGatewayHealthzResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


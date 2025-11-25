# \HelloWorldHealthAPI

All URIs are relative to *https://api.briskstack.com/ai-gateway/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**HelloWorldV1HealthzGet**](HelloWorldHealthAPI.md#HelloWorldV1HealthzGet) | **Get** /hello-world/v1/healthz | Health check endpoint



## HelloWorldV1HealthzGet

> HelloWorldHealthzResponse HelloWorldV1HealthzGet(ctx).Execute()

Health check endpoint



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/briskstack/platform-sdk-go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.HelloWorldHealthAPI.HelloWorldV1HealthzGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `HelloWorldHealthAPI.HelloWorldV1HealthzGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `HelloWorldV1HealthzGet`: HelloWorldHealthzResponse
	fmt.Fprintf(os.Stdout, "Response from `HelloWorldHealthAPI.HelloWorldV1HealthzGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiHelloWorldV1HealthzGetRequest struct via the builder pattern


### Return type

[**HelloWorldHealthzResponse**](HelloWorldHealthzResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


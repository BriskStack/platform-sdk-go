# \HelloWorldCoreAPI

All URIs are relative to *https://api.briskstack.com/ai-gateway/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**HelloWorldV1Get**](HelloWorldCoreAPI.md#HelloWorldV1Get) | **Get** /hello-world/v1/ | Hello endpoint



## HelloWorldV1Get

> HelloWorldHelloResponse HelloWorldV1Get(ctx).Execute()

Hello endpoint



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
	resp, r, err := apiClient.HelloWorldCoreAPI.HelloWorldV1Get(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `HelloWorldCoreAPI.HelloWorldV1Get``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `HelloWorldV1Get`: HelloWorldHelloResponse
	fmt.Fprintf(os.Stdout, "Response from `HelloWorldCoreAPI.HelloWorldV1Get`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiHelloWorldV1GetRequest struct via the builder pattern


### Return type

[**HelloWorldHelloResponse**](HelloWorldHelloResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


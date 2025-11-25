# \HelloWorldAuthAPI

All URIs are relative to *https://api.briskstack.com/ai-gateway/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**HelloWorldV1ProtectedGet**](HelloWorldAuthAPI.md#HelloWorldV1ProtectedGet) | **Get** /hello-world/v1/protected | Protected endpoint (requires authentication)



## HelloWorldV1ProtectedGet

> HelloWorldProtectedResponse HelloWorldV1ProtectedGet(ctx).Execute()

Protected endpoint (requires authentication)



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
	resp, r, err := apiClient.HelloWorldAuthAPI.HelloWorldV1ProtectedGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `HelloWorldAuthAPI.HelloWorldV1ProtectedGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `HelloWorldV1ProtectedGet`: HelloWorldProtectedResponse
	fmt.Fprintf(os.Stdout, "Response from `HelloWorldAuthAPI.HelloWorldV1ProtectedGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiHelloWorldV1ProtectedGetRequest struct via the builder pattern


### Return type

[**HelloWorldProtectedResponse**](HelloWorldProtectedResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


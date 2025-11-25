# \HelloWorldMessagesAPI

All URIs are relative to *https://api.briskstack.com/ai-gateway/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**HelloWorldV1MessagesPost**](HelloWorldMessagesAPI.md#HelloWorldV1MessagesPost) | **Post** /hello-world/v1/messages | Create message



## HelloWorldV1MessagesPost

> HelloWorldCreateMessageResponse HelloWorldV1MessagesPost(ctx).HelloWorldCreateMessageRequest(helloWorldCreateMessageRequest).Execute()

Create message



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
	helloWorldCreateMessageRequest := *openapiclient.NewHelloWorldCreateMessageRequest("Hello World") // HelloWorldCreateMessageRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.HelloWorldMessagesAPI.HelloWorldV1MessagesPost(context.Background()).HelloWorldCreateMessageRequest(helloWorldCreateMessageRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `HelloWorldMessagesAPI.HelloWorldV1MessagesPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `HelloWorldV1MessagesPost`: HelloWorldCreateMessageResponse
	fmt.Fprintf(os.Stdout, "Response from `HelloWorldMessagesAPI.HelloWorldV1MessagesPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiHelloWorldV1MessagesPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **helloWorldCreateMessageRequest** | [**HelloWorldCreateMessageRequest**](HelloWorldCreateMessageRequest.md) |  | 

### Return type

[**HelloWorldCreateMessageResponse**](HelloWorldCreateMessageResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


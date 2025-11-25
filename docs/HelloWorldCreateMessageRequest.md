# HelloWorldCreateMessageRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Message** | **string** | Message content (1-500 characters) | 
**Priority** | Pointer to **string** | Message priority level | [optional] 

## Methods

### NewHelloWorldCreateMessageRequest

`func NewHelloWorldCreateMessageRequest(message string, ) *HelloWorldCreateMessageRequest`

NewHelloWorldCreateMessageRequest instantiates a new HelloWorldCreateMessageRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewHelloWorldCreateMessageRequestWithDefaults

`func NewHelloWorldCreateMessageRequestWithDefaults() *HelloWorldCreateMessageRequest`

NewHelloWorldCreateMessageRequestWithDefaults instantiates a new HelloWorldCreateMessageRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMessage

`func (o *HelloWorldCreateMessageRequest) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *HelloWorldCreateMessageRequest) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *HelloWorldCreateMessageRequest) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetPriority

`func (o *HelloWorldCreateMessageRequest) GetPriority() string`

GetPriority returns the Priority field if non-nil, zero value otherwise.

### GetPriorityOk

`func (o *HelloWorldCreateMessageRequest) GetPriorityOk() (*string, bool)`

GetPriorityOk returns a tuple with the Priority field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriority

`func (o *HelloWorldCreateMessageRequest) SetPriority(v string)`

SetPriority sets Priority field to given value.

### HasPriority

`func (o *HelloWorldCreateMessageRequest) HasPriority() bool`

HasPriority returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



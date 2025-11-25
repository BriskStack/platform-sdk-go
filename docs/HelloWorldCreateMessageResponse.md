# HelloWorldCreateMessageResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Message ID | 
**Message** | **string** | Message content | 
**Priority** | **string** | Message priority | 
**CreatedAt** | **time.Time** | Creation timestamp | 

## Methods

### NewHelloWorldCreateMessageResponse

`func NewHelloWorldCreateMessageResponse(id string, message string, priority string, createdAt time.Time, ) *HelloWorldCreateMessageResponse`

NewHelloWorldCreateMessageResponse instantiates a new HelloWorldCreateMessageResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewHelloWorldCreateMessageResponseWithDefaults

`func NewHelloWorldCreateMessageResponseWithDefaults() *HelloWorldCreateMessageResponse`

NewHelloWorldCreateMessageResponseWithDefaults instantiates a new HelloWorldCreateMessageResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *HelloWorldCreateMessageResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *HelloWorldCreateMessageResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *HelloWorldCreateMessageResponse) SetId(v string)`

SetId sets Id field to given value.


### GetMessage

`func (o *HelloWorldCreateMessageResponse) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *HelloWorldCreateMessageResponse) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *HelloWorldCreateMessageResponse) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetPriority

`func (o *HelloWorldCreateMessageResponse) GetPriority() string`

GetPriority returns the Priority field if non-nil, zero value otherwise.

### GetPriorityOk

`func (o *HelloWorldCreateMessageResponse) GetPriorityOk() (*string, bool)`

GetPriorityOk returns a tuple with the Priority field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriority

`func (o *HelloWorldCreateMessageResponse) SetPriority(v string)`

SetPriority sets Priority field to given value.


### GetCreatedAt

`func (o *HelloWorldCreateMessageResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *HelloWorldCreateMessageResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *HelloWorldCreateMessageResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



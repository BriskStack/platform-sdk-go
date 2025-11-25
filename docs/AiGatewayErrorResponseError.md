# AiGatewayErrorResponseError

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Code** | **string** | Error code | 
**Message** | **string** | Error message | 
**Details** | Pointer to **map[string]interface{}** | Additional error details | [optional] 

## Methods

### NewAiGatewayErrorResponseError

`func NewAiGatewayErrorResponseError(code string, message string, ) *AiGatewayErrorResponseError`

NewAiGatewayErrorResponseError instantiates a new AiGatewayErrorResponseError object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAiGatewayErrorResponseErrorWithDefaults

`func NewAiGatewayErrorResponseErrorWithDefaults() *AiGatewayErrorResponseError`

NewAiGatewayErrorResponseErrorWithDefaults instantiates a new AiGatewayErrorResponseError object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCode

`func (o *AiGatewayErrorResponseError) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *AiGatewayErrorResponseError) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *AiGatewayErrorResponseError) SetCode(v string)`

SetCode sets Code field to given value.


### GetMessage

`func (o *AiGatewayErrorResponseError) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *AiGatewayErrorResponseError) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *AiGatewayErrorResponseError) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetDetails

`func (o *AiGatewayErrorResponseError) GetDetails() map[string]interface{}`

GetDetails returns the Details field if non-nil, zero value otherwise.

### GetDetailsOk

`func (o *AiGatewayErrorResponseError) GetDetailsOk() (*map[string]interface{}, bool)`

GetDetailsOk returns a tuple with the Details field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDetails

`func (o *AiGatewayErrorResponseError) SetDetails(v map[string]interface{})`

SetDetails sets Details field to given value.

### HasDetails

`func (o *AiGatewayErrorResponseError) HasDetails() bool`

HasDetails returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



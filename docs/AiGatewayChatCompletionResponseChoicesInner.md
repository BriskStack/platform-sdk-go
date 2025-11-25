# AiGatewayChatCompletionResponseChoicesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Index** | **int32** |  | 
**Message** | [**AiGatewayChatMessage**](AiGatewayChatMessage.md) |  | 
**FinishReason** | **string** |  | 
**Logprobs** | Pointer to **interface{}** |  | [optional] 

## Methods

### NewAiGatewayChatCompletionResponseChoicesInner

`func NewAiGatewayChatCompletionResponseChoicesInner(index int32, message AiGatewayChatMessage, finishReason string, ) *AiGatewayChatCompletionResponseChoicesInner`

NewAiGatewayChatCompletionResponseChoicesInner instantiates a new AiGatewayChatCompletionResponseChoicesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAiGatewayChatCompletionResponseChoicesInnerWithDefaults

`func NewAiGatewayChatCompletionResponseChoicesInnerWithDefaults() *AiGatewayChatCompletionResponseChoicesInner`

NewAiGatewayChatCompletionResponseChoicesInnerWithDefaults instantiates a new AiGatewayChatCompletionResponseChoicesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIndex

`func (o *AiGatewayChatCompletionResponseChoicesInner) GetIndex() int32`

GetIndex returns the Index field if non-nil, zero value otherwise.

### GetIndexOk

`func (o *AiGatewayChatCompletionResponseChoicesInner) GetIndexOk() (*int32, bool)`

GetIndexOk returns a tuple with the Index field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIndex

`func (o *AiGatewayChatCompletionResponseChoicesInner) SetIndex(v int32)`

SetIndex sets Index field to given value.


### GetMessage

`func (o *AiGatewayChatCompletionResponseChoicesInner) GetMessage() AiGatewayChatMessage`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *AiGatewayChatCompletionResponseChoicesInner) GetMessageOk() (*AiGatewayChatMessage, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *AiGatewayChatCompletionResponseChoicesInner) SetMessage(v AiGatewayChatMessage)`

SetMessage sets Message field to given value.


### GetFinishReason

`func (o *AiGatewayChatCompletionResponseChoicesInner) GetFinishReason() string`

GetFinishReason returns the FinishReason field if non-nil, zero value otherwise.

### GetFinishReasonOk

`func (o *AiGatewayChatCompletionResponseChoicesInner) GetFinishReasonOk() (*string, bool)`

GetFinishReasonOk returns a tuple with the FinishReason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFinishReason

`func (o *AiGatewayChatCompletionResponseChoicesInner) SetFinishReason(v string)`

SetFinishReason sets FinishReason field to given value.


### GetLogprobs

`func (o *AiGatewayChatCompletionResponseChoicesInner) GetLogprobs() interface{}`

GetLogprobs returns the Logprobs field if non-nil, zero value otherwise.

### GetLogprobsOk

`func (o *AiGatewayChatCompletionResponseChoicesInner) GetLogprobsOk() (*interface{}, bool)`

GetLogprobsOk returns a tuple with the Logprobs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogprobs

`func (o *AiGatewayChatCompletionResponseChoicesInner) SetLogprobs(v interface{})`

SetLogprobs sets Logprobs field to given value.

### HasLogprobs

`func (o *AiGatewayChatCompletionResponseChoicesInner) HasLogprobs() bool`

HasLogprobs returns a boolean if a field has been set.

### SetLogprobsNil

`func (o *AiGatewayChatCompletionResponseChoicesInner) SetLogprobsNil(b bool)`

 SetLogprobsNil sets the value for Logprobs to be an explicit nil

### UnsetLogprobs
`func (o *AiGatewayChatCompletionResponseChoicesInner) UnsetLogprobs()`

UnsetLogprobs ensures that no value is present for Logprobs, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



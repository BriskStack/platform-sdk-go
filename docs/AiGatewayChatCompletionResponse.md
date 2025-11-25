# AiGatewayChatCompletionResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Object** | **string** |  | 
**Created** | **int32** |  | 
**Model** | **string** |  | 
**Choices** | [**[]AiGatewayChatCompletionResponseChoicesInner**](AiGatewayChatCompletionResponseChoicesInner.md) |  | 
**Usage** | Pointer to [**AiGatewayChatCompletionResponseUsage**](AiGatewayChatCompletionResponseUsage.md) |  | [optional] 
**SystemFingerprint** | Pointer to **string** |  | [optional] 

## Methods

### NewAiGatewayChatCompletionResponse

`func NewAiGatewayChatCompletionResponse(id string, object string, created int32, model string, choices []AiGatewayChatCompletionResponseChoicesInner, ) *AiGatewayChatCompletionResponse`

NewAiGatewayChatCompletionResponse instantiates a new AiGatewayChatCompletionResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAiGatewayChatCompletionResponseWithDefaults

`func NewAiGatewayChatCompletionResponseWithDefaults() *AiGatewayChatCompletionResponse`

NewAiGatewayChatCompletionResponseWithDefaults instantiates a new AiGatewayChatCompletionResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *AiGatewayChatCompletionResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *AiGatewayChatCompletionResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *AiGatewayChatCompletionResponse) SetId(v string)`

SetId sets Id field to given value.


### GetObject

`func (o *AiGatewayChatCompletionResponse) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *AiGatewayChatCompletionResponse) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *AiGatewayChatCompletionResponse) SetObject(v string)`

SetObject sets Object field to given value.


### GetCreated

`func (o *AiGatewayChatCompletionResponse) GetCreated() int32`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *AiGatewayChatCompletionResponse) GetCreatedOk() (*int32, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *AiGatewayChatCompletionResponse) SetCreated(v int32)`

SetCreated sets Created field to given value.


### GetModel

`func (o *AiGatewayChatCompletionResponse) GetModel() string`

GetModel returns the Model field if non-nil, zero value otherwise.

### GetModelOk

`func (o *AiGatewayChatCompletionResponse) GetModelOk() (*string, bool)`

GetModelOk returns a tuple with the Model field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModel

`func (o *AiGatewayChatCompletionResponse) SetModel(v string)`

SetModel sets Model field to given value.


### GetChoices

`func (o *AiGatewayChatCompletionResponse) GetChoices() []AiGatewayChatCompletionResponseChoicesInner`

GetChoices returns the Choices field if non-nil, zero value otherwise.

### GetChoicesOk

`func (o *AiGatewayChatCompletionResponse) GetChoicesOk() (*[]AiGatewayChatCompletionResponseChoicesInner, bool)`

GetChoicesOk returns a tuple with the Choices field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChoices

`func (o *AiGatewayChatCompletionResponse) SetChoices(v []AiGatewayChatCompletionResponseChoicesInner)`

SetChoices sets Choices field to given value.


### GetUsage

`func (o *AiGatewayChatCompletionResponse) GetUsage() AiGatewayChatCompletionResponseUsage`

GetUsage returns the Usage field if non-nil, zero value otherwise.

### GetUsageOk

`func (o *AiGatewayChatCompletionResponse) GetUsageOk() (*AiGatewayChatCompletionResponseUsage, bool)`

GetUsageOk returns a tuple with the Usage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsage

`func (o *AiGatewayChatCompletionResponse) SetUsage(v AiGatewayChatCompletionResponseUsage)`

SetUsage sets Usage field to given value.

### HasUsage

`func (o *AiGatewayChatCompletionResponse) HasUsage() bool`

HasUsage returns a boolean if a field has been set.

### GetSystemFingerprint

`func (o *AiGatewayChatCompletionResponse) GetSystemFingerprint() string`

GetSystemFingerprint returns the SystemFingerprint field if non-nil, zero value otherwise.

### GetSystemFingerprintOk

`func (o *AiGatewayChatCompletionResponse) GetSystemFingerprintOk() (*string, bool)`

GetSystemFingerprintOk returns a tuple with the SystemFingerprint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSystemFingerprint

`func (o *AiGatewayChatCompletionResponse) SetSystemFingerprint(v string)`

SetSystemFingerprint sets SystemFingerprint field to given value.

### HasSystemFingerprint

`func (o *AiGatewayChatCompletionResponse) HasSystemFingerprint() bool`

HasSystemFingerprint returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



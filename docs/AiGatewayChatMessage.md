# AiGatewayChatMessage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Role** | **string** |  | 
**Content** | Pointer to **NullableString** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**ToolCalls** | Pointer to **[]interface{}** |  | [optional] 
**ToolCallId** | Pointer to **string** |  | [optional] 

## Methods

### NewAiGatewayChatMessage

`func NewAiGatewayChatMessage(role string, ) *AiGatewayChatMessage`

NewAiGatewayChatMessage instantiates a new AiGatewayChatMessage object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAiGatewayChatMessageWithDefaults

`func NewAiGatewayChatMessageWithDefaults() *AiGatewayChatMessage`

NewAiGatewayChatMessageWithDefaults instantiates a new AiGatewayChatMessage object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRole

`func (o *AiGatewayChatMessage) GetRole() string`

GetRole returns the Role field if non-nil, zero value otherwise.

### GetRoleOk

`func (o *AiGatewayChatMessage) GetRoleOk() (*string, bool)`

GetRoleOk returns a tuple with the Role field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRole

`func (o *AiGatewayChatMessage) SetRole(v string)`

SetRole sets Role field to given value.


### GetContent

`func (o *AiGatewayChatMessage) GetContent() string`

GetContent returns the Content field if non-nil, zero value otherwise.

### GetContentOk

`func (o *AiGatewayChatMessage) GetContentOk() (*string, bool)`

GetContentOk returns a tuple with the Content field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContent

`func (o *AiGatewayChatMessage) SetContent(v string)`

SetContent sets Content field to given value.

### HasContent

`func (o *AiGatewayChatMessage) HasContent() bool`

HasContent returns a boolean if a field has been set.

### SetContentNil

`func (o *AiGatewayChatMessage) SetContentNil(b bool)`

 SetContentNil sets the value for Content to be an explicit nil

### UnsetContent
`func (o *AiGatewayChatMessage) UnsetContent()`

UnsetContent ensures that no value is present for Content, not even an explicit nil
### GetName

`func (o *AiGatewayChatMessage) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *AiGatewayChatMessage) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *AiGatewayChatMessage) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *AiGatewayChatMessage) HasName() bool`

HasName returns a boolean if a field has been set.

### GetToolCalls

`func (o *AiGatewayChatMessage) GetToolCalls() []interface{}`

GetToolCalls returns the ToolCalls field if non-nil, zero value otherwise.

### GetToolCallsOk

`func (o *AiGatewayChatMessage) GetToolCallsOk() (*[]interface{}, bool)`

GetToolCallsOk returns a tuple with the ToolCalls field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToolCalls

`func (o *AiGatewayChatMessage) SetToolCalls(v []interface{})`

SetToolCalls sets ToolCalls field to given value.

### HasToolCalls

`func (o *AiGatewayChatMessage) HasToolCalls() bool`

HasToolCalls returns a boolean if a field has been set.

### GetToolCallId

`func (o *AiGatewayChatMessage) GetToolCallId() string`

GetToolCallId returns the ToolCallId field if non-nil, zero value otherwise.

### GetToolCallIdOk

`func (o *AiGatewayChatMessage) GetToolCallIdOk() (*string, bool)`

GetToolCallIdOk returns a tuple with the ToolCallId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToolCallId

`func (o *AiGatewayChatMessage) SetToolCallId(v string)`

SetToolCallId sets ToolCallId field to given value.

### HasToolCallId

`func (o *AiGatewayChatMessage) HasToolCallId() bool`

HasToolCallId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



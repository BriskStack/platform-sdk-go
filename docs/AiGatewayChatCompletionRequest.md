# AiGatewayChatCompletionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Model** | **string** | Model to use (e.g., \&quot;openai/gpt-4\&quot;, \&quot;anthropic/claude-3-5-sonnet-20241022\&quot;) | 
**Messages** | [**[]AiGatewayChatMessage**](AiGatewayChatMessage.md) | Array of messages in the conversation | 
**Temperature** | Pointer to **float32** | Sampling temperature (0-2) | [optional] 
**TopP** | Pointer to **float32** | Nucleus sampling parameter | [optional] 
**N** | Pointer to **int32** | Number of completions to generate | [optional] 
**Stream** | Pointer to **bool** | Whether to stream responses | [optional] 
**Stop** | Pointer to [**AiGatewayChatCompletionRequestStop**](AiGatewayChatCompletionRequestStop.md) |  | [optional] 
**MaxTokens** | Pointer to **int32** | Maximum tokens to generate | [optional] 
**PresencePenalty** | Pointer to **float32** | Presence penalty (-2 to 2) | [optional] 
**FrequencyPenalty** | Pointer to **float32** | Frequency penalty (-2 to 2) | [optional] 
**LogitBias** | Pointer to **map[string]float32** | Token logit bias | [optional] 
**User** | Pointer to **string** | Unique user identifier | [optional] 
**Tools** | Pointer to **[]interface{}** | Tools available for the model to call | [optional] 
**ToolChoice** | Pointer to **NullableString** |  | [optional] 
**ResponseFormat** | Pointer to [**AiGatewayChatCompletionRequestResponseFormat**](AiGatewayChatCompletionRequestResponseFormat.md) |  | [optional] 
**Seed** | Pointer to **int32** | Random seed for deterministic sampling | [optional] 

## Methods

### NewAiGatewayChatCompletionRequest

`func NewAiGatewayChatCompletionRequest(model string, messages []AiGatewayChatMessage, ) *AiGatewayChatCompletionRequest`

NewAiGatewayChatCompletionRequest instantiates a new AiGatewayChatCompletionRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAiGatewayChatCompletionRequestWithDefaults

`func NewAiGatewayChatCompletionRequestWithDefaults() *AiGatewayChatCompletionRequest`

NewAiGatewayChatCompletionRequestWithDefaults instantiates a new AiGatewayChatCompletionRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetModel

`func (o *AiGatewayChatCompletionRequest) GetModel() string`

GetModel returns the Model field if non-nil, zero value otherwise.

### GetModelOk

`func (o *AiGatewayChatCompletionRequest) GetModelOk() (*string, bool)`

GetModelOk returns a tuple with the Model field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModel

`func (o *AiGatewayChatCompletionRequest) SetModel(v string)`

SetModel sets Model field to given value.


### GetMessages

`func (o *AiGatewayChatCompletionRequest) GetMessages() []AiGatewayChatMessage`

GetMessages returns the Messages field if non-nil, zero value otherwise.

### GetMessagesOk

`func (o *AiGatewayChatCompletionRequest) GetMessagesOk() (*[]AiGatewayChatMessage, bool)`

GetMessagesOk returns a tuple with the Messages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessages

`func (o *AiGatewayChatCompletionRequest) SetMessages(v []AiGatewayChatMessage)`

SetMessages sets Messages field to given value.


### GetTemperature

`func (o *AiGatewayChatCompletionRequest) GetTemperature() float32`

GetTemperature returns the Temperature field if non-nil, zero value otherwise.

### GetTemperatureOk

`func (o *AiGatewayChatCompletionRequest) GetTemperatureOk() (*float32, bool)`

GetTemperatureOk returns a tuple with the Temperature field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemperature

`func (o *AiGatewayChatCompletionRequest) SetTemperature(v float32)`

SetTemperature sets Temperature field to given value.

### HasTemperature

`func (o *AiGatewayChatCompletionRequest) HasTemperature() bool`

HasTemperature returns a boolean if a field has been set.

### GetTopP

`func (o *AiGatewayChatCompletionRequest) GetTopP() float32`

GetTopP returns the TopP field if non-nil, zero value otherwise.

### GetTopPOk

`func (o *AiGatewayChatCompletionRequest) GetTopPOk() (*float32, bool)`

GetTopPOk returns a tuple with the TopP field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTopP

`func (o *AiGatewayChatCompletionRequest) SetTopP(v float32)`

SetTopP sets TopP field to given value.

### HasTopP

`func (o *AiGatewayChatCompletionRequest) HasTopP() bool`

HasTopP returns a boolean if a field has been set.

### GetN

`func (o *AiGatewayChatCompletionRequest) GetN() int32`

GetN returns the N field if non-nil, zero value otherwise.

### GetNOk

`func (o *AiGatewayChatCompletionRequest) GetNOk() (*int32, bool)`

GetNOk returns a tuple with the N field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetN

`func (o *AiGatewayChatCompletionRequest) SetN(v int32)`

SetN sets N field to given value.

### HasN

`func (o *AiGatewayChatCompletionRequest) HasN() bool`

HasN returns a boolean if a field has been set.

### GetStream

`func (o *AiGatewayChatCompletionRequest) GetStream() bool`

GetStream returns the Stream field if non-nil, zero value otherwise.

### GetStreamOk

`func (o *AiGatewayChatCompletionRequest) GetStreamOk() (*bool, bool)`

GetStreamOk returns a tuple with the Stream field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStream

`func (o *AiGatewayChatCompletionRequest) SetStream(v bool)`

SetStream sets Stream field to given value.

### HasStream

`func (o *AiGatewayChatCompletionRequest) HasStream() bool`

HasStream returns a boolean if a field has been set.

### GetStop

`func (o *AiGatewayChatCompletionRequest) GetStop() AiGatewayChatCompletionRequestStop`

GetStop returns the Stop field if non-nil, zero value otherwise.

### GetStopOk

`func (o *AiGatewayChatCompletionRequest) GetStopOk() (*AiGatewayChatCompletionRequestStop, bool)`

GetStopOk returns a tuple with the Stop field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStop

`func (o *AiGatewayChatCompletionRequest) SetStop(v AiGatewayChatCompletionRequestStop)`

SetStop sets Stop field to given value.

### HasStop

`func (o *AiGatewayChatCompletionRequest) HasStop() bool`

HasStop returns a boolean if a field has been set.

### GetMaxTokens

`func (o *AiGatewayChatCompletionRequest) GetMaxTokens() int32`

GetMaxTokens returns the MaxTokens field if non-nil, zero value otherwise.

### GetMaxTokensOk

`func (o *AiGatewayChatCompletionRequest) GetMaxTokensOk() (*int32, bool)`

GetMaxTokensOk returns a tuple with the MaxTokens field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxTokens

`func (o *AiGatewayChatCompletionRequest) SetMaxTokens(v int32)`

SetMaxTokens sets MaxTokens field to given value.

### HasMaxTokens

`func (o *AiGatewayChatCompletionRequest) HasMaxTokens() bool`

HasMaxTokens returns a boolean if a field has been set.

### GetPresencePenalty

`func (o *AiGatewayChatCompletionRequest) GetPresencePenalty() float32`

GetPresencePenalty returns the PresencePenalty field if non-nil, zero value otherwise.

### GetPresencePenaltyOk

`func (o *AiGatewayChatCompletionRequest) GetPresencePenaltyOk() (*float32, bool)`

GetPresencePenaltyOk returns a tuple with the PresencePenalty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPresencePenalty

`func (o *AiGatewayChatCompletionRequest) SetPresencePenalty(v float32)`

SetPresencePenalty sets PresencePenalty field to given value.

### HasPresencePenalty

`func (o *AiGatewayChatCompletionRequest) HasPresencePenalty() bool`

HasPresencePenalty returns a boolean if a field has been set.

### GetFrequencyPenalty

`func (o *AiGatewayChatCompletionRequest) GetFrequencyPenalty() float32`

GetFrequencyPenalty returns the FrequencyPenalty field if non-nil, zero value otherwise.

### GetFrequencyPenaltyOk

`func (o *AiGatewayChatCompletionRequest) GetFrequencyPenaltyOk() (*float32, bool)`

GetFrequencyPenaltyOk returns a tuple with the FrequencyPenalty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrequencyPenalty

`func (o *AiGatewayChatCompletionRequest) SetFrequencyPenalty(v float32)`

SetFrequencyPenalty sets FrequencyPenalty field to given value.

### HasFrequencyPenalty

`func (o *AiGatewayChatCompletionRequest) HasFrequencyPenalty() bool`

HasFrequencyPenalty returns a boolean if a field has been set.

### GetLogitBias

`func (o *AiGatewayChatCompletionRequest) GetLogitBias() map[string]float32`

GetLogitBias returns the LogitBias field if non-nil, zero value otherwise.

### GetLogitBiasOk

`func (o *AiGatewayChatCompletionRequest) GetLogitBiasOk() (*map[string]float32, bool)`

GetLogitBiasOk returns a tuple with the LogitBias field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogitBias

`func (o *AiGatewayChatCompletionRequest) SetLogitBias(v map[string]float32)`

SetLogitBias sets LogitBias field to given value.

### HasLogitBias

`func (o *AiGatewayChatCompletionRequest) HasLogitBias() bool`

HasLogitBias returns a boolean if a field has been set.

### GetUser

`func (o *AiGatewayChatCompletionRequest) GetUser() string`

GetUser returns the User field if non-nil, zero value otherwise.

### GetUserOk

`func (o *AiGatewayChatCompletionRequest) GetUserOk() (*string, bool)`

GetUserOk returns a tuple with the User field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUser

`func (o *AiGatewayChatCompletionRequest) SetUser(v string)`

SetUser sets User field to given value.

### HasUser

`func (o *AiGatewayChatCompletionRequest) HasUser() bool`

HasUser returns a boolean if a field has been set.

### GetTools

`func (o *AiGatewayChatCompletionRequest) GetTools() []interface{}`

GetTools returns the Tools field if non-nil, zero value otherwise.

### GetToolsOk

`func (o *AiGatewayChatCompletionRequest) GetToolsOk() (*[]interface{}, bool)`

GetToolsOk returns a tuple with the Tools field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTools

`func (o *AiGatewayChatCompletionRequest) SetTools(v []interface{})`

SetTools sets Tools field to given value.

### HasTools

`func (o *AiGatewayChatCompletionRequest) HasTools() bool`

HasTools returns a boolean if a field has been set.

### GetToolChoice

`func (o *AiGatewayChatCompletionRequest) GetToolChoice() string`

GetToolChoice returns the ToolChoice field if non-nil, zero value otherwise.

### GetToolChoiceOk

`func (o *AiGatewayChatCompletionRequest) GetToolChoiceOk() (*string, bool)`

GetToolChoiceOk returns a tuple with the ToolChoice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToolChoice

`func (o *AiGatewayChatCompletionRequest) SetToolChoice(v string)`

SetToolChoice sets ToolChoice field to given value.

### HasToolChoice

`func (o *AiGatewayChatCompletionRequest) HasToolChoice() bool`

HasToolChoice returns a boolean if a field has been set.

### SetToolChoiceNil

`func (o *AiGatewayChatCompletionRequest) SetToolChoiceNil(b bool)`

 SetToolChoiceNil sets the value for ToolChoice to be an explicit nil

### UnsetToolChoice
`func (o *AiGatewayChatCompletionRequest) UnsetToolChoice()`

UnsetToolChoice ensures that no value is present for ToolChoice, not even an explicit nil
### GetResponseFormat

`func (o *AiGatewayChatCompletionRequest) GetResponseFormat() AiGatewayChatCompletionRequestResponseFormat`

GetResponseFormat returns the ResponseFormat field if non-nil, zero value otherwise.

### GetResponseFormatOk

`func (o *AiGatewayChatCompletionRequest) GetResponseFormatOk() (*AiGatewayChatCompletionRequestResponseFormat, bool)`

GetResponseFormatOk returns a tuple with the ResponseFormat field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseFormat

`func (o *AiGatewayChatCompletionRequest) SetResponseFormat(v AiGatewayChatCompletionRequestResponseFormat)`

SetResponseFormat sets ResponseFormat field to given value.

### HasResponseFormat

`func (o *AiGatewayChatCompletionRequest) HasResponseFormat() bool`

HasResponseFormat returns a boolean if a field has been set.

### GetSeed

`func (o *AiGatewayChatCompletionRequest) GetSeed() int32`

GetSeed returns the Seed field if non-nil, zero value otherwise.

### GetSeedOk

`func (o *AiGatewayChatCompletionRequest) GetSeedOk() (*int32, bool)`

GetSeedOk returns a tuple with the Seed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeed

`func (o *AiGatewayChatCompletionRequest) SetSeed(v int32)`

SetSeed sets Seed field to given value.

### HasSeed

`func (o *AiGatewayChatCompletionRequest) HasSeed() bool`

HasSeed returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AiGatewayHealthzResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Status** | **string** | Health status indicator | 
**Service** | **string** | Service name | 
**Environment** | **string** | Deployment environment | 
**Version** | **string** | Service version | 
**Timestamp** | **time.Time** | Current server time in ISO 8601 format | 
**Uptime** | Pointer to **float32** | Service uptime in seconds (if available) | [optional] 

## Methods

### NewAiGatewayHealthzResponse

`func NewAiGatewayHealthzResponse(status string, service string, environment string, version string, timestamp time.Time, ) *AiGatewayHealthzResponse`

NewAiGatewayHealthzResponse instantiates a new AiGatewayHealthzResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAiGatewayHealthzResponseWithDefaults

`func NewAiGatewayHealthzResponseWithDefaults() *AiGatewayHealthzResponse`

NewAiGatewayHealthzResponseWithDefaults instantiates a new AiGatewayHealthzResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetStatus

`func (o *AiGatewayHealthzResponse) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *AiGatewayHealthzResponse) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *AiGatewayHealthzResponse) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetService

`func (o *AiGatewayHealthzResponse) GetService() string`

GetService returns the Service field if non-nil, zero value otherwise.

### GetServiceOk

`func (o *AiGatewayHealthzResponse) GetServiceOk() (*string, bool)`

GetServiceOk returns a tuple with the Service field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetService

`func (o *AiGatewayHealthzResponse) SetService(v string)`

SetService sets Service field to given value.


### GetEnvironment

`func (o *AiGatewayHealthzResponse) GetEnvironment() string`

GetEnvironment returns the Environment field if non-nil, zero value otherwise.

### GetEnvironmentOk

`func (o *AiGatewayHealthzResponse) GetEnvironmentOk() (*string, bool)`

GetEnvironmentOk returns a tuple with the Environment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnvironment

`func (o *AiGatewayHealthzResponse) SetEnvironment(v string)`

SetEnvironment sets Environment field to given value.


### GetVersion

`func (o *AiGatewayHealthzResponse) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *AiGatewayHealthzResponse) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *AiGatewayHealthzResponse) SetVersion(v string)`

SetVersion sets Version field to given value.


### GetTimestamp

`func (o *AiGatewayHealthzResponse) GetTimestamp() time.Time`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *AiGatewayHealthzResponse) GetTimestampOk() (*time.Time, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *AiGatewayHealthzResponse) SetTimestamp(v time.Time)`

SetTimestamp sets Timestamp field to given value.


### GetUptime

`func (o *AiGatewayHealthzResponse) GetUptime() float32`

GetUptime returns the Uptime field if non-nil, zero value otherwise.

### GetUptimeOk

`func (o *AiGatewayHealthzResponse) GetUptimeOk() (*float32, bool)`

GetUptimeOk returns a tuple with the Uptime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUptime

`func (o *AiGatewayHealthzResponse) SetUptime(v float32)`

SetUptime sets Uptime field to given value.

### HasUptime

`func (o *AiGatewayHealthzResponse) HasUptime() bool`

HasUptime returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# HelloWorldHealthzResponse

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

### NewHelloWorldHealthzResponse

`func NewHelloWorldHealthzResponse(status string, service string, environment string, version string, timestamp time.Time, ) *HelloWorldHealthzResponse`

NewHelloWorldHealthzResponse instantiates a new HelloWorldHealthzResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewHelloWorldHealthzResponseWithDefaults

`func NewHelloWorldHealthzResponseWithDefaults() *HelloWorldHealthzResponse`

NewHelloWorldHealthzResponseWithDefaults instantiates a new HelloWorldHealthzResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetStatus

`func (o *HelloWorldHealthzResponse) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *HelloWorldHealthzResponse) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *HelloWorldHealthzResponse) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetService

`func (o *HelloWorldHealthzResponse) GetService() string`

GetService returns the Service field if non-nil, zero value otherwise.

### GetServiceOk

`func (o *HelloWorldHealthzResponse) GetServiceOk() (*string, bool)`

GetServiceOk returns a tuple with the Service field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetService

`func (o *HelloWorldHealthzResponse) SetService(v string)`

SetService sets Service field to given value.


### GetEnvironment

`func (o *HelloWorldHealthzResponse) GetEnvironment() string`

GetEnvironment returns the Environment field if non-nil, zero value otherwise.

### GetEnvironmentOk

`func (o *HelloWorldHealthzResponse) GetEnvironmentOk() (*string, bool)`

GetEnvironmentOk returns a tuple with the Environment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnvironment

`func (o *HelloWorldHealthzResponse) SetEnvironment(v string)`

SetEnvironment sets Environment field to given value.


### GetVersion

`func (o *HelloWorldHealthzResponse) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *HelloWorldHealthzResponse) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *HelloWorldHealthzResponse) SetVersion(v string)`

SetVersion sets Version field to given value.


### GetTimestamp

`func (o *HelloWorldHealthzResponse) GetTimestamp() time.Time`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *HelloWorldHealthzResponse) GetTimestampOk() (*time.Time, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *HelloWorldHealthzResponse) SetTimestamp(v time.Time)`

SetTimestamp sets Timestamp field to given value.


### GetUptime

`func (o *HelloWorldHealthzResponse) GetUptime() float32`

GetUptime returns the Uptime field if non-nil, zero value otherwise.

### GetUptimeOk

`func (o *HelloWorldHealthzResponse) GetUptimeOk() (*float32, bool)`

GetUptimeOk returns a tuple with the Uptime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUptime

`func (o *HelloWorldHealthzResponse) SetUptime(v float32)`

SetUptime sets Uptime field to given value.

### HasUptime

`func (o *HelloWorldHealthzResponse) HasUptime() bool`

HasUptime returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



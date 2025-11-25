# HelloWorldHelloResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Message** | **string** | Greeting message | 
**Service** | **string** | Service name | 
**Environment** | **string** | Environment (development/staging/production) | 
**Timestamp** | **time.Time** | ISO 8601 timestamp | 
**Version** | **string** | Service version | 

## Methods

### NewHelloWorldHelloResponse

`func NewHelloWorldHelloResponse(message string, service string, environment string, timestamp time.Time, version string, ) *HelloWorldHelloResponse`

NewHelloWorldHelloResponse instantiates a new HelloWorldHelloResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewHelloWorldHelloResponseWithDefaults

`func NewHelloWorldHelloResponseWithDefaults() *HelloWorldHelloResponse`

NewHelloWorldHelloResponseWithDefaults instantiates a new HelloWorldHelloResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMessage

`func (o *HelloWorldHelloResponse) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *HelloWorldHelloResponse) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *HelloWorldHelloResponse) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetService

`func (o *HelloWorldHelloResponse) GetService() string`

GetService returns the Service field if non-nil, zero value otherwise.

### GetServiceOk

`func (o *HelloWorldHelloResponse) GetServiceOk() (*string, bool)`

GetServiceOk returns a tuple with the Service field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetService

`func (o *HelloWorldHelloResponse) SetService(v string)`

SetService sets Service field to given value.


### GetEnvironment

`func (o *HelloWorldHelloResponse) GetEnvironment() string`

GetEnvironment returns the Environment field if non-nil, zero value otherwise.

### GetEnvironmentOk

`func (o *HelloWorldHelloResponse) GetEnvironmentOk() (*string, bool)`

GetEnvironmentOk returns a tuple with the Environment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnvironment

`func (o *HelloWorldHelloResponse) SetEnvironment(v string)`

SetEnvironment sets Environment field to given value.


### GetTimestamp

`func (o *HelloWorldHelloResponse) GetTimestamp() time.Time`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *HelloWorldHelloResponse) GetTimestampOk() (*time.Time, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *HelloWorldHelloResponse) SetTimestamp(v time.Time)`

SetTimestamp sets Timestamp field to given value.


### GetVersion

`func (o *HelloWorldHelloResponse) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *HelloWorldHelloResponse) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *HelloWorldHelloResponse) SetVersion(v string)`

SetVersion sets Version field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



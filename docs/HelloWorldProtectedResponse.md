# HelloWorldProtectedResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Message** | **string** | Success message | 
**UserId** | **string** | Authenticated user or service ID (from auth.sub) | 
**Roles** | **[]string** | User roles or service scopes (from auth.roles) | 
**Timestamp** | **time.Time** | ISO 8601 timestamp | 

## Methods

### NewHelloWorldProtectedResponse

`func NewHelloWorldProtectedResponse(message string, userId string, roles []string, timestamp time.Time, ) *HelloWorldProtectedResponse`

NewHelloWorldProtectedResponse instantiates a new HelloWorldProtectedResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewHelloWorldProtectedResponseWithDefaults

`func NewHelloWorldProtectedResponseWithDefaults() *HelloWorldProtectedResponse`

NewHelloWorldProtectedResponseWithDefaults instantiates a new HelloWorldProtectedResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMessage

`func (o *HelloWorldProtectedResponse) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *HelloWorldProtectedResponse) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *HelloWorldProtectedResponse) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetUserId

`func (o *HelloWorldProtectedResponse) GetUserId() string`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *HelloWorldProtectedResponse) GetUserIdOk() (*string, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *HelloWorldProtectedResponse) SetUserId(v string)`

SetUserId sets UserId field to given value.


### GetRoles

`func (o *HelloWorldProtectedResponse) GetRoles() []string`

GetRoles returns the Roles field if non-nil, zero value otherwise.

### GetRolesOk

`func (o *HelloWorldProtectedResponse) GetRolesOk() (*[]string, bool)`

GetRolesOk returns a tuple with the Roles field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoles

`func (o *HelloWorldProtectedResponse) SetRoles(v []string)`

SetRoles sets Roles field to given value.


### GetTimestamp

`func (o *HelloWorldProtectedResponse) GetTimestamp() time.Time`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *HelloWorldProtectedResponse) GetTimestampOk() (*time.Time, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *HelloWorldProtectedResponse) SetTimestamp(v time.Time)`

SetTimestamp sets Timestamp field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



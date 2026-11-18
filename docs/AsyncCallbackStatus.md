# AsyncCallbackStatus

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RequestId** | **string** |  | 
**State** | **string** | &#x60;pending&#x60;: the call is still running. &#x60;delivering&#x60;: an attempt is under way or the next retry is due at &#x60;next_attempt_at&#x60;. &#x60;delivered&#x60;: the endpoint answered 2xx. &#x60;failed&#x60;: every attempt failed, a final status (not 408/429/5xx) came back, or a gateway restart interrupted the delivery (&#x60;last_error&#x60; \&quot;interrupted (gateway restart)\&quot;). | 
**Attempts** | **int32** |  | 
**LastStatus** | Pointer to **NullableInt32** |  | [optional] 
**LastError** | Pointer to **NullableString** |  | [optional] 
**NextAttemptAt** | Pointer to **NullableInt32** |  | [optional] 
**DeliveredAt** | Pointer to **NullableInt32** |  | [optional] 
**CallbackHost** | **string** | Host of the callback URL only (never its path or query). | 

## Methods

### NewAsyncCallbackStatus

`func NewAsyncCallbackStatus(requestId string, state string, attempts int32, callbackHost string, ) *AsyncCallbackStatus`

NewAsyncCallbackStatus instantiates a new AsyncCallbackStatus object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAsyncCallbackStatusWithDefaults

`func NewAsyncCallbackStatusWithDefaults() *AsyncCallbackStatus`

NewAsyncCallbackStatusWithDefaults instantiates a new AsyncCallbackStatus object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRequestId

`func (o *AsyncCallbackStatus) GetRequestId() string`

GetRequestId returns the RequestId field if non-nil, zero value otherwise.

### GetRequestIdOk

`func (o *AsyncCallbackStatus) GetRequestIdOk() (*string, bool)`

GetRequestIdOk returns a tuple with the RequestId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequestId

`func (o *AsyncCallbackStatus) SetRequestId(v string)`

SetRequestId sets RequestId field to given value.


### GetState

`func (o *AsyncCallbackStatus) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *AsyncCallbackStatus) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *AsyncCallbackStatus) SetState(v string)`

SetState sets State field to given value.


### GetAttempts

`func (o *AsyncCallbackStatus) GetAttempts() int32`

GetAttempts returns the Attempts field if non-nil, zero value otherwise.

### GetAttemptsOk

`func (o *AsyncCallbackStatus) GetAttemptsOk() (*int32, bool)`

GetAttemptsOk returns a tuple with the Attempts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttempts

`func (o *AsyncCallbackStatus) SetAttempts(v int32)`

SetAttempts sets Attempts field to given value.


### GetLastStatus

`func (o *AsyncCallbackStatus) GetLastStatus() int32`

GetLastStatus returns the LastStatus field if non-nil, zero value otherwise.

### GetLastStatusOk

`func (o *AsyncCallbackStatus) GetLastStatusOk() (*int32, bool)`

GetLastStatusOk returns a tuple with the LastStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastStatus

`func (o *AsyncCallbackStatus) SetLastStatus(v int32)`

SetLastStatus sets LastStatus field to given value.

### HasLastStatus

`func (o *AsyncCallbackStatus) HasLastStatus() bool`

HasLastStatus returns a boolean if a field has been set.

### SetLastStatusNil

`func (o *AsyncCallbackStatus) SetLastStatusNil(b bool)`

 SetLastStatusNil sets the value for LastStatus to be an explicit nil

### UnsetLastStatus
`func (o *AsyncCallbackStatus) UnsetLastStatus()`

UnsetLastStatus ensures that no value is present for LastStatus, not even an explicit nil
### GetLastError

`func (o *AsyncCallbackStatus) GetLastError() string`

GetLastError returns the LastError field if non-nil, zero value otherwise.

### GetLastErrorOk

`func (o *AsyncCallbackStatus) GetLastErrorOk() (*string, bool)`

GetLastErrorOk returns a tuple with the LastError field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastError

`func (o *AsyncCallbackStatus) SetLastError(v string)`

SetLastError sets LastError field to given value.

### HasLastError

`func (o *AsyncCallbackStatus) HasLastError() bool`

HasLastError returns a boolean if a field has been set.

### SetLastErrorNil

`func (o *AsyncCallbackStatus) SetLastErrorNil(b bool)`

 SetLastErrorNil sets the value for LastError to be an explicit nil

### UnsetLastError
`func (o *AsyncCallbackStatus) UnsetLastError()`

UnsetLastError ensures that no value is present for LastError, not even an explicit nil
### GetNextAttemptAt

`func (o *AsyncCallbackStatus) GetNextAttemptAt() int32`

GetNextAttemptAt returns the NextAttemptAt field if non-nil, zero value otherwise.

### GetNextAttemptAtOk

`func (o *AsyncCallbackStatus) GetNextAttemptAtOk() (*int32, bool)`

GetNextAttemptAtOk returns a tuple with the NextAttemptAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextAttemptAt

`func (o *AsyncCallbackStatus) SetNextAttemptAt(v int32)`

SetNextAttemptAt sets NextAttemptAt field to given value.

### HasNextAttemptAt

`func (o *AsyncCallbackStatus) HasNextAttemptAt() bool`

HasNextAttemptAt returns a boolean if a field has been set.

### SetNextAttemptAtNil

`func (o *AsyncCallbackStatus) SetNextAttemptAtNil(b bool)`

 SetNextAttemptAtNil sets the value for NextAttemptAt to be an explicit nil

### UnsetNextAttemptAt
`func (o *AsyncCallbackStatus) UnsetNextAttemptAt()`

UnsetNextAttemptAt ensures that no value is present for NextAttemptAt, not even an explicit nil
### GetDeliveredAt

`func (o *AsyncCallbackStatus) GetDeliveredAt() int32`

GetDeliveredAt returns the DeliveredAt field if non-nil, zero value otherwise.

### GetDeliveredAtOk

`func (o *AsyncCallbackStatus) GetDeliveredAtOk() (*int32, bool)`

GetDeliveredAtOk returns a tuple with the DeliveredAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeliveredAt

`func (o *AsyncCallbackStatus) SetDeliveredAt(v int32)`

SetDeliveredAt sets DeliveredAt field to given value.

### HasDeliveredAt

`func (o *AsyncCallbackStatus) HasDeliveredAt() bool`

HasDeliveredAt returns a boolean if a field has been set.

### SetDeliveredAtNil

`func (o *AsyncCallbackStatus) SetDeliveredAtNil(b bool)`

 SetDeliveredAtNil sets the value for DeliveredAt to be an explicit nil

### UnsetDeliveredAt
`func (o *AsyncCallbackStatus) UnsetDeliveredAt()`

UnsetDeliveredAt ensures that no value is present for DeliveredAt, not even an explicit nil
### GetCallbackHost

`func (o *AsyncCallbackStatus) GetCallbackHost() string`

GetCallbackHost returns the CallbackHost field if non-nil, zero value otherwise.

### GetCallbackHostOk

`func (o *AsyncCallbackStatus) GetCallbackHostOk() (*string, bool)`

GetCallbackHostOk returns a tuple with the CallbackHost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCallbackHost

`func (o *AsyncCallbackStatus) SetCallbackHost(v string)`

SetCallbackHost sets CallbackHost field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



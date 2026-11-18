# AsyncAccepted

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RequestId** | **string** |  | 
**Status** | **string** |  | 
**RetryAfterSeconds** | **int32** |  | 
**NextAction** | [**AsyncAcceptedNextAction**](AsyncAcceptedNextAction.md) |  | 
**Detail** | Pointer to **string** |  | [optional] 
**Callback** | Pointer to **map[string]interface{}** | Only on a poll of a call submitted with a callback: the delivery state so far (&#x60;status&#x60;, &#x60;attempts&#x60;, &#x60;last_error&#x60;). | [optional] 

## Methods

### NewAsyncAccepted

`func NewAsyncAccepted(requestId string, status string, retryAfterSeconds int32, nextAction AsyncAcceptedNextAction, ) *AsyncAccepted`

NewAsyncAccepted instantiates a new AsyncAccepted object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAsyncAcceptedWithDefaults

`func NewAsyncAcceptedWithDefaults() *AsyncAccepted`

NewAsyncAcceptedWithDefaults instantiates a new AsyncAccepted object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRequestId

`func (o *AsyncAccepted) GetRequestId() string`

GetRequestId returns the RequestId field if non-nil, zero value otherwise.

### GetRequestIdOk

`func (o *AsyncAccepted) GetRequestIdOk() (*string, bool)`

GetRequestIdOk returns a tuple with the RequestId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequestId

`func (o *AsyncAccepted) SetRequestId(v string)`

SetRequestId sets RequestId field to given value.


### GetStatus

`func (o *AsyncAccepted) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *AsyncAccepted) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *AsyncAccepted) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetRetryAfterSeconds

`func (o *AsyncAccepted) GetRetryAfterSeconds() int32`

GetRetryAfterSeconds returns the RetryAfterSeconds field if non-nil, zero value otherwise.

### GetRetryAfterSecondsOk

`func (o *AsyncAccepted) GetRetryAfterSecondsOk() (*int32, bool)`

GetRetryAfterSecondsOk returns a tuple with the RetryAfterSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRetryAfterSeconds

`func (o *AsyncAccepted) SetRetryAfterSeconds(v int32)`

SetRetryAfterSeconds sets RetryAfterSeconds field to given value.


### GetNextAction

`func (o *AsyncAccepted) GetNextAction() AsyncAcceptedNextAction`

GetNextAction returns the NextAction field if non-nil, zero value otherwise.

### GetNextActionOk

`func (o *AsyncAccepted) GetNextActionOk() (*AsyncAcceptedNextAction, bool)`

GetNextActionOk returns a tuple with the NextAction field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextAction

`func (o *AsyncAccepted) SetNextAction(v AsyncAcceptedNextAction)`

SetNextAction sets NextAction field to given value.


### GetDetail

`func (o *AsyncAccepted) GetDetail() string`

GetDetail returns the Detail field if non-nil, zero value otherwise.

### GetDetailOk

`func (o *AsyncAccepted) GetDetailOk() (*string, bool)`

GetDetailOk returns a tuple with the Detail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDetail

`func (o *AsyncAccepted) SetDetail(v string)`

SetDetail sets Detail field to given value.

### HasDetail

`func (o *AsyncAccepted) HasDetail() bool`

HasDetail returns a boolean if a field has been set.

### GetCallback

`func (o *AsyncAccepted) GetCallback() map[string]interface{}`

GetCallback returns the Callback field if non-nil, zero value otherwise.

### GetCallbackOk

`func (o *AsyncAccepted) GetCallbackOk() (*map[string]interface{}, bool)`

GetCallbackOk returns a tuple with the Callback field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCallback

`func (o *AsyncAccepted) SetCallback(v map[string]interface{})`

SetCallback sets Callback field to given value.

### HasCallback

`func (o *AsyncAccepted) HasCallback() bool`

HasCallback returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



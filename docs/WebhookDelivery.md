# WebhookDelivery

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RequestId** | **string** |  | 
**Endpoint** | **string** | Path of the call, e.g. &#x60;/v1/perplexity/ask&#x60; (never its query). | 
**State** | **string** | &#x60;pending&#x60;: the call is still running. &#x60;delivering&#x60;: an attempt is under way or the next retry is due at &#x60;next_attempt_at&#x60;. &#x60;delivered&#x60;: the endpoint answered 2xx. &#x60;failed&#x60;: every attempt failed, a final status (not 408/429/5xx) came back, or a gateway restart interrupted the delivery (&#x60;last_error&#x60; \&quot;interrupted (gateway restart)\&quot;). | 
**Attempts** | **int32** |  | 
**LastStatus** | Pointer to **NullableInt32** |  | [optional] 
**LastError** | Pointer to **NullableString** |  | [optional] 
**CreatedAt** | **int32** | Unix time the call was submitted. | 
**DeliveredAt** | Pointer to **NullableInt32** |  | [optional] 
**CallbackHost** | **string** |  | 

## Methods

### NewWebhookDelivery

`func NewWebhookDelivery(requestId string, endpoint string, state string, attempts int32, createdAt int32, callbackHost string, ) *WebhookDelivery`

NewWebhookDelivery instantiates a new WebhookDelivery object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebhookDeliveryWithDefaults

`func NewWebhookDeliveryWithDefaults() *WebhookDelivery`

NewWebhookDeliveryWithDefaults instantiates a new WebhookDelivery object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRequestId

`func (o *WebhookDelivery) GetRequestId() string`

GetRequestId returns the RequestId field if non-nil, zero value otherwise.

### GetRequestIdOk

`func (o *WebhookDelivery) GetRequestIdOk() (*string, bool)`

GetRequestIdOk returns a tuple with the RequestId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequestId

`func (o *WebhookDelivery) SetRequestId(v string)`

SetRequestId sets RequestId field to given value.


### GetEndpoint

`func (o *WebhookDelivery) GetEndpoint() string`

GetEndpoint returns the Endpoint field if non-nil, zero value otherwise.

### GetEndpointOk

`func (o *WebhookDelivery) GetEndpointOk() (*string, bool)`

GetEndpointOk returns a tuple with the Endpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndpoint

`func (o *WebhookDelivery) SetEndpoint(v string)`

SetEndpoint sets Endpoint field to given value.


### GetState

`func (o *WebhookDelivery) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *WebhookDelivery) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *WebhookDelivery) SetState(v string)`

SetState sets State field to given value.


### GetAttempts

`func (o *WebhookDelivery) GetAttempts() int32`

GetAttempts returns the Attempts field if non-nil, zero value otherwise.

### GetAttemptsOk

`func (o *WebhookDelivery) GetAttemptsOk() (*int32, bool)`

GetAttemptsOk returns a tuple with the Attempts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttempts

`func (o *WebhookDelivery) SetAttempts(v int32)`

SetAttempts sets Attempts field to given value.


### GetLastStatus

`func (o *WebhookDelivery) GetLastStatus() int32`

GetLastStatus returns the LastStatus field if non-nil, zero value otherwise.

### GetLastStatusOk

`func (o *WebhookDelivery) GetLastStatusOk() (*int32, bool)`

GetLastStatusOk returns a tuple with the LastStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastStatus

`func (o *WebhookDelivery) SetLastStatus(v int32)`

SetLastStatus sets LastStatus field to given value.

### HasLastStatus

`func (o *WebhookDelivery) HasLastStatus() bool`

HasLastStatus returns a boolean if a field has been set.

### SetLastStatusNil

`func (o *WebhookDelivery) SetLastStatusNil(b bool)`

 SetLastStatusNil sets the value for LastStatus to be an explicit nil

### UnsetLastStatus
`func (o *WebhookDelivery) UnsetLastStatus()`

UnsetLastStatus ensures that no value is present for LastStatus, not even an explicit nil
### GetLastError

`func (o *WebhookDelivery) GetLastError() string`

GetLastError returns the LastError field if non-nil, zero value otherwise.

### GetLastErrorOk

`func (o *WebhookDelivery) GetLastErrorOk() (*string, bool)`

GetLastErrorOk returns a tuple with the LastError field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastError

`func (o *WebhookDelivery) SetLastError(v string)`

SetLastError sets LastError field to given value.

### HasLastError

`func (o *WebhookDelivery) HasLastError() bool`

HasLastError returns a boolean if a field has been set.

### SetLastErrorNil

`func (o *WebhookDelivery) SetLastErrorNil(b bool)`

 SetLastErrorNil sets the value for LastError to be an explicit nil

### UnsetLastError
`func (o *WebhookDelivery) UnsetLastError()`

UnsetLastError ensures that no value is present for LastError, not even an explicit nil
### GetCreatedAt

`func (o *WebhookDelivery) GetCreatedAt() int32`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *WebhookDelivery) GetCreatedAtOk() (*int32, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *WebhookDelivery) SetCreatedAt(v int32)`

SetCreatedAt sets CreatedAt field to given value.


### GetDeliveredAt

`func (o *WebhookDelivery) GetDeliveredAt() int32`

GetDeliveredAt returns the DeliveredAt field if non-nil, zero value otherwise.

### GetDeliveredAtOk

`func (o *WebhookDelivery) GetDeliveredAtOk() (*int32, bool)`

GetDeliveredAtOk returns a tuple with the DeliveredAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeliveredAt

`func (o *WebhookDelivery) SetDeliveredAt(v int32)`

SetDeliveredAt sets DeliveredAt field to given value.

### HasDeliveredAt

`func (o *WebhookDelivery) HasDeliveredAt() bool`

HasDeliveredAt returns a boolean if a field has been set.

### SetDeliveredAtNil

`func (o *WebhookDelivery) SetDeliveredAtNil(b bool)`

 SetDeliveredAtNil sets the value for DeliveredAt to be an explicit nil

### UnsetDeliveredAt
`func (o *WebhookDelivery) UnsetDeliveredAt()`

UnsetDeliveredAt ensures that no value is present for DeliveredAt, not even an explicit nil
### GetCallbackHost

`func (o *WebhookDelivery) GetCallbackHost() string`

GetCallbackHost returns the CallbackHost field if non-nil, zero value otherwise.

### GetCallbackHostOk

`func (o *WebhookDelivery) GetCallbackHostOk() (*string, bool)`

GetCallbackHostOk returns a tuple with the CallbackHost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCallbackHost

`func (o *WebhookDelivery) SetCallbackHost(v string)`

SetCallbackHost sets CallbackHost field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



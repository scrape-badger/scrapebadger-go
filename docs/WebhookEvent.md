# WebhookEvent

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Event** | **string** |  | 
**RequestId** | **NullableString** |  | 
**BatchId** | **NullableString** |  | 
**Status** | **int32** | The call&#39;s own HTTP status. | 
**Headers** | **map[string]string** | The call&#39;s kept response headers, lower-case (content-type, x-credits-used, x-request-duration-ms, x-api-tier). | 
**ResultUrl** | **NullableString** |  | 
**ResultExpiresAt** | **int32** | Unix time. | 
**BodySize** | **NullableInt32** |  | 
**Body** | **interface{}** |  | 
**BodyOmitted** | Pointer to **bool** | Present (true) when the body was over 1 MB: fetch &#x60;result_url&#x60;. | [optional] 
**Attempt** | **NullableInt32** |  | 
**SentAt** | **int32** | Unix time of this attempt. | 

## Methods

### NewWebhookEvent

`func NewWebhookEvent(event string, requestId NullableString, batchId NullableString, status int32, headers map[string]string, resultUrl NullableString, resultExpiresAt int32, bodySize NullableInt32, body interface{}, attempt NullableInt32, sentAt int32, ) *WebhookEvent`

NewWebhookEvent instantiates a new WebhookEvent object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebhookEventWithDefaults

`func NewWebhookEventWithDefaults() *WebhookEvent`

NewWebhookEventWithDefaults instantiates a new WebhookEvent object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEvent

`func (o *WebhookEvent) GetEvent() string`

GetEvent returns the Event field if non-nil, zero value otherwise.

### GetEventOk

`func (o *WebhookEvent) GetEventOk() (*string, bool)`

GetEventOk returns a tuple with the Event field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvent

`func (o *WebhookEvent) SetEvent(v string)`

SetEvent sets Event field to given value.


### GetRequestId

`func (o *WebhookEvent) GetRequestId() string`

GetRequestId returns the RequestId field if non-nil, zero value otherwise.

### GetRequestIdOk

`func (o *WebhookEvent) GetRequestIdOk() (*string, bool)`

GetRequestIdOk returns a tuple with the RequestId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequestId

`func (o *WebhookEvent) SetRequestId(v string)`

SetRequestId sets RequestId field to given value.


### SetRequestIdNil

`func (o *WebhookEvent) SetRequestIdNil(b bool)`

 SetRequestIdNil sets the value for RequestId to be an explicit nil

### UnsetRequestId
`func (o *WebhookEvent) UnsetRequestId()`

UnsetRequestId ensures that no value is present for RequestId, not even an explicit nil
### GetBatchId

`func (o *WebhookEvent) GetBatchId() string`

GetBatchId returns the BatchId field if non-nil, zero value otherwise.

### GetBatchIdOk

`func (o *WebhookEvent) GetBatchIdOk() (*string, bool)`

GetBatchIdOk returns a tuple with the BatchId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBatchId

`func (o *WebhookEvent) SetBatchId(v string)`

SetBatchId sets BatchId field to given value.


### SetBatchIdNil

`func (o *WebhookEvent) SetBatchIdNil(b bool)`

 SetBatchIdNil sets the value for BatchId to be an explicit nil

### UnsetBatchId
`func (o *WebhookEvent) UnsetBatchId()`

UnsetBatchId ensures that no value is present for BatchId, not even an explicit nil
### GetStatus

`func (o *WebhookEvent) GetStatus() int32`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *WebhookEvent) GetStatusOk() (*int32, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *WebhookEvent) SetStatus(v int32)`

SetStatus sets Status field to given value.


### GetHeaders

`func (o *WebhookEvent) GetHeaders() map[string]string`

GetHeaders returns the Headers field if non-nil, zero value otherwise.

### GetHeadersOk

`func (o *WebhookEvent) GetHeadersOk() (*map[string]string, bool)`

GetHeadersOk returns a tuple with the Headers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeaders

`func (o *WebhookEvent) SetHeaders(v map[string]string)`

SetHeaders sets Headers field to given value.


### GetResultUrl

`func (o *WebhookEvent) GetResultUrl() string`

GetResultUrl returns the ResultUrl field if non-nil, zero value otherwise.

### GetResultUrlOk

`func (o *WebhookEvent) GetResultUrlOk() (*string, bool)`

GetResultUrlOk returns a tuple with the ResultUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResultUrl

`func (o *WebhookEvent) SetResultUrl(v string)`

SetResultUrl sets ResultUrl field to given value.


### SetResultUrlNil

`func (o *WebhookEvent) SetResultUrlNil(b bool)`

 SetResultUrlNil sets the value for ResultUrl to be an explicit nil

### UnsetResultUrl
`func (o *WebhookEvent) UnsetResultUrl()`

UnsetResultUrl ensures that no value is present for ResultUrl, not even an explicit nil
### GetResultExpiresAt

`func (o *WebhookEvent) GetResultExpiresAt() int32`

GetResultExpiresAt returns the ResultExpiresAt field if non-nil, zero value otherwise.

### GetResultExpiresAtOk

`func (o *WebhookEvent) GetResultExpiresAtOk() (*int32, bool)`

GetResultExpiresAtOk returns a tuple with the ResultExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResultExpiresAt

`func (o *WebhookEvent) SetResultExpiresAt(v int32)`

SetResultExpiresAt sets ResultExpiresAt field to given value.


### GetBodySize

`func (o *WebhookEvent) GetBodySize() int32`

GetBodySize returns the BodySize field if non-nil, zero value otherwise.

### GetBodySizeOk

`func (o *WebhookEvent) GetBodySizeOk() (*int32, bool)`

GetBodySizeOk returns a tuple with the BodySize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBodySize

`func (o *WebhookEvent) SetBodySize(v int32)`

SetBodySize sets BodySize field to given value.


### SetBodySizeNil

`func (o *WebhookEvent) SetBodySizeNil(b bool)`

 SetBodySizeNil sets the value for BodySize to be an explicit nil

### UnsetBodySize
`func (o *WebhookEvent) UnsetBodySize()`

UnsetBodySize ensures that no value is present for BodySize, not even an explicit nil
### GetBody

`func (o *WebhookEvent) GetBody() interface{}`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *WebhookEvent) GetBodyOk() (*interface{}, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *WebhookEvent) SetBody(v interface{})`

SetBody sets Body field to given value.


### SetBodyNil

`func (o *WebhookEvent) SetBodyNil(b bool)`

 SetBodyNil sets the value for Body to be an explicit nil

### UnsetBody
`func (o *WebhookEvent) UnsetBody()`

UnsetBody ensures that no value is present for Body, not even an explicit nil
### GetBodyOmitted

`func (o *WebhookEvent) GetBodyOmitted() bool`

GetBodyOmitted returns the BodyOmitted field if non-nil, zero value otherwise.

### GetBodyOmittedOk

`func (o *WebhookEvent) GetBodyOmittedOk() (*bool, bool)`

GetBodyOmittedOk returns a tuple with the BodyOmitted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBodyOmitted

`func (o *WebhookEvent) SetBodyOmitted(v bool)`

SetBodyOmitted sets BodyOmitted field to given value.

### HasBodyOmitted

`func (o *WebhookEvent) HasBodyOmitted() bool`

HasBodyOmitted returns a boolean if a field has been set.

### GetAttempt

`func (o *WebhookEvent) GetAttempt() int32`

GetAttempt returns the Attempt field if non-nil, zero value otherwise.

### GetAttemptOk

`func (o *WebhookEvent) GetAttemptOk() (*int32, bool)`

GetAttemptOk returns a tuple with the Attempt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttempt

`func (o *WebhookEvent) SetAttempt(v int32)`

SetAttempt sets Attempt field to given value.


### SetAttemptNil

`func (o *WebhookEvent) SetAttemptNil(b bool)`

 SetAttemptNil sets the value for Attempt to be an explicit nil

### UnsetAttempt
`func (o *WebhookEvent) UnsetAttempt()`

UnsetAttempt ensures that no value is present for Attempt, not even an explicit nil
### GetSentAt

`func (o *WebhookEvent) GetSentAt() int32`

GetSentAt returns the SentAt field if non-nil, zero value otherwise.

### GetSentAtOk

`func (o *WebhookEvent) GetSentAtOk() (*int32, bool)`

GetSentAtOk returns a tuple with the SentAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSentAt

`func (o *WebhookEvent) SetSentAt(v int32)`

SetSentAt sets SentAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



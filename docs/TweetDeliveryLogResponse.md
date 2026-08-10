# TweetDeliveryLogResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**MonitorId** | **string** |  | 
**MonitorName** | **string** |  | 
**TweetId** | **string** |  | 
**AuthorUsername** | **string** |  | 
**TweetTextPreview** | **NullableString** |  | 
**TweetUrl** | **string** |  | 
**TweetPublishedAt** | **time.Time** |  | 
**DetectedAt** | **time.Time** |  | 
**LatencyMs** | **int32** |  | 
**LatencyBadge** | **string** |  | 
**DeliveryStatus** | **string** |  | 
**WebhookStatusCode** | **NullableInt32** |  | 
**WebhookAttempts** | **int32** |  | 

## Methods

### NewTweetDeliveryLogResponse

`func NewTweetDeliveryLogResponse(id string, monitorId string, monitorName string, tweetId string, authorUsername string, tweetTextPreview NullableString, tweetUrl string, tweetPublishedAt time.Time, detectedAt time.Time, latencyMs int32, latencyBadge string, deliveryStatus string, webhookStatusCode NullableInt32, webhookAttempts int32, ) *TweetDeliveryLogResponse`

NewTweetDeliveryLogResponse instantiates a new TweetDeliveryLogResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTweetDeliveryLogResponseWithDefaults

`func NewTweetDeliveryLogResponseWithDefaults() *TweetDeliveryLogResponse`

NewTweetDeliveryLogResponseWithDefaults instantiates a new TweetDeliveryLogResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *TweetDeliveryLogResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *TweetDeliveryLogResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *TweetDeliveryLogResponse) SetId(v string)`

SetId sets Id field to given value.


### GetMonitorId

`func (o *TweetDeliveryLogResponse) GetMonitorId() string`

GetMonitorId returns the MonitorId field if non-nil, zero value otherwise.

### GetMonitorIdOk

`func (o *TweetDeliveryLogResponse) GetMonitorIdOk() (*string, bool)`

GetMonitorIdOk returns a tuple with the MonitorId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMonitorId

`func (o *TweetDeliveryLogResponse) SetMonitorId(v string)`

SetMonitorId sets MonitorId field to given value.


### GetMonitorName

`func (o *TweetDeliveryLogResponse) GetMonitorName() string`

GetMonitorName returns the MonitorName field if non-nil, zero value otherwise.

### GetMonitorNameOk

`func (o *TweetDeliveryLogResponse) GetMonitorNameOk() (*string, bool)`

GetMonitorNameOk returns a tuple with the MonitorName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMonitorName

`func (o *TweetDeliveryLogResponse) SetMonitorName(v string)`

SetMonitorName sets MonitorName field to given value.


### GetTweetId

`func (o *TweetDeliveryLogResponse) GetTweetId() string`

GetTweetId returns the TweetId field if non-nil, zero value otherwise.

### GetTweetIdOk

`func (o *TweetDeliveryLogResponse) GetTweetIdOk() (*string, bool)`

GetTweetIdOk returns a tuple with the TweetId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTweetId

`func (o *TweetDeliveryLogResponse) SetTweetId(v string)`

SetTweetId sets TweetId field to given value.


### GetAuthorUsername

`func (o *TweetDeliveryLogResponse) GetAuthorUsername() string`

GetAuthorUsername returns the AuthorUsername field if non-nil, zero value otherwise.

### GetAuthorUsernameOk

`func (o *TweetDeliveryLogResponse) GetAuthorUsernameOk() (*string, bool)`

GetAuthorUsernameOk returns a tuple with the AuthorUsername field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthorUsername

`func (o *TweetDeliveryLogResponse) SetAuthorUsername(v string)`

SetAuthorUsername sets AuthorUsername field to given value.


### GetTweetTextPreview

`func (o *TweetDeliveryLogResponse) GetTweetTextPreview() string`

GetTweetTextPreview returns the TweetTextPreview field if non-nil, zero value otherwise.

### GetTweetTextPreviewOk

`func (o *TweetDeliveryLogResponse) GetTweetTextPreviewOk() (*string, bool)`

GetTweetTextPreviewOk returns a tuple with the TweetTextPreview field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTweetTextPreview

`func (o *TweetDeliveryLogResponse) SetTweetTextPreview(v string)`

SetTweetTextPreview sets TweetTextPreview field to given value.


### SetTweetTextPreviewNil

`func (o *TweetDeliveryLogResponse) SetTweetTextPreviewNil(b bool)`

 SetTweetTextPreviewNil sets the value for TweetTextPreview to be an explicit nil

### UnsetTweetTextPreview
`func (o *TweetDeliveryLogResponse) UnsetTweetTextPreview()`

UnsetTweetTextPreview ensures that no value is present for TweetTextPreview, not even an explicit nil
### GetTweetUrl

`func (o *TweetDeliveryLogResponse) GetTweetUrl() string`

GetTweetUrl returns the TweetUrl field if non-nil, zero value otherwise.

### GetTweetUrlOk

`func (o *TweetDeliveryLogResponse) GetTweetUrlOk() (*string, bool)`

GetTweetUrlOk returns a tuple with the TweetUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTweetUrl

`func (o *TweetDeliveryLogResponse) SetTweetUrl(v string)`

SetTweetUrl sets TweetUrl field to given value.


### GetTweetPublishedAt

`func (o *TweetDeliveryLogResponse) GetTweetPublishedAt() time.Time`

GetTweetPublishedAt returns the TweetPublishedAt field if non-nil, zero value otherwise.

### GetTweetPublishedAtOk

`func (o *TweetDeliveryLogResponse) GetTweetPublishedAtOk() (*time.Time, bool)`

GetTweetPublishedAtOk returns a tuple with the TweetPublishedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTweetPublishedAt

`func (o *TweetDeliveryLogResponse) SetTweetPublishedAt(v time.Time)`

SetTweetPublishedAt sets TweetPublishedAt field to given value.


### GetDetectedAt

`func (o *TweetDeliveryLogResponse) GetDetectedAt() time.Time`

GetDetectedAt returns the DetectedAt field if non-nil, zero value otherwise.

### GetDetectedAtOk

`func (o *TweetDeliveryLogResponse) GetDetectedAtOk() (*time.Time, bool)`

GetDetectedAtOk returns a tuple with the DetectedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDetectedAt

`func (o *TweetDeliveryLogResponse) SetDetectedAt(v time.Time)`

SetDetectedAt sets DetectedAt field to given value.


### GetLatencyMs

`func (o *TweetDeliveryLogResponse) GetLatencyMs() int32`

GetLatencyMs returns the LatencyMs field if non-nil, zero value otherwise.

### GetLatencyMsOk

`func (o *TweetDeliveryLogResponse) GetLatencyMsOk() (*int32, bool)`

GetLatencyMsOk returns a tuple with the LatencyMs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatencyMs

`func (o *TweetDeliveryLogResponse) SetLatencyMs(v int32)`

SetLatencyMs sets LatencyMs field to given value.


### GetLatencyBadge

`func (o *TweetDeliveryLogResponse) GetLatencyBadge() string`

GetLatencyBadge returns the LatencyBadge field if non-nil, zero value otherwise.

### GetLatencyBadgeOk

`func (o *TweetDeliveryLogResponse) GetLatencyBadgeOk() (*string, bool)`

GetLatencyBadgeOk returns a tuple with the LatencyBadge field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatencyBadge

`func (o *TweetDeliveryLogResponse) SetLatencyBadge(v string)`

SetLatencyBadge sets LatencyBadge field to given value.


### GetDeliveryStatus

`func (o *TweetDeliveryLogResponse) GetDeliveryStatus() string`

GetDeliveryStatus returns the DeliveryStatus field if non-nil, zero value otherwise.

### GetDeliveryStatusOk

`func (o *TweetDeliveryLogResponse) GetDeliveryStatusOk() (*string, bool)`

GetDeliveryStatusOk returns a tuple with the DeliveryStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeliveryStatus

`func (o *TweetDeliveryLogResponse) SetDeliveryStatus(v string)`

SetDeliveryStatus sets DeliveryStatus field to given value.


### GetWebhookStatusCode

`func (o *TweetDeliveryLogResponse) GetWebhookStatusCode() int32`

GetWebhookStatusCode returns the WebhookStatusCode field if non-nil, zero value otherwise.

### GetWebhookStatusCodeOk

`func (o *TweetDeliveryLogResponse) GetWebhookStatusCodeOk() (*int32, bool)`

GetWebhookStatusCodeOk returns a tuple with the WebhookStatusCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookStatusCode

`func (o *TweetDeliveryLogResponse) SetWebhookStatusCode(v int32)`

SetWebhookStatusCode sets WebhookStatusCode field to given value.


### SetWebhookStatusCodeNil

`func (o *TweetDeliveryLogResponse) SetWebhookStatusCodeNil(b bool)`

 SetWebhookStatusCodeNil sets the value for WebhookStatusCode to be an explicit nil

### UnsetWebhookStatusCode
`func (o *TweetDeliveryLogResponse) UnsetWebhookStatusCode()`

UnsetWebhookStatusCode ensures that no value is present for WebhookStatusCode, not even an explicit nil
### GetWebhookAttempts

`func (o *TweetDeliveryLogResponse) GetWebhookAttempts() int32`

GetWebhookAttempts returns the WebhookAttempts field if non-nil, zero value otherwise.

### GetWebhookAttemptsOk

`func (o *TweetDeliveryLogResponse) GetWebhookAttemptsOk() (*int32, bool)`

GetWebhookAttemptsOk returns a tuple with the WebhookAttempts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookAttempts

`func (o *TweetDeliveryLogResponse) SetWebhookAttempts(v int32)`

SetWebhookAttempts sets WebhookAttempts field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



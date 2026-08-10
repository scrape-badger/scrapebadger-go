# FilterRuleDeliveryLogResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**RuleId** | **string** |  | 
**RuleTag** | **string** |  | 
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

### NewFilterRuleDeliveryLogResponse

`func NewFilterRuleDeliveryLogResponse(id string, ruleId string, ruleTag string, tweetId string, authorUsername string, tweetTextPreview NullableString, tweetUrl string, tweetPublishedAt time.Time, detectedAt time.Time, latencyMs int32, latencyBadge string, deliveryStatus string, webhookStatusCode NullableInt32, webhookAttempts int32, ) *FilterRuleDeliveryLogResponse`

NewFilterRuleDeliveryLogResponse instantiates a new FilterRuleDeliveryLogResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFilterRuleDeliveryLogResponseWithDefaults

`func NewFilterRuleDeliveryLogResponseWithDefaults() *FilterRuleDeliveryLogResponse`

NewFilterRuleDeliveryLogResponseWithDefaults instantiates a new FilterRuleDeliveryLogResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *FilterRuleDeliveryLogResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *FilterRuleDeliveryLogResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *FilterRuleDeliveryLogResponse) SetId(v string)`

SetId sets Id field to given value.


### GetRuleId

`func (o *FilterRuleDeliveryLogResponse) GetRuleId() string`

GetRuleId returns the RuleId field if non-nil, zero value otherwise.

### GetRuleIdOk

`func (o *FilterRuleDeliveryLogResponse) GetRuleIdOk() (*string, bool)`

GetRuleIdOk returns a tuple with the RuleId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRuleId

`func (o *FilterRuleDeliveryLogResponse) SetRuleId(v string)`

SetRuleId sets RuleId field to given value.


### GetRuleTag

`func (o *FilterRuleDeliveryLogResponse) GetRuleTag() string`

GetRuleTag returns the RuleTag field if non-nil, zero value otherwise.

### GetRuleTagOk

`func (o *FilterRuleDeliveryLogResponse) GetRuleTagOk() (*string, bool)`

GetRuleTagOk returns a tuple with the RuleTag field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRuleTag

`func (o *FilterRuleDeliveryLogResponse) SetRuleTag(v string)`

SetRuleTag sets RuleTag field to given value.


### GetTweetId

`func (o *FilterRuleDeliveryLogResponse) GetTweetId() string`

GetTweetId returns the TweetId field if non-nil, zero value otherwise.

### GetTweetIdOk

`func (o *FilterRuleDeliveryLogResponse) GetTweetIdOk() (*string, bool)`

GetTweetIdOk returns a tuple with the TweetId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTweetId

`func (o *FilterRuleDeliveryLogResponse) SetTweetId(v string)`

SetTweetId sets TweetId field to given value.


### GetAuthorUsername

`func (o *FilterRuleDeliveryLogResponse) GetAuthorUsername() string`

GetAuthorUsername returns the AuthorUsername field if non-nil, zero value otherwise.

### GetAuthorUsernameOk

`func (o *FilterRuleDeliveryLogResponse) GetAuthorUsernameOk() (*string, bool)`

GetAuthorUsernameOk returns a tuple with the AuthorUsername field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthorUsername

`func (o *FilterRuleDeliveryLogResponse) SetAuthorUsername(v string)`

SetAuthorUsername sets AuthorUsername field to given value.


### GetTweetTextPreview

`func (o *FilterRuleDeliveryLogResponse) GetTweetTextPreview() string`

GetTweetTextPreview returns the TweetTextPreview field if non-nil, zero value otherwise.

### GetTweetTextPreviewOk

`func (o *FilterRuleDeliveryLogResponse) GetTweetTextPreviewOk() (*string, bool)`

GetTweetTextPreviewOk returns a tuple with the TweetTextPreview field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTweetTextPreview

`func (o *FilterRuleDeliveryLogResponse) SetTweetTextPreview(v string)`

SetTweetTextPreview sets TweetTextPreview field to given value.


### SetTweetTextPreviewNil

`func (o *FilterRuleDeliveryLogResponse) SetTweetTextPreviewNil(b bool)`

 SetTweetTextPreviewNil sets the value for TweetTextPreview to be an explicit nil

### UnsetTweetTextPreview
`func (o *FilterRuleDeliveryLogResponse) UnsetTweetTextPreview()`

UnsetTweetTextPreview ensures that no value is present for TweetTextPreview, not even an explicit nil
### GetTweetUrl

`func (o *FilterRuleDeliveryLogResponse) GetTweetUrl() string`

GetTweetUrl returns the TweetUrl field if non-nil, zero value otherwise.

### GetTweetUrlOk

`func (o *FilterRuleDeliveryLogResponse) GetTweetUrlOk() (*string, bool)`

GetTweetUrlOk returns a tuple with the TweetUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTweetUrl

`func (o *FilterRuleDeliveryLogResponse) SetTweetUrl(v string)`

SetTweetUrl sets TweetUrl field to given value.


### GetTweetPublishedAt

`func (o *FilterRuleDeliveryLogResponse) GetTweetPublishedAt() time.Time`

GetTweetPublishedAt returns the TweetPublishedAt field if non-nil, zero value otherwise.

### GetTweetPublishedAtOk

`func (o *FilterRuleDeliveryLogResponse) GetTweetPublishedAtOk() (*time.Time, bool)`

GetTweetPublishedAtOk returns a tuple with the TweetPublishedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTweetPublishedAt

`func (o *FilterRuleDeliveryLogResponse) SetTweetPublishedAt(v time.Time)`

SetTweetPublishedAt sets TweetPublishedAt field to given value.


### GetDetectedAt

`func (o *FilterRuleDeliveryLogResponse) GetDetectedAt() time.Time`

GetDetectedAt returns the DetectedAt field if non-nil, zero value otherwise.

### GetDetectedAtOk

`func (o *FilterRuleDeliveryLogResponse) GetDetectedAtOk() (*time.Time, bool)`

GetDetectedAtOk returns a tuple with the DetectedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDetectedAt

`func (o *FilterRuleDeliveryLogResponse) SetDetectedAt(v time.Time)`

SetDetectedAt sets DetectedAt field to given value.


### GetLatencyMs

`func (o *FilterRuleDeliveryLogResponse) GetLatencyMs() int32`

GetLatencyMs returns the LatencyMs field if non-nil, zero value otherwise.

### GetLatencyMsOk

`func (o *FilterRuleDeliveryLogResponse) GetLatencyMsOk() (*int32, bool)`

GetLatencyMsOk returns a tuple with the LatencyMs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatencyMs

`func (o *FilterRuleDeliveryLogResponse) SetLatencyMs(v int32)`

SetLatencyMs sets LatencyMs field to given value.


### GetLatencyBadge

`func (o *FilterRuleDeliveryLogResponse) GetLatencyBadge() string`

GetLatencyBadge returns the LatencyBadge field if non-nil, zero value otherwise.

### GetLatencyBadgeOk

`func (o *FilterRuleDeliveryLogResponse) GetLatencyBadgeOk() (*string, bool)`

GetLatencyBadgeOk returns a tuple with the LatencyBadge field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatencyBadge

`func (o *FilterRuleDeliveryLogResponse) SetLatencyBadge(v string)`

SetLatencyBadge sets LatencyBadge field to given value.


### GetDeliveryStatus

`func (o *FilterRuleDeliveryLogResponse) GetDeliveryStatus() string`

GetDeliveryStatus returns the DeliveryStatus field if non-nil, zero value otherwise.

### GetDeliveryStatusOk

`func (o *FilterRuleDeliveryLogResponse) GetDeliveryStatusOk() (*string, bool)`

GetDeliveryStatusOk returns a tuple with the DeliveryStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeliveryStatus

`func (o *FilterRuleDeliveryLogResponse) SetDeliveryStatus(v string)`

SetDeliveryStatus sets DeliveryStatus field to given value.


### GetWebhookStatusCode

`func (o *FilterRuleDeliveryLogResponse) GetWebhookStatusCode() int32`

GetWebhookStatusCode returns the WebhookStatusCode field if non-nil, zero value otherwise.

### GetWebhookStatusCodeOk

`func (o *FilterRuleDeliveryLogResponse) GetWebhookStatusCodeOk() (*int32, bool)`

GetWebhookStatusCodeOk returns a tuple with the WebhookStatusCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookStatusCode

`func (o *FilterRuleDeliveryLogResponse) SetWebhookStatusCode(v int32)`

SetWebhookStatusCode sets WebhookStatusCode field to given value.


### SetWebhookStatusCodeNil

`func (o *FilterRuleDeliveryLogResponse) SetWebhookStatusCodeNil(b bool)`

 SetWebhookStatusCodeNil sets the value for WebhookStatusCode to be an explicit nil

### UnsetWebhookStatusCode
`func (o *FilterRuleDeliveryLogResponse) UnsetWebhookStatusCode()`

UnsetWebhookStatusCode ensures that no value is present for WebhookStatusCode, not even an explicit nil
### GetWebhookAttempts

`func (o *FilterRuleDeliveryLogResponse) GetWebhookAttempts() int32`

GetWebhookAttempts returns the WebhookAttempts field if non-nil, zero value otherwise.

### GetWebhookAttemptsOk

`func (o *FilterRuleDeliveryLogResponse) GetWebhookAttemptsOk() (*int32, bool)`

GetWebhookAttemptsOk returns a tuple with the WebhookAttempts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookAttempts

`func (o *FilterRuleDeliveryLogResponse) SetWebhookAttempts(v int32)`

SetWebhookAttempts sets WebhookAttempts field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



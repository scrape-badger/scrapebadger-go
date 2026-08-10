# FilterRuleUpdate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Tag** | Pointer to **NullableString** |  | [optional] 
**Query** | Pointer to **NullableString** |  | [optional] 
**IntervalSeconds** | Pointer to **NullableFloat32** |  | [optional] 
**MaxResultsPerPoll** | Pointer to **NullableInt32** |  | [optional] 
**Status** | Pointer to **NullableString** |  | [optional] 
**WebhookUrl** | Pointer to **NullableString** |  | [optional] 
**WebhookSecret** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewFilterRuleUpdate

`func NewFilterRuleUpdate() *FilterRuleUpdate`

NewFilterRuleUpdate instantiates a new FilterRuleUpdate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFilterRuleUpdateWithDefaults

`func NewFilterRuleUpdateWithDefaults() *FilterRuleUpdate`

NewFilterRuleUpdateWithDefaults instantiates a new FilterRuleUpdate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTag

`func (o *FilterRuleUpdate) GetTag() string`

GetTag returns the Tag field if non-nil, zero value otherwise.

### GetTagOk

`func (o *FilterRuleUpdate) GetTagOk() (*string, bool)`

GetTagOk returns a tuple with the Tag field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTag

`func (o *FilterRuleUpdate) SetTag(v string)`

SetTag sets Tag field to given value.

### HasTag

`func (o *FilterRuleUpdate) HasTag() bool`

HasTag returns a boolean if a field has been set.

### SetTagNil

`func (o *FilterRuleUpdate) SetTagNil(b bool)`

 SetTagNil sets the value for Tag to be an explicit nil

### UnsetTag
`func (o *FilterRuleUpdate) UnsetTag()`

UnsetTag ensures that no value is present for Tag, not even an explicit nil
### GetQuery

`func (o *FilterRuleUpdate) GetQuery() string`

GetQuery returns the Query field if non-nil, zero value otherwise.

### GetQueryOk

`func (o *FilterRuleUpdate) GetQueryOk() (*string, bool)`

GetQueryOk returns a tuple with the Query field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuery

`func (o *FilterRuleUpdate) SetQuery(v string)`

SetQuery sets Query field to given value.

### HasQuery

`func (o *FilterRuleUpdate) HasQuery() bool`

HasQuery returns a boolean if a field has been set.

### SetQueryNil

`func (o *FilterRuleUpdate) SetQueryNil(b bool)`

 SetQueryNil sets the value for Query to be an explicit nil

### UnsetQuery
`func (o *FilterRuleUpdate) UnsetQuery()`

UnsetQuery ensures that no value is present for Query, not even an explicit nil
### GetIntervalSeconds

`func (o *FilterRuleUpdate) GetIntervalSeconds() float32`

GetIntervalSeconds returns the IntervalSeconds field if non-nil, zero value otherwise.

### GetIntervalSecondsOk

`func (o *FilterRuleUpdate) GetIntervalSecondsOk() (*float32, bool)`

GetIntervalSecondsOk returns a tuple with the IntervalSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntervalSeconds

`func (o *FilterRuleUpdate) SetIntervalSeconds(v float32)`

SetIntervalSeconds sets IntervalSeconds field to given value.

### HasIntervalSeconds

`func (o *FilterRuleUpdate) HasIntervalSeconds() bool`

HasIntervalSeconds returns a boolean if a field has been set.

### SetIntervalSecondsNil

`func (o *FilterRuleUpdate) SetIntervalSecondsNil(b bool)`

 SetIntervalSecondsNil sets the value for IntervalSeconds to be an explicit nil

### UnsetIntervalSeconds
`func (o *FilterRuleUpdate) UnsetIntervalSeconds()`

UnsetIntervalSeconds ensures that no value is present for IntervalSeconds, not even an explicit nil
### GetMaxResultsPerPoll

`func (o *FilterRuleUpdate) GetMaxResultsPerPoll() int32`

GetMaxResultsPerPoll returns the MaxResultsPerPoll field if non-nil, zero value otherwise.

### GetMaxResultsPerPollOk

`func (o *FilterRuleUpdate) GetMaxResultsPerPollOk() (*int32, bool)`

GetMaxResultsPerPollOk returns a tuple with the MaxResultsPerPoll field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxResultsPerPoll

`func (o *FilterRuleUpdate) SetMaxResultsPerPoll(v int32)`

SetMaxResultsPerPoll sets MaxResultsPerPoll field to given value.

### HasMaxResultsPerPoll

`func (o *FilterRuleUpdate) HasMaxResultsPerPoll() bool`

HasMaxResultsPerPoll returns a boolean if a field has been set.

### SetMaxResultsPerPollNil

`func (o *FilterRuleUpdate) SetMaxResultsPerPollNil(b bool)`

 SetMaxResultsPerPollNil sets the value for MaxResultsPerPoll to be an explicit nil

### UnsetMaxResultsPerPoll
`func (o *FilterRuleUpdate) UnsetMaxResultsPerPoll()`

UnsetMaxResultsPerPoll ensures that no value is present for MaxResultsPerPoll, not even an explicit nil
### GetStatus

`func (o *FilterRuleUpdate) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *FilterRuleUpdate) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *FilterRuleUpdate) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *FilterRuleUpdate) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### SetStatusNil

`func (o *FilterRuleUpdate) SetStatusNil(b bool)`

 SetStatusNil sets the value for Status to be an explicit nil

### UnsetStatus
`func (o *FilterRuleUpdate) UnsetStatus()`

UnsetStatus ensures that no value is present for Status, not even an explicit nil
### GetWebhookUrl

`func (o *FilterRuleUpdate) GetWebhookUrl() string`

GetWebhookUrl returns the WebhookUrl field if non-nil, zero value otherwise.

### GetWebhookUrlOk

`func (o *FilterRuleUpdate) GetWebhookUrlOk() (*string, bool)`

GetWebhookUrlOk returns a tuple with the WebhookUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookUrl

`func (o *FilterRuleUpdate) SetWebhookUrl(v string)`

SetWebhookUrl sets WebhookUrl field to given value.

### HasWebhookUrl

`func (o *FilterRuleUpdate) HasWebhookUrl() bool`

HasWebhookUrl returns a boolean if a field has been set.

### SetWebhookUrlNil

`func (o *FilterRuleUpdate) SetWebhookUrlNil(b bool)`

 SetWebhookUrlNil sets the value for WebhookUrl to be an explicit nil

### UnsetWebhookUrl
`func (o *FilterRuleUpdate) UnsetWebhookUrl()`

UnsetWebhookUrl ensures that no value is present for WebhookUrl, not even an explicit nil
### GetWebhookSecret

`func (o *FilterRuleUpdate) GetWebhookSecret() string`

GetWebhookSecret returns the WebhookSecret field if non-nil, zero value otherwise.

### GetWebhookSecretOk

`func (o *FilterRuleUpdate) GetWebhookSecretOk() (*string, bool)`

GetWebhookSecretOk returns a tuple with the WebhookSecret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookSecret

`func (o *FilterRuleUpdate) SetWebhookSecret(v string)`

SetWebhookSecret sets WebhookSecret field to given value.

### HasWebhookSecret

`func (o *FilterRuleUpdate) HasWebhookSecret() bool`

HasWebhookSecret returns a boolean if a field has been set.

### SetWebhookSecretNil

`func (o *FilterRuleUpdate) SetWebhookSecretNil(b bool)`

 SetWebhookSecretNil sets the value for WebhookSecret to be an explicit nil

### UnsetWebhookSecret
`func (o *FilterRuleUpdate) UnsetWebhookSecret()`

UnsetWebhookSecret ensures that no value is present for WebhookSecret, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



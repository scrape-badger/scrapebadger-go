# FilterRuleCreate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Tag** | **string** |  | 
**Query** | **string** |  | 
**IntervalSeconds** | **float32** |  | 
**MaxResultsPerPoll** | Pointer to **int32** |  | [optional] [default to 20]
**WebhookUrl** | Pointer to **NullableString** |  | [optional] 
**WebhookSecret** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewFilterRuleCreate

`func NewFilterRuleCreate(tag string, query string, intervalSeconds float32, ) *FilterRuleCreate`

NewFilterRuleCreate instantiates a new FilterRuleCreate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFilterRuleCreateWithDefaults

`func NewFilterRuleCreateWithDefaults() *FilterRuleCreate`

NewFilterRuleCreateWithDefaults instantiates a new FilterRuleCreate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTag

`func (o *FilterRuleCreate) GetTag() string`

GetTag returns the Tag field if non-nil, zero value otherwise.

### GetTagOk

`func (o *FilterRuleCreate) GetTagOk() (*string, bool)`

GetTagOk returns a tuple with the Tag field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTag

`func (o *FilterRuleCreate) SetTag(v string)`

SetTag sets Tag field to given value.


### GetQuery

`func (o *FilterRuleCreate) GetQuery() string`

GetQuery returns the Query field if non-nil, zero value otherwise.

### GetQueryOk

`func (o *FilterRuleCreate) GetQueryOk() (*string, bool)`

GetQueryOk returns a tuple with the Query field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuery

`func (o *FilterRuleCreate) SetQuery(v string)`

SetQuery sets Query field to given value.


### GetIntervalSeconds

`func (o *FilterRuleCreate) GetIntervalSeconds() float32`

GetIntervalSeconds returns the IntervalSeconds field if non-nil, zero value otherwise.

### GetIntervalSecondsOk

`func (o *FilterRuleCreate) GetIntervalSecondsOk() (*float32, bool)`

GetIntervalSecondsOk returns a tuple with the IntervalSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntervalSeconds

`func (o *FilterRuleCreate) SetIntervalSeconds(v float32)`

SetIntervalSeconds sets IntervalSeconds field to given value.


### GetMaxResultsPerPoll

`func (o *FilterRuleCreate) GetMaxResultsPerPoll() int32`

GetMaxResultsPerPoll returns the MaxResultsPerPoll field if non-nil, zero value otherwise.

### GetMaxResultsPerPollOk

`func (o *FilterRuleCreate) GetMaxResultsPerPollOk() (*int32, bool)`

GetMaxResultsPerPollOk returns a tuple with the MaxResultsPerPoll field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxResultsPerPoll

`func (o *FilterRuleCreate) SetMaxResultsPerPoll(v int32)`

SetMaxResultsPerPoll sets MaxResultsPerPoll field to given value.

### HasMaxResultsPerPoll

`func (o *FilterRuleCreate) HasMaxResultsPerPoll() bool`

HasMaxResultsPerPoll returns a boolean if a field has been set.

### GetWebhookUrl

`func (o *FilterRuleCreate) GetWebhookUrl() string`

GetWebhookUrl returns the WebhookUrl field if non-nil, zero value otherwise.

### GetWebhookUrlOk

`func (o *FilterRuleCreate) GetWebhookUrlOk() (*string, bool)`

GetWebhookUrlOk returns a tuple with the WebhookUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookUrl

`func (o *FilterRuleCreate) SetWebhookUrl(v string)`

SetWebhookUrl sets WebhookUrl field to given value.

### HasWebhookUrl

`func (o *FilterRuleCreate) HasWebhookUrl() bool`

HasWebhookUrl returns a boolean if a field has been set.

### SetWebhookUrlNil

`func (o *FilterRuleCreate) SetWebhookUrlNil(b bool)`

 SetWebhookUrlNil sets the value for WebhookUrl to be an explicit nil

### UnsetWebhookUrl
`func (o *FilterRuleCreate) UnsetWebhookUrl()`

UnsetWebhookUrl ensures that no value is present for WebhookUrl, not even an explicit nil
### GetWebhookSecret

`func (o *FilterRuleCreate) GetWebhookSecret() string`

GetWebhookSecret returns the WebhookSecret field if non-nil, zero value otherwise.

### GetWebhookSecretOk

`func (o *FilterRuleCreate) GetWebhookSecretOk() (*string, bool)`

GetWebhookSecretOk returns a tuple with the WebhookSecret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookSecret

`func (o *FilterRuleCreate) SetWebhookSecret(v string)`

SetWebhookSecret sets WebhookSecret field to given value.

### HasWebhookSecret

`func (o *FilterRuleCreate) HasWebhookSecret() bool`

HasWebhookSecret returns a boolean if a field has been set.

### SetWebhookSecretNil

`func (o *FilterRuleCreate) SetWebhookSecretNil(b bool)`

 SetWebhookSecretNil sets the value for WebhookSecret to be an explicit nil

### UnsetWebhookSecret
`func (o *FilterRuleCreate) UnsetWebhookSecret()`

UnsetWebhookSecret ensures that no value is present for WebhookSecret, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



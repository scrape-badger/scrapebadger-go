# FilterRuleResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Tag** | **string** |  | 
**Query** | **string** |  | 
**IntervalSeconds** | **float32** |  | 
**MaxResultsPerPoll** | **int32** |  | 
**Status** | **string** |  | 
**StatusReason** | **NullableString** |  | 
**WebhookUrl** | **NullableString** |  | 
**WebhookSecretSet** | **bool** |  | 
**TotalCreditsBurned** | **float32** |  | 
**CreatedAt** | **time.Time** |  | 
**UpdatedAt** | **time.Time** |  | 

## Methods

### NewFilterRuleResponse

`func NewFilterRuleResponse(id string, tag string, query string, intervalSeconds float32, maxResultsPerPoll int32, status string, statusReason NullableString, webhookUrl NullableString, webhookSecretSet bool, totalCreditsBurned float32, createdAt time.Time, updatedAt time.Time, ) *FilterRuleResponse`

NewFilterRuleResponse instantiates a new FilterRuleResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFilterRuleResponseWithDefaults

`func NewFilterRuleResponseWithDefaults() *FilterRuleResponse`

NewFilterRuleResponseWithDefaults instantiates a new FilterRuleResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *FilterRuleResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *FilterRuleResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *FilterRuleResponse) SetId(v string)`

SetId sets Id field to given value.


### GetTag

`func (o *FilterRuleResponse) GetTag() string`

GetTag returns the Tag field if non-nil, zero value otherwise.

### GetTagOk

`func (o *FilterRuleResponse) GetTagOk() (*string, bool)`

GetTagOk returns a tuple with the Tag field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTag

`func (o *FilterRuleResponse) SetTag(v string)`

SetTag sets Tag field to given value.


### GetQuery

`func (o *FilterRuleResponse) GetQuery() string`

GetQuery returns the Query field if non-nil, zero value otherwise.

### GetQueryOk

`func (o *FilterRuleResponse) GetQueryOk() (*string, bool)`

GetQueryOk returns a tuple with the Query field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuery

`func (o *FilterRuleResponse) SetQuery(v string)`

SetQuery sets Query field to given value.


### GetIntervalSeconds

`func (o *FilterRuleResponse) GetIntervalSeconds() float32`

GetIntervalSeconds returns the IntervalSeconds field if non-nil, zero value otherwise.

### GetIntervalSecondsOk

`func (o *FilterRuleResponse) GetIntervalSecondsOk() (*float32, bool)`

GetIntervalSecondsOk returns a tuple with the IntervalSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntervalSeconds

`func (o *FilterRuleResponse) SetIntervalSeconds(v float32)`

SetIntervalSeconds sets IntervalSeconds field to given value.


### GetMaxResultsPerPoll

`func (o *FilterRuleResponse) GetMaxResultsPerPoll() int32`

GetMaxResultsPerPoll returns the MaxResultsPerPoll field if non-nil, zero value otherwise.

### GetMaxResultsPerPollOk

`func (o *FilterRuleResponse) GetMaxResultsPerPollOk() (*int32, bool)`

GetMaxResultsPerPollOk returns a tuple with the MaxResultsPerPoll field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxResultsPerPoll

`func (o *FilterRuleResponse) SetMaxResultsPerPoll(v int32)`

SetMaxResultsPerPoll sets MaxResultsPerPoll field to given value.


### GetStatus

`func (o *FilterRuleResponse) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *FilterRuleResponse) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *FilterRuleResponse) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetStatusReason

`func (o *FilterRuleResponse) GetStatusReason() string`

GetStatusReason returns the StatusReason field if non-nil, zero value otherwise.

### GetStatusReasonOk

`func (o *FilterRuleResponse) GetStatusReasonOk() (*string, bool)`

GetStatusReasonOk returns a tuple with the StatusReason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusReason

`func (o *FilterRuleResponse) SetStatusReason(v string)`

SetStatusReason sets StatusReason field to given value.


### SetStatusReasonNil

`func (o *FilterRuleResponse) SetStatusReasonNil(b bool)`

 SetStatusReasonNil sets the value for StatusReason to be an explicit nil

### UnsetStatusReason
`func (o *FilterRuleResponse) UnsetStatusReason()`

UnsetStatusReason ensures that no value is present for StatusReason, not even an explicit nil
### GetWebhookUrl

`func (o *FilterRuleResponse) GetWebhookUrl() string`

GetWebhookUrl returns the WebhookUrl field if non-nil, zero value otherwise.

### GetWebhookUrlOk

`func (o *FilterRuleResponse) GetWebhookUrlOk() (*string, bool)`

GetWebhookUrlOk returns a tuple with the WebhookUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookUrl

`func (o *FilterRuleResponse) SetWebhookUrl(v string)`

SetWebhookUrl sets WebhookUrl field to given value.


### SetWebhookUrlNil

`func (o *FilterRuleResponse) SetWebhookUrlNil(b bool)`

 SetWebhookUrlNil sets the value for WebhookUrl to be an explicit nil

### UnsetWebhookUrl
`func (o *FilterRuleResponse) UnsetWebhookUrl()`

UnsetWebhookUrl ensures that no value is present for WebhookUrl, not even an explicit nil
### GetWebhookSecretSet

`func (o *FilterRuleResponse) GetWebhookSecretSet() bool`

GetWebhookSecretSet returns the WebhookSecretSet field if non-nil, zero value otherwise.

### GetWebhookSecretSetOk

`func (o *FilterRuleResponse) GetWebhookSecretSetOk() (*bool, bool)`

GetWebhookSecretSetOk returns a tuple with the WebhookSecretSet field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookSecretSet

`func (o *FilterRuleResponse) SetWebhookSecretSet(v bool)`

SetWebhookSecretSet sets WebhookSecretSet field to given value.


### GetTotalCreditsBurned

`func (o *FilterRuleResponse) GetTotalCreditsBurned() float32`

GetTotalCreditsBurned returns the TotalCreditsBurned field if non-nil, zero value otherwise.

### GetTotalCreditsBurnedOk

`func (o *FilterRuleResponse) GetTotalCreditsBurnedOk() (*float32, bool)`

GetTotalCreditsBurnedOk returns a tuple with the TotalCreditsBurned field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalCreditsBurned

`func (o *FilterRuleResponse) SetTotalCreditsBurned(v float32)`

SetTotalCreditsBurned sets TotalCreditsBurned field to given value.


### GetCreatedAt

`func (o *FilterRuleResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *FilterRuleResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *FilterRuleResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *FilterRuleResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *FilterRuleResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *FilterRuleResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



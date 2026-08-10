# StreamMonitorResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Name** | **string** |  | 
**Usernames** | **[]string** |  | 
**Status** | **string** |  | 
**StatusReason** | **NullableString** |  | 
**WebhookUrl** | **NullableString** |  | 
**WebhookSecretSet** | **bool** |  | 
**FilterTypes** | **[]string** |  | 
**CreditsPerAccountPerDay** | **float32** |  | 
**EstimatedCreditsPerDay** | **float32** |  | 
**PricingTier** | **string** |  | 
**CreatedAt** | **time.Time** |  | 
**UpdatedAt** | **time.Time** |  | 

## Methods

### NewStreamMonitorResponse

`func NewStreamMonitorResponse(id string, name string, usernames []string, status string, statusReason NullableString, webhookUrl NullableString, webhookSecretSet bool, filterTypes []string, creditsPerAccountPerDay float32, estimatedCreditsPerDay float32, pricingTier string, createdAt time.Time, updatedAt time.Time, ) *StreamMonitorResponse`

NewStreamMonitorResponse instantiates a new StreamMonitorResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStreamMonitorResponseWithDefaults

`func NewStreamMonitorResponseWithDefaults() *StreamMonitorResponse`

NewStreamMonitorResponseWithDefaults instantiates a new StreamMonitorResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *StreamMonitorResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *StreamMonitorResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *StreamMonitorResponse) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *StreamMonitorResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *StreamMonitorResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *StreamMonitorResponse) SetName(v string)`

SetName sets Name field to given value.


### GetUsernames

`func (o *StreamMonitorResponse) GetUsernames() []string`

GetUsernames returns the Usernames field if non-nil, zero value otherwise.

### GetUsernamesOk

`func (o *StreamMonitorResponse) GetUsernamesOk() (*[]string, bool)`

GetUsernamesOk returns a tuple with the Usernames field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsernames

`func (o *StreamMonitorResponse) SetUsernames(v []string)`

SetUsernames sets Usernames field to given value.


### GetStatus

`func (o *StreamMonitorResponse) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *StreamMonitorResponse) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *StreamMonitorResponse) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetStatusReason

`func (o *StreamMonitorResponse) GetStatusReason() string`

GetStatusReason returns the StatusReason field if non-nil, zero value otherwise.

### GetStatusReasonOk

`func (o *StreamMonitorResponse) GetStatusReasonOk() (*string, bool)`

GetStatusReasonOk returns a tuple with the StatusReason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusReason

`func (o *StreamMonitorResponse) SetStatusReason(v string)`

SetStatusReason sets StatusReason field to given value.


### SetStatusReasonNil

`func (o *StreamMonitorResponse) SetStatusReasonNil(b bool)`

 SetStatusReasonNil sets the value for StatusReason to be an explicit nil

### UnsetStatusReason
`func (o *StreamMonitorResponse) UnsetStatusReason()`

UnsetStatusReason ensures that no value is present for StatusReason, not even an explicit nil
### GetWebhookUrl

`func (o *StreamMonitorResponse) GetWebhookUrl() string`

GetWebhookUrl returns the WebhookUrl field if non-nil, zero value otherwise.

### GetWebhookUrlOk

`func (o *StreamMonitorResponse) GetWebhookUrlOk() (*string, bool)`

GetWebhookUrlOk returns a tuple with the WebhookUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookUrl

`func (o *StreamMonitorResponse) SetWebhookUrl(v string)`

SetWebhookUrl sets WebhookUrl field to given value.


### SetWebhookUrlNil

`func (o *StreamMonitorResponse) SetWebhookUrlNil(b bool)`

 SetWebhookUrlNil sets the value for WebhookUrl to be an explicit nil

### UnsetWebhookUrl
`func (o *StreamMonitorResponse) UnsetWebhookUrl()`

UnsetWebhookUrl ensures that no value is present for WebhookUrl, not even an explicit nil
### GetWebhookSecretSet

`func (o *StreamMonitorResponse) GetWebhookSecretSet() bool`

GetWebhookSecretSet returns the WebhookSecretSet field if non-nil, zero value otherwise.

### GetWebhookSecretSetOk

`func (o *StreamMonitorResponse) GetWebhookSecretSetOk() (*bool, bool)`

GetWebhookSecretSetOk returns a tuple with the WebhookSecretSet field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookSecretSet

`func (o *StreamMonitorResponse) SetWebhookSecretSet(v bool)`

SetWebhookSecretSet sets WebhookSecretSet field to given value.


### GetFilterTypes

`func (o *StreamMonitorResponse) GetFilterTypes() []string`

GetFilterTypes returns the FilterTypes field if non-nil, zero value otherwise.

### GetFilterTypesOk

`func (o *StreamMonitorResponse) GetFilterTypesOk() (*[]string, bool)`

GetFilterTypesOk returns a tuple with the FilterTypes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilterTypes

`func (o *StreamMonitorResponse) SetFilterTypes(v []string)`

SetFilterTypes sets FilterTypes field to given value.


### SetFilterTypesNil

`func (o *StreamMonitorResponse) SetFilterTypesNil(b bool)`

 SetFilterTypesNil sets the value for FilterTypes to be an explicit nil

### UnsetFilterTypes
`func (o *StreamMonitorResponse) UnsetFilterTypes()`

UnsetFilterTypes ensures that no value is present for FilterTypes, not even an explicit nil
### GetCreditsPerAccountPerDay

`func (o *StreamMonitorResponse) GetCreditsPerAccountPerDay() float32`

GetCreditsPerAccountPerDay returns the CreditsPerAccountPerDay field if non-nil, zero value otherwise.

### GetCreditsPerAccountPerDayOk

`func (o *StreamMonitorResponse) GetCreditsPerAccountPerDayOk() (*float32, bool)`

GetCreditsPerAccountPerDayOk returns a tuple with the CreditsPerAccountPerDay field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreditsPerAccountPerDay

`func (o *StreamMonitorResponse) SetCreditsPerAccountPerDay(v float32)`

SetCreditsPerAccountPerDay sets CreditsPerAccountPerDay field to given value.


### GetEstimatedCreditsPerDay

`func (o *StreamMonitorResponse) GetEstimatedCreditsPerDay() float32`

GetEstimatedCreditsPerDay returns the EstimatedCreditsPerDay field if non-nil, zero value otherwise.

### GetEstimatedCreditsPerDayOk

`func (o *StreamMonitorResponse) GetEstimatedCreditsPerDayOk() (*float32, bool)`

GetEstimatedCreditsPerDayOk returns a tuple with the EstimatedCreditsPerDay field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEstimatedCreditsPerDay

`func (o *StreamMonitorResponse) SetEstimatedCreditsPerDay(v float32)`

SetEstimatedCreditsPerDay sets EstimatedCreditsPerDay field to given value.


### GetPricingTier

`func (o *StreamMonitorResponse) GetPricingTier() string`

GetPricingTier returns the PricingTier field if non-nil, zero value otherwise.

### GetPricingTierOk

`func (o *StreamMonitorResponse) GetPricingTierOk() (*string, bool)`

GetPricingTierOk returns a tuple with the PricingTier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPricingTier

`func (o *StreamMonitorResponse) SetPricingTier(v string)`

SetPricingTier sets PricingTier field to given value.


### GetCreatedAt

`func (o *StreamMonitorResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *StreamMonitorResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *StreamMonitorResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *StreamMonitorResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *StreamMonitorResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *StreamMonitorResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



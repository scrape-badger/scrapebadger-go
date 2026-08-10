# AccountInfo

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CreditsBalance** | **int32** |  | 
**SubscriptionCreditsBalance** | **int32** |  | 
**TotalCreditsBalance** | **int32** |  | 
**Tier** | **NullableString** |  | 
**RateLimitPerMinute** | **NullableInt32** |  | 
**Subscription** | Pointer to [**NullableSubscriptionInfo**](SubscriptionInfo.md) |  | [optional] 

## Methods

### NewAccountInfo

`func NewAccountInfo(creditsBalance int32, subscriptionCreditsBalance int32, totalCreditsBalance int32, tier NullableString, rateLimitPerMinute NullableInt32, ) *AccountInfo`

NewAccountInfo instantiates a new AccountInfo object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAccountInfoWithDefaults

`func NewAccountInfoWithDefaults() *AccountInfo`

NewAccountInfoWithDefaults instantiates a new AccountInfo object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCreditsBalance

`func (o *AccountInfo) GetCreditsBalance() int32`

GetCreditsBalance returns the CreditsBalance field if non-nil, zero value otherwise.

### GetCreditsBalanceOk

`func (o *AccountInfo) GetCreditsBalanceOk() (*int32, bool)`

GetCreditsBalanceOk returns a tuple with the CreditsBalance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreditsBalance

`func (o *AccountInfo) SetCreditsBalance(v int32)`

SetCreditsBalance sets CreditsBalance field to given value.


### GetSubscriptionCreditsBalance

`func (o *AccountInfo) GetSubscriptionCreditsBalance() int32`

GetSubscriptionCreditsBalance returns the SubscriptionCreditsBalance field if non-nil, zero value otherwise.

### GetSubscriptionCreditsBalanceOk

`func (o *AccountInfo) GetSubscriptionCreditsBalanceOk() (*int32, bool)`

GetSubscriptionCreditsBalanceOk returns a tuple with the SubscriptionCreditsBalance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubscriptionCreditsBalance

`func (o *AccountInfo) SetSubscriptionCreditsBalance(v int32)`

SetSubscriptionCreditsBalance sets SubscriptionCreditsBalance field to given value.


### GetTotalCreditsBalance

`func (o *AccountInfo) GetTotalCreditsBalance() int32`

GetTotalCreditsBalance returns the TotalCreditsBalance field if non-nil, zero value otherwise.

### GetTotalCreditsBalanceOk

`func (o *AccountInfo) GetTotalCreditsBalanceOk() (*int32, bool)`

GetTotalCreditsBalanceOk returns a tuple with the TotalCreditsBalance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalCreditsBalance

`func (o *AccountInfo) SetTotalCreditsBalance(v int32)`

SetTotalCreditsBalance sets TotalCreditsBalance field to given value.


### GetTier

`func (o *AccountInfo) GetTier() string`

GetTier returns the Tier field if non-nil, zero value otherwise.

### GetTierOk

`func (o *AccountInfo) GetTierOk() (*string, bool)`

GetTierOk returns a tuple with the Tier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTier

`func (o *AccountInfo) SetTier(v string)`

SetTier sets Tier field to given value.


### SetTierNil

`func (o *AccountInfo) SetTierNil(b bool)`

 SetTierNil sets the value for Tier to be an explicit nil

### UnsetTier
`func (o *AccountInfo) UnsetTier()`

UnsetTier ensures that no value is present for Tier, not even an explicit nil
### GetRateLimitPerMinute

`func (o *AccountInfo) GetRateLimitPerMinute() int32`

GetRateLimitPerMinute returns the RateLimitPerMinute field if non-nil, zero value otherwise.

### GetRateLimitPerMinuteOk

`func (o *AccountInfo) GetRateLimitPerMinuteOk() (*int32, bool)`

GetRateLimitPerMinuteOk returns a tuple with the RateLimitPerMinute field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRateLimitPerMinute

`func (o *AccountInfo) SetRateLimitPerMinute(v int32)`

SetRateLimitPerMinute sets RateLimitPerMinute field to given value.


### SetRateLimitPerMinuteNil

`func (o *AccountInfo) SetRateLimitPerMinuteNil(b bool)`

 SetRateLimitPerMinuteNil sets the value for RateLimitPerMinute to be an explicit nil

### UnsetRateLimitPerMinute
`func (o *AccountInfo) UnsetRateLimitPerMinute()`

UnsetRateLimitPerMinute ensures that no value is present for RateLimitPerMinute, not even an explicit nil
### GetSubscription

`func (o *AccountInfo) GetSubscription() SubscriptionInfo`

GetSubscription returns the Subscription field if non-nil, zero value otherwise.

### GetSubscriptionOk

`func (o *AccountInfo) GetSubscriptionOk() (*SubscriptionInfo, bool)`

GetSubscriptionOk returns a tuple with the Subscription field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubscription

`func (o *AccountInfo) SetSubscription(v SubscriptionInfo)`

SetSubscription sets Subscription field to given value.

### HasSubscription

`func (o *AccountInfo) HasSubscription() bool`

HasSubscription returns a boolean if a field has been set.

### SetSubscriptionNil

`func (o *AccountInfo) SetSubscriptionNil(b bool)`

 SetSubscriptionNil sets the value for Subscription to be an explicit nil

### UnsetSubscription
`func (o *AccountInfo) UnsetSubscription()`

UnsetSubscription ensures that no value is present for Subscription, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



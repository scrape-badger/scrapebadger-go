# SubscriptionInfo

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PlanCode** | **string** |  | 
**PlanTitle** | **string** |  | 
**BillingCadence** | **string** |  | 
**Status** | **string** |  | 
**CurrentPeriodStart** | Pointer to **NullableTime** |  | [optional] 
**CurrentPeriodEnd** | Pointer to **NullableTime** |  | [optional] 
**CancelAtPeriodEnd** | Pointer to **bool** |  | [optional] [default to false]
**CancelEffectiveAt** | Pointer to **NullableTime** |  | [optional] 
**MonthlyCredits** | Pointer to **int32** |  | [optional] [default to 0]
**PendingPlanCode** | Pointer to **NullableString** |  | [optional] 
**PendingPlanTitle** | Pointer to **NullableString** |  | [optional] 
**PendingChangeEffectiveAt** | Pointer to **NullableTime** |  | [optional] 

## Methods

### NewSubscriptionInfo

`func NewSubscriptionInfo(planCode string, planTitle string, billingCadence string, status string, ) *SubscriptionInfo`

NewSubscriptionInfo instantiates a new SubscriptionInfo object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSubscriptionInfoWithDefaults

`func NewSubscriptionInfoWithDefaults() *SubscriptionInfo`

NewSubscriptionInfoWithDefaults instantiates a new SubscriptionInfo object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPlanCode

`func (o *SubscriptionInfo) GetPlanCode() string`

GetPlanCode returns the PlanCode field if non-nil, zero value otherwise.

### GetPlanCodeOk

`func (o *SubscriptionInfo) GetPlanCodeOk() (*string, bool)`

GetPlanCodeOk returns a tuple with the PlanCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlanCode

`func (o *SubscriptionInfo) SetPlanCode(v string)`

SetPlanCode sets PlanCode field to given value.


### GetPlanTitle

`func (o *SubscriptionInfo) GetPlanTitle() string`

GetPlanTitle returns the PlanTitle field if non-nil, zero value otherwise.

### GetPlanTitleOk

`func (o *SubscriptionInfo) GetPlanTitleOk() (*string, bool)`

GetPlanTitleOk returns a tuple with the PlanTitle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlanTitle

`func (o *SubscriptionInfo) SetPlanTitle(v string)`

SetPlanTitle sets PlanTitle field to given value.


### GetBillingCadence

`func (o *SubscriptionInfo) GetBillingCadence() string`

GetBillingCadence returns the BillingCadence field if non-nil, zero value otherwise.

### GetBillingCadenceOk

`func (o *SubscriptionInfo) GetBillingCadenceOk() (*string, bool)`

GetBillingCadenceOk returns a tuple with the BillingCadence field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBillingCadence

`func (o *SubscriptionInfo) SetBillingCadence(v string)`

SetBillingCadence sets BillingCadence field to given value.


### GetStatus

`func (o *SubscriptionInfo) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *SubscriptionInfo) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *SubscriptionInfo) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetCurrentPeriodStart

`func (o *SubscriptionInfo) GetCurrentPeriodStart() time.Time`

GetCurrentPeriodStart returns the CurrentPeriodStart field if non-nil, zero value otherwise.

### GetCurrentPeriodStartOk

`func (o *SubscriptionInfo) GetCurrentPeriodStartOk() (*time.Time, bool)`

GetCurrentPeriodStartOk returns a tuple with the CurrentPeriodStart field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrentPeriodStart

`func (o *SubscriptionInfo) SetCurrentPeriodStart(v time.Time)`

SetCurrentPeriodStart sets CurrentPeriodStart field to given value.

### HasCurrentPeriodStart

`func (o *SubscriptionInfo) HasCurrentPeriodStart() bool`

HasCurrentPeriodStart returns a boolean if a field has been set.

### SetCurrentPeriodStartNil

`func (o *SubscriptionInfo) SetCurrentPeriodStartNil(b bool)`

 SetCurrentPeriodStartNil sets the value for CurrentPeriodStart to be an explicit nil

### UnsetCurrentPeriodStart
`func (o *SubscriptionInfo) UnsetCurrentPeriodStart()`

UnsetCurrentPeriodStart ensures that no value is present for CurrentPeriodStart, not even an explicit nil
### GetCurrentPeriodEnd

`func (o *SubscriptionInfo) GetCurrentPeriodEnd() time.Time`

GetCurrentPeriodEnd returns the CurrentPeriodEnd field if non-nil, zero value otherwise.

### GetCurrentPeriodEndOk

`func (o *SubscriptionInfo) GetCurrentPeriodEndOk() (*time.Time, bool)`

GetCurrentPeriodEndOk returns a tuple with the CurrentPeriodEnd field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrentPeriodEnd

`func (o *SubscriptionInfo) SetCurrentPeriodEnd(v time.Time)`

SetCurrentPeriodEnd sets CurrentPeriodEnd field to given value.

### HasCurrentPeriodEnd

`func (o *SubscriptionInfo) HasCurrentPeriodEnd() bool`

HasCurrentPeriodEnd returns a boolean if a field has been set.

### SetCurrentPeriodEndNil

`func (o *SubscriptionInfo) SetCurrentPeriodEndNil(b bool)`

 SetCurrentPeriodEndNil sets the value for CurrentPeriodEnd to be an explicit nil

### UnsetCurrentPeriodEnd
`func (o *SubscriptionInfo) UnsetCurrentPeriodEnd()`

UnsetCurrentPeriodEnd ensures that no value is present for CurrentPeriodEnd, not even an explicit nil
### GetCancelAtPeriodEnd

`func (o *SubscriptionInfo) GetCancelAtPeriodEnd() bool`

GetCancelAtPeriodEnd returns the CancelAtPeriodEnd field if non-nil, zero value otherwise.

### GetCancelAtPeriodEndOk

`func (o *SubscriptionInfo) GetCancelAtPeriodEndOk() (*bool, bool)`

GetCancelAtPeriodEndOk returns a tuple with the CancelAtPeriodEnd field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelAtPeriodEnd

`func (o *SubscriptionInfo) SetCancelAtPeriodEnd(v bool)`

SetCancelAtPeriodEnd sets CancelAtPeriodEnd field to given value.

### HasCancelAtPeriodEnd

`func (o *SubscriptionInfo) HasCancelAtPeriodEnd() bool`

HasCancelAtPeriodEnd returns a boolean if a field has been set.

### GetCancelEffectiveAt

`func (o *SubscriptionInfo) GetCancelEffectiveAt() time.Time`

GetCancelEffectiveAt returns the CancelEffectiveAt field if non-nil, zero value otherwise.

### GetCancelEffectiveAtOk

`func (o *SubscriptionInfo) GetCancelEffectiveAtOk() (*time.Time, bool)`

GetCancelEffectiveAtOk returns a tuple with the CancelEffectiveAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelEffectiveAt

`func (o *SubscriptionInfo) SetCancelEffectiveAt(v time.Time)`

SetCancelEffectiveAt sets CancelEffectiveAt field to given value.

### HasCancelEffectiveAt

`func (o *SubscriptionInfo) HasCancelEffectiveAt() bool`

HasCancelEffectiveAt returns a boolean if a field has been set.

### SetCancelEffectiveAtNil

`func (o *SubscriptionInfo) SetCancelEffectiveAtNil(b bool)`

 SetCancelEffectiveAtNil sets the value for CancelEffectiveAt to be an explicit nil

### UnsetCancelEffectiveAt
`func (o *SubscriptionInfo) UnsetCancelEffectiveAt()`

UnsetCancelEffectiveAt ensures that no value is present for CancelEffectiveAt, not even an explicit nil
### GetMonthlyCredits

`func (o *SubscriptionInfo) GetMonthlyCredits() int32`

GetMonthlyCredits returns the MonthlyCredits field if non-nil, zero value otherwise.

### GetMonthlyCreditsOk

`func (o *SubscriptionInfo) GetMonthlyCreditsOk() (*int32, bool)`

GetMonthlyCreditsOk returns a tuple with the MonthlyCredits field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMonthlyCredits

`func (o *SubscriptionInfo) SetMonthlyCredits(v int32)`

SetMonthlyCredits sets MonthlyCredits field to given value.

### HasMonthlyCredits

`func (o *SubscriptionInfo) HasMonthlyCredits() bool`

HasMonthlyCredits returns a boolean if a field has been set.

### GetPendingPlanCode

`func (o *SubscriptionInfo) GetPendingPlanCode() string`

GetPendingPlanCode returns the PendingPlanCode field if non-nil, zero value otherwise.

### GetPendingPlanCodeOk

`func (o *SubscriptionInfo) GetPendingPlanCodeOk() (*string, bool)`

GetPendingPlanCodeOk returns a tuple with the PendingPlanCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPendingPlanCode

`func (o *SubscriptionInfo) SetPendingPlanCode(v string)`

SetPendingPlanCode sets PendingPlanCode field to given value.

### HasPendingPlanCode

`func (o *SubscriptionInfo) HasPendingPlanCode() bool`

HasPendingPlanCode returns a boolean if a field has been set.

### SetPendingPlanCodeNil

`func (o *SubscriptionInfo) SetPendingPlanCodeNil(b bool)`

 SetPendingPlanCodeNil sets the value for PendingPlanCode to be an explicit nil

### UnsetPendingPlanCode
`func (o *SubscriptionInfo) UnsetPendingPlanCode()`

UnsetPendingPlanCode ensures that no value is present for PendingPlanCode, not even an explicit nil
### GetPendingPlanTitle

`func (o *SubscriptionInfo) GetPendingPlanTitle() string`

GetPendingPlanTitle returns the PendingPlanTitle field if non-nil, zero value otherwise.

### GetPendingPlanTitleOk

`func (o *SubscriptionInfo) GetPendingPlanTitleOk() (*string, bool)`

GetPendingPlanTitleOk returns a tuple with the PendingPlanTitle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPendingPlanTitle

`func (o *SubscriptionInfo) SetPendingPlanTitle(v string)`

SetPendingPlanTitle sets PendingPlanTitle field to given value.

### HasPendingPlanTitle

`func (o *SubscriptionInfo) HasPendingPlanTitle() bool`

HasPendingPlanTitle returns a boolean if a field has been set.

### SetPendingPlanTitleNil

`func (o *SubscriptionInfo) SetPendingPlanTitleNil(b bool)`

 SetPendingPlanTitleNil sets the value for PendingPlanTitle to be an explicit nil

### UnsetPendingPlanTitle
`func (o *SubscriptionInfo) UnsetPendingPlanTitle()`

UnsetPendingPlanTitle ensures that no value is present for PendingPlanTitle, not even an explicit nil
### GetPendingChangeEffectiveAt

`func (o *SubscriptionInfo) GetPendingChangeEffectiveAt() time.Time`

GetPendingChangeEffectiveAt returns the PendingChangeEffectiveAt field if non-nil, zero value otherwise.

### GetPendingChangeEffectiveAtOk

`func (o *SubscriptionInfo) GetPendingChangeEffectiveAtOk() (*time.Time, bool)`

GetPendingChangeEffectiveAtOk returns a tuple with the PendingChangeEffectiveAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPendingChangeEffectiveAt

`func (o *SubscriptionInfo) SetPendingChangeEffectiveAt(v time.Time)`

SetPendingChangeEffectiveAt sets PendingChangeEffectiveAt field to given value.

### HasPendingChangeEffectiveAt

`func (o *SubscriptionInfo) HasPendingChangeEffectiveAt() bool`

HasPendingChangeEffectiveAt returns a boolean if a field has been set.

### SetPendingChangeEffectiveAtNil

`func (o *SubscriptionInfo) SetPendingChangeEffectiveAtNil(b bool)`

 SetPendingChangeEffectiveAtNil sets the value for PendingChangeEffectiveAt to be an explicit nil

### UnsetPendingChangeEffectiveAt
`func (o *SubscriptionInfo) UnsetPendingChangeEffectiveAt()`

UnsetPendingChangeEffectiveAt ensures that no value is present for PendingChangeEffectiveAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



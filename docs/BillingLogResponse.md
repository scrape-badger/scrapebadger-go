# BillingLogResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**MonitorId** | **string** |  | 
**MonitorName** | **string** |  | 
**BilledAt** | **time.Time** |  | 
**NumAccounts** | **int32** |  | 
**CreditsDeducted** | **float32** |  | 
**TierLabel** | **string** |  | 
**RateApplied** | **float32** |  | 

## Methods

### NewBillingLogResponse

`func NewBillingLogResponse(id string, monitorId string, monitorName string, billedAt time.Time, numAccounts int32, creditsDeducted float32, tierLabel string, rateApplied float32, ) *BillingLogResponse`

NewBillingLogResponse instantiates a new BillingLogResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBillingLogResponseWithDefaults

`func NewBillingLogResponseWithDefaults() *BillingLogResponse`

NewBillingLogResponseWithDefaults instantiates a new BillingLogResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *BillingLogResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *BillingLogResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *BillingLogResponse) SetId(v string)`

SetId sets Id field to given value.


### GetMonitorId

`func (o *BillingLogResponse) GetMonitorId() string`

GetMonitorId returns the MonitorId field if non-nil, zero value otherwise.

### GetMonitorIdOk

`func (o *BillingLogResponse) GetMonitorIdOk() (*string, bool)`

GetMonitorIdOk returns a tuple with the MonitorId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMonitorId

`func (o *BillingLogResponse) SetMonitorId(v string)`

SetMonitorId sets MonitorId field to given value.


### GetMonitorName

`func (o *BillingLogResponse) GetMonitorName() string`

GetMonitorName returns the MonitorName field if non-nil, zero value otherwise.

### GetMonitorNameOk

`func (o *BillingLogResponse) GetMonitorNameOk() (*string, bool)`

GetMonitorNameOk returns a tuple with the MonitorName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMonitorName

`func (o *BillingLogResponse) SetMonitorName(v string)`

SetMonitorName sets MonitorName field to given value.


### GetBilledAt

`func (o *BillingLogResponse) GetBilledAt() time.Time`

GetBilledAt returns the BilledAt field if non-nil, zero value otherwise.

### GetBilledAtOk

`func (o *BillingLogResponse) GetBilledAtOk() (*time.Time, bool)`

GetBilledAtOk returns a tuple with the BilledAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBilledAt

`func (o *BillingLogResponse) SetBilledAt(v time.Time)`

SetBilledAt sets BilledAt field to given value.


### GetNumAccounts

`func (o *BillingLogResponse) GetNumAccounts() int32`

GetNumAccounts returns the NumAccounts field if non-nil, zero value otherwise.

### GetNumAccountsOk

`func (o *BillingLogResponse) GetNumAccountsOk() (*int32, bool)`

GetNumAccountsOk returns a tuple with the NumAccounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumAccounts

`func (o *BillingLogResponse) SetNumAccounts(v int32)`

SetNumAccounts sets NumAccounts field to given value.


### GetCreditsDeducted

`func (o *BillingLogResponse) GetCreditsDeducted() float32`

GetCreditsDeducted returns the CreditsDeducted field if non-nil, zero value otherwise.

### GetCreditsDeductedOk

`func (o *BillingLogResponse) GetCreditsDeductedOk() (*float32, bool)`

GetCreditsDeductedOk returns a tuple with the CreditsDeducted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreditsDeducted

`func (o *BillingLogResponse) SetCreditsDeducted(v float32)`

SetCreditsDeducted sets CreditsDeducted field to given value.


### GetTierLabel

`func (o *BillingLogResponse) GetTierLabel() string`

GetTierLabel returns the TierLabel field if non-nil, zero value otherwise.

### GetTierLabelOk

`func (o *BillingLogResponse) GetTierLabelOk() (*string, bool)`

GetTierLabelOk returns a tuple with the TierLabel field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTierLabel

`func (o *BillingLogResponse) SetTierLabel(v string)`

SetTierLabel sets TierLabel field to given value.


### GetRateApplied

`func (o *BillingLogResponse) GetRateApplied() float32`

GetRateApplied returns the RateApplied field if non-nil, zero value otherwise.

### GetRateAppliedOk

`func (o *BillingLogResponse) GetRateAppliedOk() (*float32, bool)`

GetRateAppliedOk returns a tuple with the RateApplied field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRateApplied

`func (o *BillingLogResponse) SetRateApplied(v float32)`

SetRateApplied sets RateApplied field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



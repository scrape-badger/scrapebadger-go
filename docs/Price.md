# Price

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Current** | Pointer to [**NullablePriceValue**](PriceValue.md) |  | [optional] 
**Previous** | Pointer to [**NullablePriceValue**](PriceValue.md) |  | [optional] 
**Rrp** | Pointer to [**NullablePriceValue**](PriceValue.md) |  | [optional] 
**Currency** | Pointer to **NullableString** |  | [optional] 
**IsMarkedDown** | Pointer to **bool** |  | [optional] [default to false]
**IsOutletPrice** | Pointer to **bool** |  | [optional] [default to false]
**DiscountPercentage** | Pointer to **NullableFloat32** |  | [optional] 

## Methods

### NewPrice

`func NewPrice() *Price`

NewPrice instantiates a new Price object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPriceWithDefaults

`func NewPriceWithDefaults() *Price`

NewPriceWithDefaults instantiates a new Price object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCurrent

`func (o *Price) GetCurrent() PriceValue`

GetCurrent returns the Current field if non-nil, zero value otherwise.

### GetCurrentOk

`func (o *Price) GetCurrentOk() (*PriceValue, bool)`

GetCurrentOk returns a tuple with the Current field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrent

`func (o *Price) SetCurrent(v PriceValue)`

SetCurrent sets Current field to given value.

### HasCurrent

`func (o *Price) HasCurrent() bool`

HasCurrent returns a boolean if a field has been set.

### SetCurrentNil

`func (o *Price) SetCurrentNil(b bool)`

 SetCurrentNil sets the value for Current to be an explicit nil

### UnsetCurrent
`func (o *Price) UnsetCurrent()`

UnsetCurrent ensures that no value is present for Current, not even an explicit nil
### GetPrevious

`func (o *Price) GetPrevious() PriceValue`

GetPrevious returns the Previous field if non-nil, zero value otherwise.

### GetPreviousOk

`func (o *Price) GetPreviousOk() (*PriceValue, bool)`

GetPreviousOk returns a tuple with the Previous field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrevious

`func (o *Price) SetPrevious(v PriceValue)`

SetPrevious sets Previous field to given value.

### HasPrevious

`func (o *Price) HasPrevious() bool`

HasPrevious returns a boolean if a field has been set.

### SetPreviousNil

`func (o *Price) SetPreviousNil(b bool)`

 SetPreviousNil sets the value for Previous to be an explicit nil

### UnsetPrevious
`func (o *Price) UnsetPrevious()`

UnsetPrevious ensures that no value is present for Previous, not even an explicit nil
### GetRrp

`func (o *Price) GetRrp() PriceValue`

GetRrp returns the Rrp field if non-nil, zero value otherwise.

### GetRrpOk

`func (o *Price) GetRrpOk() (*PriceValue, bool)`

GetRrpOk returns a tuple with the Rrp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRrp

`func (o *Price) SetRrp(v PriceValue)`

SetRrp sets Rrp field to given value.

### HasRrp

`func (o *Price) HasRrp() bool`

HasRrp returns a boolean if a field has been set.

### SetRrpNil

`func (o *Price) SetRrpNil(b bool)`

 SetRrpNil sets the value for Rrp to be an explicit nil

### UnsetRrp
`func (o *Price) UnsetRrp()`

UnsetRrp ensures that no value is present for Rrp, not even an explicit nil
### GetCurrency

`func (o *Price) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *Price) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *Price) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *Price) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### SetCurrencyNil

`func (o *Price) SetCurrencyNil(b bool)`

 SetCurrencyNil sets the value for Currency to be an explicit nil

### UnsetCurrency
`func (o *Price) UnsetCurrency()`

UnsetCurrency ensures that no value is present for Currency, not even an explicit nil
### GetIsMarkedDown

`func (o *Price) GetIsMarkedDown() bool`

GetIsMarkedDown returns the IsMarkedDown field if non-nil, zero value otherwise.

### GetIsMarkedDownOk

`func (o *Price) GetIsMarkedDownOk() (*bool, bool)`

GetIsMarkedDownOk returns a tuple with the IsMarkedDown field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsMarkedDown

`func (o *Price) SetIsMarkedDown(v bool)`

SetIsMarkedDown sets IsMarkedDown field to given value.

### HasIsMarkedDown

`func (o *Price) HasIsMarkedDown() bool`

HasIsMarkedDown returns a boolean if a field has been set.

### GetIsOutletPrice

`func (o *Price) GetIsOutletPrice() bool`

GetIsOutletPrice returns the IsOutletPrice field if non-nil, zero value otherwise.

### GetIsOutletPriceOk

`func (o *Price) GetIsOutletPriceOk() (*bool, bool)`

GetIsOutletPriceOk returns a tuple with the IsOutletPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsOutletPrice

`func (o *Price) SetIsOutletPrice(v bool)`

SetIsOutletPrice sets IsOutletPrice field to given value.

### HasIsOutletPrice

`func (o *Price) HasIsOutletPrice() bool`

HasIsOutletPrice returns a boolean if a field has been set.

### GetDiscountPercentage

`func (o *Price) GetDiscountPercentage() float32`

GetDiscountPercentage returns the DiscountPercentage field if non-nil, zero value otherwise.

### GetDiscountPercentageOk

`func (o *Price) GetDiscountPercentageOk() (*float32, bool)`

GetDiscountPercentageOk returns a tuple with the DiscountPercentage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiscountPercentage

`func (o *Price) SetDiscountPercentage(v float32)`

SetDiscountPercentage sets DiscountPercentage field to given value.

### HasDiscountPercentage

`func (o *Price) HasDiscountPercentage() bool`

HasDiscountPercentage returns a boolean if a field has been set.

### SetDiscountPercentageNil

`func (o *Price) SetDiscountPercentageNil(b bool)`

 SetDiscountPercentageNil sets the value for DiscountPercentage to be an explicit nil

### UnsetDiscountPercentage
`func (o *Price) UnsetDiscountPercentage()`

UnsetDiscountPercentage ensures that no value is present for DiscountPercentage, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



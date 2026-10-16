# ProductPrice

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Current** | Pointer to [**PriceValue**](PriceValue.md) |  | [optional] 
**Previous** | Pointer to [**PriceValue**](PriceValue.md) |  | [optional] 
**Rrp** | Pointer to [**PriceValue**](PriceValue.md) |  | [optional] 
**Currency** | Pointer to **string** |  | [optional] 
**IsMarkedDown** | Pointer to **bool** |  | [optional] [default to false]
**IsOutletPrice** | Pointer to **bool** |  | [optional] [default to false]
**DiscountPercentage** | Pointer to **float32** |  | [optional] 

## Methods

### NewProductPrice

`func NewProductPrice() *ProductPrice`

NewProductPrice instantiates a new ProductPrice object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProductPriceWithDefaults

`func NewProductPriceWithDefaults() *ProductPrice`

NewProductPriceWithDefaults instantiates a new ProductPrice object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCurrent

`func (o *ProductPrice) GetCurrent() PriceValue`

GetCurrent returns the Current field if non-nil, zero value otherwise.

### GetCurrentOk

`func (o *ProductPrice) GetCurrentOk() (*PriceValue, bool)`

GetCurrentOk returns a tuple with the Current field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrent

`func (o *ProductPrice) SetCurrent(v PriceValue)`

SetCurrent sets Current field to given value.

### HasCurrent

`func (o *ProductPrice) HasCurrent() bool`

HasCurrent returns a boolean if a field has been set.

### GetPrevious

`func (o *ProductPrice) GetPrevious() PriceValue`

GetPrevious returns the Previous field if non-nil, zero value otherwise.

### GetPreviousOk

`func (o *ProductPrice) GetPreviousOk() (*PriceValue, bool)`

GetPreviousOk returns a tuple with the Previous field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrevious

`func (o *ProductPrice) SetPrevious(v PriceValue)`

SetPrevious sets Previous field to given value.

### HasPrevious

`func (o *ProductPrice) HasPrevious() bool`

HasPrevious returns a boolean if a field has been set.

### GetRrp

`func (o *ProductPrice) GetRrp() PriceValue`

GetRrp returns the Rrp field if non-nil, zero value otherwise.

### GetRrpOk

`func (o *ProductPrice) GetRrpOk() (*PriceValue, bool)`

GetRrpOk returns a tuple with the Rrp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRrp

`func (o *ProductPrice) SetRrp(v PriceValue)`

SetRrp sets Rrp field to given value.

### HasRrp

`func (o *ProductPrice) HasRrp() bool`

HasRrp returns a boolean if a field has been set.

### GetCurrency

`func (o *ProductPrice) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *ProductPrice) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *ProductPrice) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *ProductPrice) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetIsMarkedDown

`func (o *ProductPrice) GetIsMarkedDown() bool`

GetIsMarkedDown returns the IsMarkedDown field if non-nil, zero value otherwise.

### GetIsMarkedDownOk

`func (o *ProductPrice) GetIsMarkedDownOk() (*bool, bool)`

GetIsMarkedDownOk returns a tuple with the IsMarkedDown field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsMarkedDown

`func (o *ProductPrice) SetIsMarkedDown(v bool)`

SetIsMarkedDown sets IsMarkedDown field to given value.

### HasIsMarkedDown

`func (o *ProductPrice) HasIsMarkedDown() bool`

HasIsMarkedDown returns a boolean if a field has been set.

### GetIsOutletPrice

`func (o *ProductPrice) GetIsOutletPrice() bool`

GetIsOutletPrice returns the IsOutletPrice field if non-nil, zero value otherwise.

### GetIsOutletPriceOk

`func (o *ProductPrice) GetIsOutletPriceOk() (*bool, bool)`

GetIsOutletPriceOk returns a tuple with the IsOutletPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsOutletPrice

`func (o *ProductPrice) SetIsOutletPrice(v bool)`

SetIsOutletPrice sets IsOutletPrice field to given value.

### HasIsOutletPrice

`func (o *ProductPrice) HasIsOutletPrice() bool`

HasIsOutletPrice returns a boolean if a field has been set.

### GetDiscountPercentage

`func (o *ProductPrice) GetDiscountPercentage() float32`

GetDiscountPercentage returns the DiscountPercentage field if non-nil, zero value otherwise.

### GetDiscountPercentageOk

`func (o *ProductPrice) GetDiscountPercentageOk() (*float32, bool)`

GetDiscountPercentageOk returns a tuple with the DiscountPercentage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiscountPercentage

`func (o *ProductPrice) SetDiscountPercentage(v float32)`

SetDiscountPercentage sets DiscountPercentage field to given value.

### HasDiscountPercentage

`func (o *ProductPrice) HasDiscountPercentage() bool`

HasDiscountPercentage returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



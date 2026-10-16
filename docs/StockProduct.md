# StockProduct

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProductId** | **int32** |  | 
**ProductPrice** | Pointer to [**NullablePrice**](Price.md) |  | [optional] 
**IsInStock** | **bool** |  | 
**Variants** | Pointer to [**[]Variant**](Variant.md) |  | [optional] 

## Methods

### NewStockProduct

`func NewStockProduct(productId int32, isInStock bool, ) *StockProduct`

NewStockProduct instantiates a new StockProduct object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStockProductWithDefaults

`func NewStockProductWithDefaults() *StockProduct`

NewStockProductWithDefaults instantiates a new StockProduct object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProductId

`func (o *StockProduct) GetProductId() int32`

GetProductId returns the ProductId field if non-nil, zero value otherwise.

### GetProductIdOk

`func (o *StockProduct) GetProductIdOk() (*int32, bool)`

GetProductIdOk returns a tuple with the ProductId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductId

`func (o *StockProduct) SetProductId(v int32)`

SetProductId sets ProductId field to given value.


### GetProductPrice

`func (o *StockProduct) GetProductPrice() Price`

GetProductPrice returns the ProductPrice field if non-nil, zero value otherwise.

### GetProductPriceOk

`func (o *StockProduct) GetProductPriceOk() (*Price, bool)`

GetProductPriceOk returns a tuple with the ProductPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductPrice

`func (o *StockProduct) SetProductPrice(v Price)`

SetProductPrice sets ProductPrice field to given value.

### HasProductPrice

`func (o *StockProduct) HasProductPrice() bool`

HasProductPrice returns a boolean if a field has been set.

### SetProductPriceNil

`func (o *StockProduct) SetProductPriceNil(b bool)`

 SetProductPriceNil sets the value for ProductPrice to be an explicit nil

### UnsetProductPrice
`func (o *StockProduct) UnsetProductPrice()`

UnsetProductPrice ensures that no value is present for ProductPrice, not even an explicit nil
### GetIsInStock

`func (o *StockProduct) GetIsInStock() bool`

GetIsInStock returns the IsInStock field if non-nil, zero value otherwise.

### GetIsInStockOk

`func (o *StockProduct) GetIsInStockOk() (*bool, bool)`

GetIsInStockOk returns a tuple with the IsInStock field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsInStock

`func (o *StockProduct) SetIsInStock(v bool)`

SetIsInStock sets IsInStock field to given value.


### GetVariants

`func (o *StockProduct) GetVariants() []Variant`

GetVariants returns the Variants field if non-nil, zero value otherwise.

### GetVariantsOk

`func (o *StockProduct) GetVariantsOk() (*[]Variant, bool)`

GetVariantsOk returns a tuple with the Variants field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVariants

`func (o *StockProduct) SetVariants(v []Variant)`

SetVariants sets Variants field to given value.

### HasVariants

`func (o *StockProduct) HasVariants() bool`

HasVariants returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



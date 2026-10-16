# Variant

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**VariantId** | Pointer to **NullableInt32** |  | [optional] 
**Id** | Pointer to **NullableInt32** |  | [optional] 
**Size** | Pointer to **NullableString** |  | [optional] 
**BrandSize** | Pointer to **NullableString** |  | [optional] 
**SizeId** | Pointer to **NullableInt32** |  | [optional] 
**Colour** | Pointer to **NullableString** |  | [optional] 
**ColourWayId** | Pointer to **NullableInt32** |  | [optional] 
**Sku** | Pointer to **NullableString** |  | [optional] 
**IsAvailable** | Pointer to **NullableBool** |  | [optional] 
**IsInStock** | Pointer to **NullableBool** |  | [optional] 
**IsLowInStock** | Pointer to **NullableBool** |  | [optional] 
**IsRestockingSoon** | Pointer to **NullableBool** |  | [optional] 
**Price** | Pointer to [**NullablePrice**](Price.md) |  | [optional] 

## Methods

### NewVariant

`func NewVariant() *Variant`

NewVariant instantiates a new Variant object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVariantWithDefaults

`func NewVariantWithDefaults() *Variant`

NewVariantWithDefaults instantiates a new Variant object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVariantId

`func (o *Variant) GetVariantId() int32`

GetVariantId returns the VariantId field if non-nil, zero value otherwise.

### GetVariantIdOk

`func (o *Variant) GetVariantIdOk() (*int32, bool)`

GetVariantIdOk returns a tuple with the VariantId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVariantId

`func (o *Variant) SetVariantId(v int32)`

SetVariantId sets VariantId field to given value.

### HasVariantId

`func (o *Variant) HasVariantId() bool`

HasVariantId returns a boolean if a field has been set.

### SetVariantIdNil

`func (o *Variant) SetVariantIdNil(b bool)`

 SetVariantIdNil sets the value for VariantId to be an explicit nil

### UnsetVariantId
`func (o *Variant) UnsetVariantId()`

UnsetVariantId ensures that no value is present for VariantId, not even an explicit nil
### GetId

`func (o *Variant) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Variant) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Variant) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *Variant) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *Variant) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *Variant) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil
### GetSize

`func (o *Variant) GetSize() string`

GetSize returns the Size field if non-nil, zero value otherwise.

### GetSizeOk

`func (o *Variant) GetSizeOk() (*string, bool)`

GetSizeOk returns a tuple with the Size field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSize

`func (o *Variant) SetSize(v string)`

SetSize sets Size field to given value.

### HasSize

`func (o *Variant) HasSize() bool`

HasSize returns a boolean if a field has been set.

### SetSizeNil

`func (o *Variant) SetSizeNil(b bool)`

 SetSizeNil sets the value for Size to be an explicit nil

### UnsetSize
`func (o *Variant) UnsetSize()`

UnsetSize ensures that no value is present for Size, not even an explicit nil
### GetBrandSize

`func (o *Variant) GetBrandSize() string`

GetBrandSize returns the BrandSize field if non-nil, zero value otherwise.

### GetBrandSizeOk

`func (o *Variant) GetBrandSizeOk() (*string, bool)`

GetBrandSizeOk returns a tuple with the BrandSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBrandSize

`func (o *Variant) SetBrandSize(v string)`

SetBrandSize sets BrandSize field to given value.

### HasBrandSize

`func (o *Variant) HasBrandSize() bool`

HasBrandSize returns a boolean if a field has been set.

### SetBrandSizeNil

`func (o *Variant) SetBrandSizeNil(b bool)`

 SetBrandSizeNil sets the value for BrandSize to be an explicit nil

### UnsetBrandSize
`func (o *Variant) UnsetBrandSize()`

UnsetBrandSize ensures that no value is present for BrandSize, not even an explicit nil
### GetSizeId

`func (o *Variant) GetSizeId() int32`

GetSizeId returns the SizeId field if non-nil, zero value otherwise.

### GetSizeIdOk

`func (o *Variant) GetSizeIdOk() (*int32, bool)`

GetSizeIdOk returns a tuple with the SizeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSizeId

`func (o *Variant) SetSizeId(v int32)`

SetSizeId sets SizeId field to given value.

### HasSizeId

`func (o *Variant) HasSizeId() bool`

HasSizeId returns a boolean if a field has been set.

### SetSizeIdNil

`func (o *Variant) SetSizeIdNil(b bool)`

 SetSizeIdNil sets the value for SizeId to be an explicit nil

### UnsetSizeId
`func (o *Variant) UnsetSizeId()`

UnsetSizeId ensures that no value is present for SizeId, not even an explicit nil
### GetColour

`func (o *Variant) GetColour() string`

GetColour returns the Colour field if non-nil, zero value otherwise.

### GetColourOk

`func (o *Variant) GetColourOk() (*string, bool)`

GetColourOk returns a tuple with the Colour field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColour

`func (o *Variant) SetColour(v string)`

SetColour sets Colour field to given value.

### HasColour

`func (o *Variant) HasColour() bool`

HasColour returns a boolean if a field has been set.

### SetColourNil

`func (o *Variant) SetColourNil(b bool)`

 SetColourNil sets the value for Colour to be an explicit nil

### UnsetColour
`func (o *Variant) UnsetColour()`

UnsetColour ensures that no value is present for Colour, not even an explicit nil
### GetColourWayId

`func (o *Variant) GetColourWayId() int32`

GetColourWayId returns the ColourWayId field if non-nil, zero value otherwise.

### GetColourWayIdOk

`func (o *Variant) GetColourWayIdOk() (*int32, bool)`

GetColourWayIdOk returns a tuple with the ColourWayId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColourWayId

`func (o *Variant) SetColourWayId(v int32)`

SetColourWayId sets ColourWayId field to given value.

### HasColourWayId

`func (o *Variant) HasColourWayId() bool`

HasColourWayId returns a boolean if a field has been set.

### SetColourWayIdNil

`func (o *Variant) SetColourWayIdNil(b bool)`

 SetColourWayIdNil sets the value for ColourWayId to be an explicit nil

### UnsetColourWayId
`func (o *Variant) UnsetColourWayId()`

UnsetColourWayId ensures that no value is present for ColourWayId, not even an explicit nil
### GetSku

`func (o *Variant) GetSku() string`

GetSku returns the Sku field if non-nil, zero value otherwise.

### GetSkuOk

`func (o *Variant) GetSkuOk() (*string, bool)`

GetSkuOk returns a tuple with the Sku field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSku

`func (o *Variant) SetSku(v string)`

SetSku sets Sku field to given value.

### HasSku

`func (o *Variant) HasSku() bool`

HasSku returns a boolean if a field has been set.

### SetSkuNil

`func (o *Variant) SetSkuNil(b bool)`

 SetSkuNil sets the value for Sku to be an explicit nil

### UnsetSku
`func (o *Variant) UnsetSku()`

UnsetSku ensures that no value is present for Sku, not even an explicit nil
### GetIsAvailable

`func (o *Variant) GetIsAvailable() bool`

GetIsAvailable returns the IsAvailable field if non-nil, zero value otherwise.

### GetIsAvailableOk

`func (o *Variant) GetIsAvailableOk() (*bool, bool)`

GetIsAvailableOk returns a tuple with the IsAvailable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsAvailable

`func (o *Variant) SetIsAvailable(v bool)`

SetIsAvailable sets IsAvailable field to given value.

### HasIsAvailable

`func (o *Variant) HasIsAvailable() bool`

HasIsAvailable returns a boolean if a field has been set.

### SetIsAvailableNil

`func (o *Variant) SetIsAvailableNil(b bool)`

 SetIsAvailableNil sets the value for IsAvailable to be an explicit nil

### UnsetIsAvailable
`func (o *Variant) UnsetIsAvailable()`

UnsetIsAvailable ensures that no value is present for IsAvailable, not even an explicit nil
### GetIsInStock

`func (o *Variant) GetIsInStock() bool`

GetIsInStock returns the IsInStock field if non-nil, zero value otherwise.

### GetIsInStockOk

`func (o *Variant) GetIsInStockOk() (*bool, bool)`

GetIsInStockOk returns a tuple with the IsInStock field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsInStock

`func (o *Variant) SetIsInStock(v bool)`

SetIsInStock sets IsInStock field to given value.

### HasIsInStock

`func (o *Variant) HasIsInStock() bool`

HasIsInStock returns a boolean if a field has been set.

### SetIsInStockNil

`func (o *Variant) SetIsInStockNil(b bool)`

 SetIsInStockNil sets the value for IsInStock to be an explicit nil

### UnsetIsInStock
`func (o *Variant) UnsetIsInStock()`

UnsetIsInStock ensures that no value is present for IsInStock, not even an explicit nil
### GetIsLowInStock

`func (o *Variant) GetIsLowInStock() bool`

GetIsLowInStock returns the IsLowInStock field if non-nil, zero value otherwise.

### GetIsLowInStockOk

`func (o *Variant) GetIsLowInStockOk() (*bool, bool)`

GetIsLowInStockOk returns a tuple with the IsLowInStock field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsLowInStock

`func (o *Variant) SetIsLowInStock(v bool)`

SetIsLowInStock sets IsLowInStock field to given value.

### HasIsLowInStock

`func (o *Variant) HasIsLowInStock() bool`

HasIsLowInStock returns a boolean if a field has been set.

### SetIsLowInStockNil

`func (o *Variant) SetIsLowInStockNil(b bool)`

 SetIsLowInStockNil sets the value for IsLowInStock to be an explicit nil

### UnsetIsLowInStock
`func (o *Variant) UnsetIsLowInStock()`

UnsetIsLowInStock ensures that no value is present for IsLowInStock, not even an explicit nil
### GetIsRestockingSoon

`func (o *Variant) GetIsRestockingSoon() bool`

GetIsRestockingSoon returns the IsRestockingSoon field if non-nil, zero value otherwise.

### GetIsRestockingSoonOk

`func (o *Variant) GetIsRestockingSoonOk() (*bool, bool)`

GetIsRestockingSoonOk returns a tuple with the IsRestockingSoon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsRestockingSoon

`func (o *Variant) SetIsRestockingSoon(v bool)`

SetIsRestockingSoon sets IsRestockingSoon field to given value.

### HasIsRestockingSoon

`func (o *Variant) HasIsRestockingSoon() bool`

HasIsRestockingSoon returns a boolean if a field has been set.

### SetIsRestockingSoonNil

`func (o *Variant) SetIsRestockingSoonNil(b bool)`

 SetIsRestockingSoonNil sets the value for IsRestockingSoon to be an explicit nil

### UnsetIsRestockingSoon
`func (o *Variant) UnsetIsRestockingSoon()`

UnsetIsRestockingSoon ensures that no value is present for IsRestockingSoon, not even an explicit nil
### GetPrice

`func (o *Variant) GetPrice() Price`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *Variant) GetPriceOk() (*Price, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *Variant) SetPrice(v Price)`

SetPrice sets Price field to given value.

### HasPrice

`func (o *Variant) HasPrice() bool`

HasPrice returns a boolean if a field has been set.

### SetPriceNil

`func (o *Variant) SetPriceNil(b bool)`

 SetPriceNil sets the value for Price to be an explicit nil

### UnsetPrice
`func (o *Variant) UnsetPrice()`

UnsetPrice ensures that no value is present for Price, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



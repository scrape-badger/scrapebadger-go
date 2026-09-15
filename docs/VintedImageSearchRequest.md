# VintedImageSearchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ImageUrl** | Pointer to **NullableString** |  | [optional] 
**ImageBase64** | Pointer to **NullableString** |  | [optional] 
**Market** | Pointer to **string** | Vinted market code; uk aliases gb | [optional] [default to "fr"]
**Page** | Pointer to **int32** |  | [optional] [default to 1]
**PerPage** | Pointer to **int32** |  | [optional] [default to 20]
**PriceFrom** | Pointer to **NullableFloat32** |  | [optional] 
**PriceTo** | Pointer to **NullableFloat32** |  | [optional] 
**BrandIds** | Pointer to **NullableString** |  | [optional] 
**CatalogIds** | Pointer to **NullableString** |  | [optional] 
**ColorIds** | Pointer to **NullableString** |  | [optional] 
**SizeIds** | Pointer to **NullableString** |  | [optional] 
**MaterialIds** | Pointer to **NullableString** |  | [optional] 
**StatusIds** | Pointer to **NullableString** |  | [optional] 
**Time** | Pointer to **NullableInt32** |  | [optional] 
**SearchSessionId** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewVintedImageSearchRequest

`func NewVintedImageSearchRequest() *VintedImageSearchRequest`

NewVintedImageSearchRequest instantiates a new VintedImageSearchRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVintedImageSearchRequestWithDefaults

`func NewVintedImageSearchRequestWithDefaults() *VintedImageSearchRequest`

NewVintedImageSearchRequestWithDefaults instantiates a new VintedImageSearchRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetImageUrl

`func (o *VintedImageSearchRequest) GetImageUrl() string`

GetImageUrl returns the ImageUrl field if non-nil, zero value otherwise.

### GetImageUrlOk

`func (o *VintedImageSearchRequest) GetImageUrlOk() (*string, bool)`

GetImageUrlOk returns a tuple with the ImageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImageUrl

`func (o *VintedImageSearchRequest) SetImageUrl(v string)`

SetImageUrl sets ImageUrl field to given value.

### HasImageUrl

`func (o *VintedImageSearchRequest) HasImageUrl() bool`

HasImageUrl returns a boolean if a field has been set.

### SetImageUrlNil

`func (o *VintedImageSearchRequest) SetImageUrlNil(b bool)`

 SetImageUrlNil sets the value for ImageUrl to be an explicit nil

### UnsetImageUrl
`func (o *VintedImageSearchRequest) UnsetImageUrl()`

UnsetImageUrl ensures that no value is present for ImageUrl, not even an explicit nil
### GetImageBase64

`func (o *VintedImageSearchRequest) GetImageBase64() string`

GetImageBase64 returns the ImageBase64 field if non-nil, zero value otherwise.

### GetImageBase64Ok

`func (o *VintedImageSearchRequest) GetImageBase64Ok() (*string, bool)`

GetImageBase64Ok returns a tuple with the ImageBase64 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImageBase64

`func (o *VintedImageSearchRequest) SetImageBase64(v string)`

SetImageBase64 sets ImageBase64 field to given value.

### HasImageBase64

`func (o *VintedImageSearchRequest) HasImageBase64() bool`

HasImageBase64 returns a boolean if a field has been set.

### SetImageBase64Nil

`func (o *VintedImageSearchRequest) SetImageBase64Nil(b bool)`

 SetImageBase64Nil sets the value for ImageBase64 to be an explicit nil

### UnsetImageBase64
`func (o *VintedImageSearchRequest) UnsetImageBase64()`

UnsetImageBase64 ensures that no value is present for ImageBase64, not even an explicit nil
### GetMarket

`func (o *VintedImageSearchRequest) GetMarket() string`

GetMarket returns the Market field if non-nil, zero value otherwise.

### GetMarketOk

`func (o *VintedImageSearchRequest) GetMarketOk() (*string, bool)`

GetMarketOk returns a tuple with the Market field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMarket

`func (o *VintedImageSearchRequest) SetMarket(v string)`

SetMarket sets Market field to given value.

### HasMarket

`func (o *VintedImageSearchRequest) HasMarket() bool`

HasMarket returns a boolean if a field has been set.

### GetPage

`func (o *VintedImageSearchRequest) GetPage() int32`

GetPage returns the Page field if non-nil, zero value otherwise.

### GetPageOk

`func (o *VintedImageSearchRequest) GetPageOk() (*int32, bool)`

GetPageOk returns a tuple with the Page field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPage

`func (o *VintedImageSearchRequest) SetPage(v int32)`

SetPage sets Page field to given value.

### HasPage

`func (o *VintedImageSearchRequest) HasPage() bool`

HasPage returns a boolean if a field has been set.

### GetPerPage

`func (o *VintedImageSearchRequest) GetPerPage() int32`

GetPerPage returns the PerPage field if non-nil, zero value otherwise.

### GetPerPageOk

`func (o *VintedImageSearchRequest) GetPerPageOk() (*int32, bool)`

GetPerPageOk returns a tuple with the PerPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPerPage

`func (o *VintedImageSearchRequest) SetPerPage(v int32)`

SetPerPage sets PerPage field to given value.

### HasPerPage

`func (o *VintedImageSearchRequest) HasPerPage() bool`

HasPerPage returns a boolean if a field has been set.

### GetPriceFrom

`func (o *VintedImageSearchRequest) GetPriceFrom() float32`

GetPriceFrom returns the PriceFrom field if non-nil, zero value otherwise.

### GetPriceFromOk

`func (o *VintedImageSearchRequest) GetPriceFromOk() (*float32, bool)`

GetPriceFromOk returns a tuple with the PriceFrom field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceFrom

`func (o *VintedImageSearchRequest) SetPriceFrom(v float32)`

SetPriceFrom sets PriceFrom field to given value.

### HasPriceFrom

`func (o *VintedImageSearchRequest) HasPriceFrom() bool`

HasPriceFrom returns a boolean if a field has been set.

### SetPriceFromNil

`func (o *VintedImageSearchRequest) SetPriceFromNil(b bool)`

 SetPriceFromNil sets the value for PriceFrom to be an explicit nil

### UnsetPriceFrom
`func (o *VintedImageSearchRequest) UnsetPriceFrom()`

UnsetPriceFrom ensures that no value is present for PriceFrom, not even an explicit nil
### GetPriceTo

`func (o *VintedImageSearchRequest) GetPriceTo() float32`

GetPriceTo returns the PriceTo field if non-nil, zero value otherwise.

### GetPriceToOk

`func (o *VintedImageSearchRequest) GetPriceToOk() (*float32, bool)`

GetPriceToOk returns a tuple with the PriceTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceTo

`func (o *VintedImageSearchRequest) SetPriceTo(v float32)`

SetPriceTo sets PriceTo field to given value.

### HasPriceTo

`func (o *VintedImageSearchRequest) HasPriceTo() bool`

HasPriceTo returns a boolean if a field has been set.

### SetPriceToNil

`func (o *VintedImageSearchRequest) SetPriceToNil(b bool)`

 SetPriceToNil sets the value for PriceTo to be an explicit nil

### UnsetPriceTo
`func (o *VintedImageSearchRequest) UnsetPriceTo()`

UnsetPriceTo ensures that no value is present for PriceTo, not even an explicit nil
### GetBrandIds

`func (o *VintedImageSearchRequest) GetBrandIds() string`

GetBrandIds returns the BrandIds field if non-nil, zero value otherwise.

### GetBrandIdsOk

`func (o *VintedImageSearchRequest) GetBrandIdsOk() (*string, bool)`

GetBrandIdsOk returns a tuple with the BrandIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBrandIds

`func (o *VintedImageSearchRequest) SetBrandIds(v string)`

SetBrandIds sets BrandIds field to given value.

### HasBrandIds

`func (o *VintedImageSearchRequest) HasBrandIds() bool`

HasBrandIds returns a boolean if a field has been set.

### SetBrandIdsNil

`func (o *VintedImageSearchRequest) SetBrandIdsNil(b bool)`

 SetBrandIdsNil sets the value for BrandIds to be an explicit nil

### UnsetBrandIds
`func (o *VintedImageSearchRequest) UnsetBrandIds()`

UnsetBrandIds ensures that no value is present for BrandIds, not even an explicit nil
### GetCatalogIds

`func (o *VintedImageSearchRequest) GetCatalogIds() string`

GetCatalogIds returns the CatalogIds field if non-nil, zero value otherwise.

### GetCatalogIdsOk

`func (o *VintedImageSearchRequest) GetCatalogIdsOk() (*string, bool)`

GetCatalogIdsOk returns a tuple with the CatalogIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCatalogIds

`func (o *VintedImageSearchRequest) SetCatalogIds(v string)`

SetCatalogIds sets CatalogIds field to given value.

### HasCatalogIds

`func (o *VintedImageSearchRequest) HasCatalogIds() bool`

HasCatalogIds returns a boolean if a field has been set.

### SetCatalogIdsNil

`func (o *VintedImageSearchRequest) SetCatalogIdsNil(b bool)`

 SetCatalogIdsNil sets the value for CatalogIds to be an explicit nil

### UnsetCatalogIds
`func (o *VintedImageSearchRequest) UnsetCatalogIds()`

UnsetCatalogIds ensures that no value is present for CatalogIds, not even an explicit nil
### GetColorIds

`func (o *VintedImageSearchRequest) GetColorIds() string`

GetColorIds returns the ColorIds field if non-nil, zero value otherwise.

### GetColorIdsOk

`func (o *VintedImageSearchRequest) GetColorIdsOk() (*string, bool)`

GetColorIdsOk returns a tuple with the ColorIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColorIds

`func (o *VintedImageSearchRequest) SetColorIds(v string)`

SetColorIds sets ColorIds field to given value.

### HasColorIds

`func (o *VintedImageSearchRequest) HasColorIds() bool`

HasColorIds returns a boolean if a field has been set.

### SetColorIdsNil

`func (o *VintedImageSearchRequest) SetColorIdsNil(b bool)`

 SetColorIdsNil sets the value for ColorIds to be an explicit nil

### UnsetColorIds
`func (o *VintedImageSearchRequest) UnsetColorIds()`

UnsetColorIds ensures that no value is present for ColorIds, not even an explicit nil
### GetSizeIds

`func (o *VintedImageSearchRequest) GetSizeIds() string`

GetSizeIds returns the SizeIds field if non-nil, zero value otherwise.

### GetSizeIdsOk

`func (o *VintedImageSearchRequest) GetSizeIdsOk() (*string, bool)`

GetSizeIdsOk returns a tuple with the SizeIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSizeIds

`func (o *VintedImageSearchRequest) SetSizeIds(v string)`

SetSizeIds sets SizeIds field to given value.

### HasSizeIds

`func (o *VintedImageSearchRequest) HasSizeIds() bool`

HasSizeIds returns a boolean if a field has been set.

### SetSizeIdsNil

`func (o *VintedImageSearchRequest) SetSizeIdsNil(b bool)`

 SetSizeIdsNil sets the value for SizeIds to be an explicit nil

### UnsetSizeIds
`func (o *VintedImageSearchRequest) UnsetSizeIds()`

UnsetSizeIds ensures that no value is present for SizeIds, not even an explicit nil
### GetMaterialIds

`func (o *VintedImageSearchRequest) GetMaterialIds() string`

GetMaterialIds returns the MaterialIds field if non-nil, zero value otherwise.

### GetMaterialIdsOk

`func (o *VintedImageSearchRequest) GetMaterialIdsOk() (*string, bool)`

GetMaterialIdsOk returns a tuple with the MaterialIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaterialIds

`func (o *VintedImageSearchRequest) SetMaterialIds(v string)`

SetMaterialIds sets MaterialIds field to given value.

### HasMaterialIds

`func (o *VintedImageSearchRequest) HasMaterialIds() bool`

HasMaterialIds returns a boolean if a field has been set.

### SetMaterialIdsNil

`func (o *VintedImageSearchRequest) SetMaterialIdsNil(b bool)`

 SetMaterialIdsNil sets the value for MaterialIds to be an explicit nil

### UnsetMaterialIds
`func (o *VintedImageSearchRequest) UnsetMaterialIds()`

UnsetMaterialIds ensures that no value is present for MaterialIds, not even an explicit nil
### GetStatusIds

`func (o *VintedImageSearchRequest) GetStatusIds() string`

GetStatusIds returns the StatusIds field if non-nil, zero value otherwise.

### GetStatusIdsOk

`func (o *VintedImageSearchRequest) GetStatusIdsOk() (*string, bool)`

GetStatusIdsOk returns a tuple with the StatusIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusIds

`func (o *VintedImageSearchRequest) SetStatusIds(v string)`

SetStatusIds sets StatusIds field to given value.

### HasStatusIds

`func (o *VintedImageSearchRequest) HasStatusIds() bool`

HasStatusIds returns a boolean if a field has been set.

### SetStatusIdsNil

`func (o *VintedImageSearchRequest) SetStatusIdsNil(b bool)`

 SetStatusIdsNil sets the value for StatusIds to be an explicit nil

### UnsetStatusIds
`func (o *VintedImageSearchRequest) UnsetStatusIds()`

UnsetStatusIds ensures that no value is present for StatusIds, not even an explicit nil
### GetTime

`func (o *VintedImageSearchRequest) GetTime() int32`

GetTime returns the Time field if non-nil, zero value otherwise.

### GetTimeOk

`func (o *VintedImageSearchRequest) GetTimeOk() (*int32, bool)`

GetTimeOk returns a tuple with the Time field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTime

`func (o *VintedImageSearchRequest) SetTime(v int32)`

SetTime sets Time field to given value.

### HasTime

`func (o *VintedImageSearchRequest) HasTime() bool`

HasTime returns a boolean if a field has been set.

### SetTimeNil

`func (o *VintedImageSearchRequest) SetTimeNil(b bool)`

 SetTimeNil sets the value for Time to be an explicit nil

### UnsetTime
`func (o *VintedImageSearchRequest) UnsetTime()`

UnsetTime ensures that no value is present for Time, not even an explicit nil
### GetSearchSessionId

`func (o *VintedImageSearchRequest) GetSearchSessionId() string`

GetSearchSessionId returns the SearchSessionId field if non-nil, zero value otherwise.

### GetSearchSessionIdOk

`func (o *VintedImageSearchRequest) GetSearchSessionIdOk() (*string, bool)`

GetSearchSessionIdOk returns a tuple with the SearchSessionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSearchSessionId

`func (o *VintedImageSearchRequest) SetSearchSessionId(v string)`

SetSearchSessionId sets SearchSessionId field to given value.

### HasSearchSessionId

`func (o *VintedImageSearchRequest) HasSearchSessionId() bool`

HasSearchSessionId returns a boolean if a field has been set.

### SetSearchSessionIdNil

`func (o *VintedImageSearchRequest) SetSearchSessionIdNil(b bool)`

 SetSearchSessionIdNil sets the value for SearchSessionId to be an explicit nil

### UnsetSearchSessionId
`func (o *VintedImageSearchRequest) UnsetSearchSessionId()`

UnsetSearchSessionId ensures that no value is present for SearchSessionId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



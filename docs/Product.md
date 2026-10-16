# Product

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **int32** |  | 
**Name** | **string** |  | 
**ProductCode** | Pointer to [**Productcode**](Productcode.md) |  | [optional] 
**BrandName** | Pointer to [**Brandname**](Brandname.md) |  | [optional] 
**BrandId** | Pointer to [**Brandid**](Brandid.md) |  | [optional] 
**Colour** | Pointer to [**Colour**](Colour.md) |  | [optional] 
**ColourWayId** | Pointer to [**Colourwayid**](Colourwayid.md) |  | [optional] 
**Price** | Pointer to [**ProductPrice**](ProductPrice.md) |  | [optional] 
**Url** | Pointer to [**NullableUrl**](Url.md) |  | [optional] 
**ImageUrl** | Pointer to [**Imageurl**](Imageurl.md) |  | [optional] 
**AdditionalImageUrls** | Pointer to **[]string** |  | [optional] 
**Images** | Pointer to **[]map[string]interface{}** |  | [optional] 
**Variants** | Pointer to [**[]Variant**](Variant.md) |  | [optional] 
**IsSellingFast** | Pointer to [**Issellingfast**](Issellingfast.md) |  | [optional] 
**IsRestockingSoon** | Pointer to [**Isrestockingsoon**](Isrestockingsoon.md) |  | [optional] 
**IsInStock** | Pointer to [**Isinstock**](Isinstock.md) |  | [optional] 
**Gender** | Pointer to [**Gender**](Gender.md) |  | [optional] 
**Description** | Pointer to [**Description**](Description.md) |  | [optional] 
**Ratings** | Pointer to [**Ratings**](Ratings.md) |  | [optional] 
**Breadcrumbs** | Pointer to **[]map[string]interface{}** |  | [optional] 

## Methods

### NewProduct

`func NewProduct(id int32, name string, ) *Product`

NewProduct instantiates a new Product object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProductWithDefaults

`func NewProductWithDefaults() *Product`

NewProductWithDefaults instantiates a new Product object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Product) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Product) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Product) SetId(v int32)`

SetId sets Id field to given value.


### GetName

`func (o *Product) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Product) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Product) SetName(v string)`

SetName sets Name field to given value.


### GetProductCode

`func (o *Product) GetProductCode() Productcode`

GetProductCode returns the ProductCode field if non-nil, zero value otherwise.

### GetProductCodeOk

`func (o *Product) GetProductCodeOk() (*Productcode, bool)`

GetProductCodeOk returns a tuple with the ProductCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductCode

`func (o *Product) SetProductCode(v Productcode)`

SetProductCode sets ProductCode field to given value.

### HasProductCode

`func (o *Product) HasProductCode() bool`

HasProductCode returns a boolean if a field has been set.

### GetBrandName

`func (o *Product) GetBrandName() Brandname`

GetBrandName returns the BrandName field if non-nil, zero value otherwise.

### GetBrandNameOk

`func (o *Product) GetBrandNameOk() (*Brandname, bool)`

GetBrandNameOk returns a tuple with the BrandName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBrandName

`func (o *Product) SetBrandName(v Brandname)`

SetBrandName sets BrandName field to given value.

### HasBrandName

`func (o *Product) HasBrandName() bool`

HasBrandName returns a boolean if a field has been set.

### GetBrandId

`func (o *Product) GetBrandId() Brandid`

GetBrandId returns the BrandId field if non-nil, zero value otherwise.

### GetBrandIdOk

`func (o *Product) GetBrandIdOk() (*Brandid, bool)`

GetBrandIdOk returns a tuple with the BrandId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBrandId

`func (o *Product) SetBrandId(v Brandid)`

SetBrandId sets BrandId field to given value.

### HasBrandId

`func (o *Product) HasBrandId() bool`

HasBrandId returns a boolean if a field has been set.

### GetColour

`func (o *Product) GetColour() Colour`

GetColour returns the Colour field if non-nil, zero value otherwise.

### GetColourOk

`func (o *Product) GetColourOk() (*Colour, bool)`

GetColourOk returns a tuple with the Colour field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColour

`func (o *Product) SetColour(v Colour)`

SetColour sets Colour field to given value.

### HasColour

`func (o *Product) HasColour() bool`

HasColour returns a boolean if a field has been set.

### GetColourWayId

`func (o *Product) GetColourWayId() Colourwayid`

GetColourWayId returns the ColourWayId field if non-nil, zero value otherwise.

### GetColourWayIdOk

`func (o *Product) GetColourWayIdOk() (*Colourwayid, bool)`

GetColourWayIdOk returns a tuple with the ColourWayId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColourWayId

`func (o *Product) SetColourWayId(v Colourwayid)`

SetColourWayId sets ColourWayId field to given value.

### HasColourWayId

`func (o *Product) HasColourWayId() bool`

HasColourWayId returns a boolean if a field has been set.

### GetPrice

`func (o *Product) GetPrice() ProductPrice`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *Product) GetPriceOk() (*ProductPrice, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *Product) SetPrice(v ProductPrice)`

SetPrice sets Price field to given value.

### HasPrice

`func (o *Product) HasPrice() bool`

HasPrice returns a boolean if a field has been set.

### GetUrl

`func (o *Product) GetUrl() Url`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *Product) GetUrlOk() (*Url, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *Product) SetUrl(v Url)`

SetUrl sets Url field to given value.

### HasUrl

`func (o *Product) HasUrl() bool`

HasUrl returns a boolean if a field has been set.

### SetUrlNil

`func (o *Product) SetUrlNil(b bool)`

 SetUrlNil sets the value for Url to be an explicit nil

### UnsetUrl
`func (o *Product) UnsetUrl()`

UnsetUrl ensures that no value is present for Url, not even an explicit nil
### GetImageUrl

`func (o *Product) GetImageUrl() Imageurl`

GetImageUrl returns the ImageUrl field if non-nil, zero value otherwise.

### GetImageUrlOk

`func (o *Product) GetImageUrlOk() (*Imageurl, bool)`

GetImageUrlOk returns a tuple with the ImageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImageUrl

`func (o *Product) SetImageUrl(v Imageurl)`

SetImageUrl sets ImageUrl field to given value.

### HasImageUrl

`func (o *Product) HasImageUrl() bool`

HasImageUrl returns a boolean if a field has been set.

### GetAdditionalImageUrls

`func (o *Product) GetAdditionalImageUrls() []string`

GetAdditionalImageUrls returns the AdditionalImageUrls field if non-nil, zero value otherwise.

### GetAdditionalImageUrlsOk

`func (o *Product) GetAdditionalImageUrlsOk() (*[]string, bool)`

GetAdditionalImageUrlsOk returns a tuple with the AdditionalImageUrls field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdditionalImageUrls

`func (o *Product) SetAdditionalImageUrls(v []string)`

SetAdditionalImageUrls sets AdditionalImageUrls field to given value.

### HasAdditionalImageUrls

`func (o *Product) HasAdditionalImageUrls() bool`

HasAdditionalImageUrls returns a boolean if a field has been set.

### GetImages

`func (o *Product) GetImages() []map[string]interface{}`

GetImages returns the Images field if non-nil, zero value otherwise.

### GetImagesOk

`func (o *Product) GetImagesOk() (*[]map[string]interface{}, bool)`

GetImagesOk returns a tuple with the Images field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImages

`func (o *Product) SetImages(v []map[string]interface{})`

SetImages sets Images field to given value.

### HasImages

`func (o *Product) HasImages() bool`

HasImages returns a boolean if a field has been set.

### GetVariants

`func (o *Product) GetVariants() []Variant`

GetVariants returns the Variants field if non-nil, zero value otherwise.

### GetVariantsOk

`func (o *Product) GetVariantsOk() (*[]Variant, bool)`

GetVariantsOk returns a tuple with the Variants field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVariants

`func (o *Product) SetVariants(v []Variant)`

SetVariants sets Variants field to given value.

### HasVariants

`func (o *Product) HasVariants() bool`

HasVariants returns a boolean if a field has been set.

### GetIsSellingFast

`func (o *Product) GetIsSellingFast() Issellingfast`

GetIsSellingFast returns the IsSellingFast field if non-nil, zero value otherwise.

### GetIsSellingFastOk

`func (o *Product) GetIsSellingFastOk() (*Issellingfast, bool)`

GetIsSellingFastOk returns a tuple with the IsSellingFast field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsSellingFast

`func (o *Product) SetIsSellingFast(v Issellingfast)`

SetIsSellingFast sets IsSellingFast field to given value.

### HasIsSellingFast

`func (o *Product) HasIsSellingFast() bool`

HasIsSellingFast returns a boolean if a field has been set.

### GetIsRestockingSoon

`func (o *Product) GetIsRestockingSoon() Isrestockingsoon`

GetIsRestockingSoon returns the IsRestockingSoon field if non-nil, zero value otherwise.

### GetIsRestockingSoonOk

`func (o *Product) GetIsRestockingSoonOk() (*Isrestockingsoon, bool)`

GetIsRestockingSoonOk returns a tuple with the IsRestockingSoon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsRestockingSoon

`func (o *Product) SetIsRestockingSoon(v Isrestockingsoon)`

SetIsRestockingSoon sets IsRestockingSoon field to given value.

### HasIsRestockingSoon

`func (o *Product) HasIsRestockingSoon() bool`

HasIsRestockingSoon returns a boolean if a field has been set.

### GetIsInStock

`func (o *Product) GetIsInStock() Isinstock`

GetIsInStock returns the IsInStock field if non-nil, zero value otherwise.

### GetIsInStockOk

`func (o *Product) GetIsInStockOk() (*Isinstock, bool)`

GetIsInStockOk returns a tuple with the IsInStock field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsInStock

`func (o *Product) SetIsInStock(v Isinstock)`

SetIsInStock sets IsInStock field to given value.

### HasIsInStock

`func (o *Product) HasIsInStock() bool`

HasIsInStock returns a boolean if a field has been set.

### GetGender

`func (o *Product) GetGender() Gender`

GetGender returns the Gender field if non-nil, zero value otherwise.

### GetGenderOk

`func (o *Product) GetGenderOk() (*Gender, bool)`

GetGenderOk returns a tuple with the Gender field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGender

`func (o *Product) SetGender(v Gender)`

SetGender sets Gender field to given value.

### HasGender

`func (o *Product) HasGender() bool`

HasGender returns a boolean if a field has been set.

### GetDescription

`func (o *Product) GetDescription() Description`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *Product) GetDescriptionOk() (*Description, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *Product) SetDescription(v Description)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *Product) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetRatings

`func (o *Product) GetRatings() Ratings`

GetRatings returns the Ratings field if non-nil, zero value otherwise.

### GetRatingsOk

`func (o *Product) GetRatingsOk() (*Ratings, bool)`

GetRatingsOk returns a tuple with the Ratings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRatings

`func (o *Product) SetRatings(v Ratings)`

SetRatings sets Ratings field to given value.

### HasRatings

`func (o *Product) HasRatings() bool`

HasRatings returns a boolean if a field has been set.

### GetBreadcrumbs

`func (o *Product) GetBreadcrumbs() []map[string]interface{}`

GetBreadcrumbs returns the Breadcrumbs field if non-nil, zero value otherwise.

### GetBreadcrumbsOk

`func (o *Product) GetBreadcrumbsOk() (*[]map[string]interface{}, bool)`

GetBreadcrumbsOk returns a tuple with the Breadcrumbs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBreadcrumbs

`func (o *Product) SetBreadcrumbs(v []map[string]interface{})`

SetBreadcrumbs sets Breadcrumbs field to given value.

### HasBreadcrumbs

`func (o *Product) HasBreadcrumbs() bool`

HasBreadcrumbs returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



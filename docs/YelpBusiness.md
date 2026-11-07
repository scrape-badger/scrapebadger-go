# YelpBusiness

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Position** | **int32** | 1-based place in Yelp&#39;s organic order across pages (page 2 starts at 11): Yelp&#39;s own number where it numbers the results; services searches are unnumbered and keep Yelp&#39;s order. For ads, the slot order. | 
**IsAd** | **bool** |  | 
**Id** | **string** | Yelp encrypted business ID. | 
**Alias** | **string** | Business slug used in /biz/&lt;alias&gt;. | 
**Name** | **string** |  | 
**Url** | **string** |  | 
**Rating** | Pointer to **NullableFloat32** |  | [optional] 
**ReviewCount** | Pointer to **NullableInt32** |  | [optional] 
**Price** | Pointer to **NullableString** |  | [optional] 
**PriceLevel** | Pointer to **NullableInt32** |  | [optional] 
**Categories** | Pointer to [**[]YelpCategory**](YelpCategory.md) |  | [optional] 
**Neighborhoods** | Pointer to **[]string** |  | [optional] 
**Address** | Pointer to **NullableString** |  | [optional] 
**City** | Pointer to **NullableString** |  | [optional] 
**Phone** | Pointer to **NullableString** |  | [optional] 
**Timezone** | Pointer to **NullableString** |  | [optional] 
**OpeningHours** | Pointer to [**[]YelpHours**](YelpHours.md) |  | [optional] 
**Snippet** | Pointer to **NullableString** |  | [optional] 
**SnippetType** | Pointer to **NullableString** |  | [optional] 
**Highlights** | Pointer to **[]string** |  | [optional] 
**Tags** | Pointer to **[]string** |  | [optional] 
**Photos** | Pointer to **[]string** |  | [optional] 
**AlternateNames** | Pointer to **[]string** |  | [optional] 
**IsServiceAreaBusiness** | Pointer to **NullableBool** |  | [optional] 
**IsYelpGuaranteed** | Pointer to **NullableBool** |  | [optional] 
**HasVerifiedLicense** | Pointer to **NullableBool** |  | [optional] 
**AdPlacement** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewYelpBusiness

`func NewYelpBusiness(position int32, isAd bool, id string, alias string, name string, url string, ) *YelpBusiness`

NewYelpBusiness instantiates a new YelpBusiness object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewYelpBusinessWithDefaults

`func NewYelpBusinessWithDefaults() *YelpBusiness`

NewYelpBusinessWithDefaults instantiates a new YelpBusiness object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPosition

`func (o *YelpBusiness) GetPosition() int32`

GetPosition returns the Position field if non-nil, zero value otherwise.

### GetPositionOk

`func (o *YelpBusiness) GetPositionOk() (*int32, bool)`

GetPositionOk returns a tuple with the Position field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPosition

`func (o *YelpBusiness) SetPosition(v int32)`

SetPosition sets Position field to given value.


### GetIsAd

`func (o *YelpBusiness) GetIsAd() bool`

GetIsAd returns the IsAd field if non-nil, zero value otherwise.

### GetIsAdOk

`func (o *YelpBusiness) GetIsAdOk() (*bool, bool)`

GetIsAdOk returns a tuple with the IsAd field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsAd

`func (o *YelpBusiness) SetIsAd(v bool)`

SetIsAd sets IsAd field to given value.


### GetId

`func (o *YelpBusiness) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *YelpBusiness) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *YelpBusiness) SetId(v string)`

SetId sets Id field to given value.


### GetAlias

`func (o *YelpBusiness) GetAlias() string`

GetAlias returns the Alias field if non-nil, zero value otherwise.

### GetAliasOk

`func (o *YelpBusiness) GetAliasOk() (*string, bool)`

GetAliasOk returns a tuple with the Alias field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAlias

`func (o *YelpBusiness) SetAlias(v string)`

SetAlias sets Alias field to given value.


### GetName

`func (o *YelpBusiness) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *YelpBusiness) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *YelpBusiness) SetName(v string)`

SetName sets Name field to given value.


### GetUrl

`func (o *YelpBusiness) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *YelpBusiness) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *YelpBusiness) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetRating

`func (o *YelpBusiness) GetRating() float32`

GetRating returns the Rating field if non-nil, zero value otherwise.

### GetRatingOk

`func (o *YelpBusiness) GetRatingOk() (*float32, bool)`

GetRatingOk returns a tuple with the Rating field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRating

`func (o *YelpBusiness) SetRating(v float32)`

SetRating sets Rating field to given value.

### HasRating

`func (o *YelpBusiness) HasRating() bool`

HasRating returns a boolean if a field has been set.

### SetRatingNil

`func (o *YelpBusiness) SetRatingNil(b bool)`

 SetRatingNil sets the value for Rating to be an explicit nil

### UnsetRating
`func (o *YelpBusiness) UnsetRating()`

UnsetRating ensures that no value is present for Rating, not even an explicit nil
### GetReviewCount

`func (o *YelpBusiness) GetReviewCount() int32`

GetReviewCount returns the ReviewCount field if non-nil, zero value otherwise.

### GetReviewCountOk

`func (o *YelpBusiness) GetReviewCountOk() (*int32, bool)`

GetReviewCountOk returns a tuple with the ReviewCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReviewCount

`func (o *YelpBusiness) SetReviewCount(v int32)`

SetReviewCount sets ReviewCount field to given value.

### HasReviewCount

`func (o *YelpBusiness) HasReviewCount() bool`

HasReviewCount returns a boolean if a field has been set.

### SetReviewCountNil

`func (o *YelpBusiness) SetReviewCountNil(b bool)`

 SetReviewCountNil sets the value for ReviewCount to be an explicit nil

### UnsetReviewCount
`func (o *YelpBusiness) UnsetReviewCount()`

UnsetReviewCount ensures that no value is present for ReviewCount, not even an explicit nil
### GetPrice

`func (o *YelpBusiness) GetPrice() string`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *YelpBusiness) GetPriceOk() (*string, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *YelpBusiness) SetPrice(v string)`

SetPrice sets Price field to given value.

### HasPrice

`func (o *YelpBusiness) HasPrice() bool`

HasPrice returns a boolean if a field has been set.

### SetPriceNil

`func (o *YelpBusiness) SetPriceNil(b bool)`

 SetPriceNil sets the value for Price to be an explicit nil

### UnsetPrice
`func (o *YelpBusiness) UnsetPrice()`

UnsetPrice ensures that no value is present for Price, not even an explicit nil
### GetPriceLevel

`func (o *YelpBusiness) GetPriceLevel() int32`

GetPriceLevel returns the PriceLevel field if non-nil, zero value otherwise.

### GetPriceLevelOk

`func (o *YelpBusiness) GetPriceLevelOk() (*int32, bool)`

GetPriceLevelOk returns a tuple with the PriceLevel field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceLevel

`func (o *YelpBusiness) SetPriceLevel(v int32)`

SetPriceLevel sets PriceLevel field to given value.

### HasPriceLevel

`func (o *YelpBusiness) HasPriceLevel() bool`

HasPriceLevel returns a boolean if a field has been set.

### SetPriceLevelNil

`func (o *YelpBusiness) SetPriceLevelNil(b bool)`

 SetPriceLevelNil sets the value for PriceLevel to be an explicit nil

### UnsetPriceLevel
`func (o *YelpBusiness) UnsetPriceLevel()`

UnsetPriceLevel ensures that no value is present for PriceLevel, not even an explicit nil
### GetCategories

`func (o *YelpBusiness) GetCategories() []YelpCategory`

GetCategories returns the Categories field if non-nil, zero value otherwise.

### GetCategoriesOk

`func (o *YelpBusiness) GetCategoriesOk() (*[]YelpCategory, bool)`

GetCategoriesOk returns a tuple with the Categories field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategories

`func (o *YelpBusiness) SetCategories(v []YelpCategory)`

SetCategories sets Categories field to given value.

### HasCategories

`func (o *YelpBusiness) HasCategories() bool`

HasCategories returns a boolean if a field has been set.

### GetNeighborhoods

`func (o *YelpBusiness) GetNeighborhoods() []string`

GetNeighborhoods returns the Neighborhoods field if non-nil, zero value otherwise.

### GetNeighborhoodsOk

`func (o *YelpBusiness) GetNeighborhoodsOk() (*[]string, bool)`

GetNeighborhoodsOk returns a tuple with the Neighborhoods field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNeighborhoods

`func (o *YelpBusiness) SetNeighborhoods(v []string)`

SetNeighborhoods sets Neighborhoods field to given value.

### HasNeighborhoods

`func (o *YelpBusiness) HasNeighborhoods() bool`

HasNeighborhoods returns a boolean if a field has been set.

### GetAddress

`func (o *YelpBusiness) GetAddress() string`

GetAddress returns the Address field if non-nil, zero value otherwise.

### GetAddressOk

`func (o *YelpBusiness) GetAddressOk() (*string, bool)`

GetAddressOk returns a tuple with the Address field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddress

`func (o *YelpBusiness) SetAddress(v string)`

SetAddress sets Address field to given value.

### HasAddress

`func (o *YelpBusiness) HasAddress() bool`

HasAddress returns a boolean if a field has been set.

### SetAddressNil

`func (o *YelpBusiness) SetAddressNil(b bool)`

 SetAddressNil sets the value for Address to be an explicit nil

### UnsetAddress
`func (o *YelpBusiness) UnsetAddress()`

UnsetAddress ensures that no value is present for Address, not even an explicit nil
### GetCity

`func (o *YelpBusiness) GetCity() string`

GetCity returns the City field if non-nil, zero value otherwise.

### GetCityOk

`func (o *YelpBusiness) GetCityOk() (*string, bool)`

GetCityOk returns a tuple with the City field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCity

`func (o *YelpBusiness) SetCity(v string)`

SetCity sets City field to given value.

### HasCity

`func (o *YelpBusiness) HasCity() bool`

HasCity returns a boolean if a field has been set.

### SetCityNil

`func (o *YelpBusiness) SetCityNil(b bool)`

 SetCityNil sets the value for City to be an explicit nil

### UnsetCity
`func (o *YelpBusiness) UnsetCity()`

UnsetCity ensures that no value is present for City, not even an explicit nil
### GetPhone

`func (o *YelpBusiness) GetPhone() string`

GetPhone returns the Phone field if non-nil, zero value otherwise.

### GetPhoneOk

`func (o *YelpBusiness) GetPhoneOk() (*string, bool)`

GetPhoneOk returns a tuple with the Phone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhone

`func (o *YelpBusiness) SetPhone(v string)`

SetPhone sets Phone field to given value.

### HasPhone

`func (o *YelpBusiness) HasPhone() bool`

HasPhone returns a boolean if a field has been set.

### SetPhoneNil

`func (o *YelpBusiness) SetPhoneNil(b bool)`

 SetPhoneNil sets the value for Phone to be an explicit nil

### UnsetPhone
`func (o *YelpBusiness) UnsetPhone()`

UnsetPhone ensures that no value is present for Phone, not even an explicit nil
### GetTimezone

`func (o *YelpBusiness) GetTimezone() string`

GetTimezone returns the Timezone field if non-nil, zero value otherwise.

### GetTimezoneOk

`func (o *YelpBusiness) GetTimezoneOk() (*string, bool)`

GetTimezoneOk returns a tuple with the Timezone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimezone

`func (o *YelpBusiness) SetTimezone(v string)`

SetTimezone sets Timezone field to given value.

### HasTimezone

`func (o *YelpBusiness) HasTimezone() bool`

HasTimezone returns a boolean if a field has been set.

### SetTimezoneNil

`func (o *YelpBusiness) SetTimezoneNil(b bool)`

 SetTimezoneNil sets the value for Timezone to be an explicit nil

### UnsetTimezone
`func (o *YelpBusiness) UnsetTimezone()`

UnsetTimezone ensures that no value is present for Timezone, not even an explicit nil
### GetOpeningHours

`func (o *YelpBusiness) GetOpeningHours() []YelpHours`

GetOpeningHours returns the OpeningHours field if non-nil, zero value otherwise.

### GetOpeningHoursOk

`func (o *YelpBusiness) GetOpeningHoursOk() (*[]YelpHours, bool)`

GetOpeningHoursOk returns a tuple with the OpeningHours field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOpeningHours

`func (o *YelpBusiness) SetOpeningHours(v []YelpHours)`

SetOpeningHours sets OpeningHours field to given value.

### HasOpeningHours

`func (o *YelpBusiness) HasOpeningHours() bool`

HasOpeningHours returns a boolean if a field has been set.

### GetSnippet

`func (o *YelpBusiness) GetSnippet() string`

GetSnippet returns the Snippet field if non-nil, zero value otherwise.

### GetSnippetOk

`func (o *YelpBusiness) GetSnippetOk() (*string, bool)`

GetSnippetOk returns a tuple with the Snippet field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSnippet

`func (o *YelpBusiness) SetSnippet(v string)`

SetSnippet sets Snippet field to given value.

### HasSnippet

`func (o *YelpBusiness) HasSnippet() bool`

HasSnippet returns a boolean if a field has been set.

### SetSnippetNil

`func (o *YelpBusiness) SetSnippetNil(b bool)`

 SetSnippetNil sets the value for Snippet to be an explicit nil

### UnsetSnippet
`func (o *YelpBusiness) UnsetSnippet()`

UnsetSnippet ensures that no value is present for Snippet, not even an explicit nil
### GetSnippetType

`func (o *YelpBusiness) GetSnippetType() string`

GetSnippetType returns the SnippetType field if non-nil, zero value otherwise.

### GetSnippetTypeOk

`func (o *YelpBusiness) GetSnippetTypeOk() (*string, bool)`

GetSnippetTypeOk returns a tuple with the SnippetType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSnippetType

`func (o *YelpBusiness) SetSnippetType(v string)`

SetSnippetType sets SnippetType field to given value.

### HasSnippetType

`func (o *YelpBusiness) HasSnippetType() bool`

HasSnippetType returns a boolean if a field has been set.

### SetSnippetTypeNil

`func (o *YelpBusiness) SetSnippetTypeNil(b bool)`

 SetSnippetTypeNil sets the value for SnippetType to be an explicit nil

### UnsetSnippetType
`func (o *YelpBusiness) UnsetSnippetType()`

UnsetSnippetType ensures that no value is present for SnippetType, not even an explicit nil
### GetHighlights

`func (o *YelpBusiness) GetHighlights() []string`

GetHighlights returns the Highlights field if non-nil, zero value otherwise.

### GetHighlightsOk

`func (o *YelpBusiness) GetHighlightsOk() (*[]string, bool)`

GetHighlightsOk returns a tuple with the Highlights field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHighlights

`func (o *YelpBusiness) SetHighlights(v []string)`

SetHighlights sets Highlights field to given value.

### HasHighlights

`func (o *YelpBusiness) HasHighlights() bool`

HasHighlights returns a boolean if a field has been set.

### GetTags

`func (o *YelpBusiness) GetTags() []string`

GetTags returns the Tags field if non-nil, zero value otherwise.

### GetTagsOk

`func (o *YelpBusiness) GetTagsOk() (*[]string, bool)`

GetTagsOk returns a tuple with the Tags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTags

`func (o *YelpBusiness) SetTags(v []string)`

SetTags sets Tags field to given value.

### HasTags

`func (o *YelpBusiness) HasTags() bool`

HasTags returns a boolean if a field has been set.

### GetPhotos

`func (o *YelpBusiness) GetPhotos() []string`

GetPhotos returns the Photos field if non-nil, zero value otherwise.

### GetPhotosOk

`func (o *YelpBusiness) GetPhotosOk() (*[]string, bool)`

GetPhotosOk returns a tuple with the Photos field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhotos

`func (o *YelpBusiness) SetPhotos(v []string)`

SetPhotos sets Photos field to given value.

### HasPhotos

`func (o *YelpBusiness) HasPhotos() bool`

HasPhotos returns a boolean if a field has been set.

### GetAlternateNames

`func (o *YelpBusiness) GetAlternateNames() []string`

GetAlternateNames returns the AlternateNames field if non-nil, zero value otherwise.

### GetAlternateNamesOk

`func (o *YelpBusiness) GetAlternateNamesOk() (*[]string, bool)`

GetAlternateNamesOk returns a tuple with the AlternateNames field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAlternateNames

`func (o *YelpBusiness) SetAlternateNames(v []string)`

SetAlternateNames sets AlternateNames field to given value.

### HasAlternateNames

`func (o *YelpBusiness) HasAlternateNames() bool`

HasAlternateNames returns a boolean if a field has been set.

### GetIsServiceAreaBusiness

`func (o *YelpBusiness) GetIsServiceAreaBusiness() bool`

GetIsServiceAreaBusiness returns the IsServiceAreaBusiness field if non-nil, zero value otherwise.

### GetIsServiceAreaBusinessOk

`func (o *YelpBusiness) GetIsServiceAreaBusinessOk() (*bool, bool)`

GetIsServiceAreaBusinessOk returns a tuple with the IsServiceAreaBusiness field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsServiceAreaBusiness

`func (o *YelpBusiness) SetIsServiceAreaBusiness(v bool)`

SetIsServiceAreaBusiness sets IsServiceAreaBusiness field to given value.

### HasIsServiceAreaBusiness

`func (o *YelpBusiness) HasIsServiceAreaBusiness() bool`

HasIsServiceAreaBusiness returns a boolean if a field has been set.

### SetIsServiceAreaBusinessNil

`func (o *YelpBusiness) SetIsServiceAreaBusinessNil(b bool)`

 SetIsServiceAreaBusinessNil sets the value for IsServiceAreaBusiness to be an explicit nil

### UnsetIsServiceAreaBusiness
`func (o *YelpBusiness) UnsetIsServiceAreaBusiness()`

UnsetIsServiceAreaBusiness ensures that no value is present for IsServiceAreaBusiness, not even an explicit nil
### GetIsYelpGuaranteed

`func (o *YelpBusiness) GetIsYelpGuaranteed() bool`

GetIsYelpGuaranteed returns the IsYelpGuaranteed field if non-nil, zero value otherwise.

### GetIsYelpGuaranteedOk

`func (o *YelpBusiness) GetIsYelpGuaranteedOk() (*bool, bool)`

GetIsYelpGuaranteedOk returns a tuple with the IsYelpGuaranteed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsYelpGuaranteed

`func (o *YelpBusiness) SetIsYelpGuaranteed(v bool)`

SetIsYelpGuaranteed sets IsYelpGuaranteed field to given value.

### HasIsYelpGuaranteed

`func (o *YelpBusiness) HasIsYelpGuaranteed() bool`

HasIsYelpGuaranteed returns a boolean if a field has been set.

### SetIsYelpGuaranteedNil

`func (o *YelpBusiness) SetIsYelpGuaranteedNil(b bool)`

 SetIsYelpGuaranteedNil sets the value for IsYelpGuaranteed to be an explicit nil

### UnsetIsYelpGuaranteed
`func (o *YelpBusiness) UnsetIsYelpGuaranteed()`

UnsetIsYelpGuaranteed ensures that no value is present for IsYelpGuaranteed, not even an explicit nil
### GetHasVerifiedLicense

`func (o *YelpBusiness) GetHasVerifiedLicense() bool`

GetHasVerifiedLicense returns the HasVerifiedLicense field if non-nil, zero value otherwise.

### GetHasVerifiedLicenseOk

`func (o *YelpBusiness) GetHasVerifiedLicenseOk() (*bool, bool)`

GetHasVerifiedLicenseOk returns a tuple with the HasVerifiedLicense field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasVerifiedLicense

`func (o *YelpBusiness) SetHasVerifiedLicense(v bool)`

SetHasVerifiedLicense sets HasVerifiedLicense field to given value.

### HasHasVerifiedLicense

`func (o *YelpBusiness) HasHasVerifiedLicense() bool`

HasHasVerifiedLicense returns a boolean if a field has been set.

### SetHasVerifiedLicenseNil

`func (o *YelpBusiness) SetHasVerifiedLicenseNil(b bool)`

 SetHasVerifiedLicenseNil sets the value for HasVerifiedLicense to be an explicit nil

### UnsetHasVerifiedLicense
`func (o *YelpBusiness) UnsetHasVerifiedLicense()`

UnsetHasVerifiedLicense ensures that no value is present for HasVerifiedLicense, not even an explicit nil
### GetAdPlacement

`func (o *YelpBusiness) GetAdPlacement() string`

GetAdPlacement returns the AdPlacement field if non-nil, zero value otherwise.

### GetAdPlacementOk

`func (o *YelpBusiness) GetAdPlacementOk() (*string, bool)`

GetAdPlacementOk returns a tuple with the AdPlacement field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdPlacement

`func (o *YelpBusiness) SetAdPlacement(v string)`

SetAdPlacement sets AdPlacement field to given value.

### HasAdPlacement

`func (o *YelpBusiness) HasAdPlacement() bool`

HasAdPlacement returns a boolean if a field has been set.

### SetAdPlacementNil

`func (o *YelpBusiness) SetAdPlacementNil(b bool)`

 SetAdPlacementNil sets the value for AdPlacement to be an explicit nil

### UnsetAdPlacement
`func (o *YelpBusiness) UnsetAdPlacement()`

UnsetAdPlacement ensures that no value is present for AdPlacement, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



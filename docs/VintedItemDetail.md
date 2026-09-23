# VintedItemDetail

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **int32** |  | 
**Title** | **string** |  | 
**Price** | [**VintedPrice**](VintedPrice.md) |  | 
**BrandTitle** | Pointer to **NullableString** |  | [optional] 
**DisplayTitle** | Pointer to **NullableString** |  | [optional] 
**DisplaySubtitle** | Pointer to **NullableString** |  | [optional] 
**SizeTitle** | Pointer to **NullableString** |  | [optional] 
**Status** | Pointer to **NullableString** |  | [optional] 
**Url** | **string** |  | 
**Path** | Pointer to **NullableString** |  | [optional] 
**IsVisible** | Pointer to **bool** |  | [optional] [default to true]
**Promoted** | Pointer to **bool** |  | [optional] [default to false]
**FavouriteCount** | Pointer to **int32** |  | [optional] [default to 0]
**ViewCount** | Pointer to **int32** |  | [optional] [default to 0]
**ServiceFee** | Pointer to **NullableString** |  | [optional] 
**TotalItemPrice** | Pointer to **NullableString** |  | [optional] 
**ContentSource** | Pointer to **NullableString** |  | [optional] 
**SellerCountryCode** | Pointer to **NullableString** |  | [optional] 
**SimilarityScore** | Pointer to **NullableFloat32** |  | [optional] 
**User** | Pointer to [**NullableVintedUserSummary**](VintedUserSummary.md) |  | [optional] 
**Photo** | Pointer to [**NullableVintedPhoto**](VintedPhoto.md) |  | [optional] 
**Photos** | Pointer to [**[]VintedPhoto**](VintedPhoto.md) |  | [optional] 
**Description** | Pointer to **NullableString** |  | [optional] 
**CatalogId** | Pointer to **NullableInt32** |  | [optional] 
**Color1** | Pointer to **NullableString** |  | [optional] 
**Color2** | Pointer to **NullableString** |  | [optional] 
**PackageSizeId** | Pointer to **NullableInt32** |  | [optional] 
**IsFavourite** | Pointer to **bool** |  | [optional] [default to false]
**CanBuy** | Pointer to **bool** |  | [optional] [default to true]
**CanBundle** | Pointer to **bool** |  | [optional] [default to false]
**CanReserve** | Pointer to **bool** |  | [optional] [default to false]
**InstantBuy** | Pointer to **bool** |  | [optional] [default to false]
**IsHidden** | Pointer to **bool** |  | [optional] [default to false]
**IsReserved** | Pointer to **bool** |  | [optional] [default to false]
**IsClosed** | Pointer to **bool** |  | [optional] [default to false]
**Seller** | Pointer to [**NullableVintedSellerSummary**](VintedSellerSummary.md) |  | [optional] 
**SizeId** | Pointer to **NullableInt32** |  | [optional] 
**StatusId** | Pointer to **NullableInt32** |  | [optional] 
**BrandId** | Pointer to **NullableInt32** |  | [optional] 
**Category** | Pointer to **[]string** |  | [optional] 
**UploadDate** | Pointer to **NullableString** |  | [optional] 
**UploadedAt** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewVintedItemDetail

`func NewVintedItemDetail(id int32, title string, price VintedPrice, url string, ) *VintedItemDetail`

NewVintedItemDetail instantiates a new VintedItemDetail object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVintedItemDetailWithDefaults

`func NewVintedItemDetailWithDefaults() *VintedItemDetail`

NewVintedItemDetailWithDefaults instantiates a new VintedItemDetail object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *VintedItemDetail) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *VintedItemDetail) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *VintedItemDetail) SetId(v int32)`

SetId sets Id field to given value.


### GetTitle

`func (o *VintedItemDetail) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *VintedItemDetail) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *VintedItemDetail) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetPrice

`func (o *VintedItemDetail) GetPrice() VintedPrice`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *VintedItemDetail) GetPriceOk() (*VintedPrice, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *VintedItemDetail) SetPrice(v VintedPrice)`

SetPrice sets Price field to given value.


### GetBrandTitle

`func (o *VintedItemDetail) GetBrandTitle() string`

GetBrandTitle returns the BrandTitle field if non-nil, zero value otherwise.

### GetBrandTitleOk

`func (o *VintedItemDetail) GetBrandTitleOk() (*string, bool)`

GetBrandTitleOk returns a tuple with the BrandTitle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBrandTitle

`func (o *VintedItemDetail) SetBrandTitle(v string)`

SetBrandTitle sets BrandTitle field to given value.

### HasBrandTitle

`func (o *VintedItemDetail) HasBrandTitle() bool`

HasBrandTitle returns a boolean if a field has been set.

### SetBrandTitleNil

`func (o *VintedItemDetail) SetBrandTitleNil(b bool)`

 SetBrandTitleNil sets the value for BrandTitle to be an explicit nil

### UnsetBrandTitle
`func (o *VintedItemDetail) UnsetBrandTitle()`

UnsetBrandTitle ensures that no value is present for BrandTitle, not even an explicit nil
### GetDisplayTitle

`func (o *VintedItemDetail) GetDisplayTitle() string`

GetDisplayTitle returns the DisplayTitle field if non-nil, zero value otherwise.

### GetDisplayTitleOk

`func (o *VintedItemDetail) GetDisplayTitleOk() (*string, bool)`

GetDisplayTitleOk returns a tuple with the DisplayTitle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayTitle

`func (o *VintedItemDetail) SetDisplayTitle(v string)`

SetDisplayTitle sets DisplayTitle field to given value.

### HasDisplayTitle

`func (o *VintedItemDetail) HasDisplayTitle() bool`

HasDisplayTitle returns a boolean if a field has been set.

### SetDisplayTitleNil

`func (o *VintedItemDetail) SetDisplayTitleNil(b bool)`

 SetDisplayTitleNil sets the value for DisplayTitle to be an explicit nil

### UnsetDisplayTitle
`func (o *VintedItemDetail) UnsetDisplayTitle()`

UnsetDisplayTitle ensures that no value is present for DisplayTitle, not even an explicit nil
### GetDisplaySubtitle

`func (o *VintedItemDetail) GetDisplaySubtitle() string`

GetDisplaySubtitle returns the DisplaySubtitle field if non-nil, zero value otherwise.

### GetDisplaySubtitleOk

`func (o *VintedItemDetail) GetDisplaySubtitleOk() (*string, bool)`

GetDisplaySubtitleOk returns a tuple with the DisplaySubtitle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplaySubtitle

`func (o *VintedItemDetail) SetDisplaySubtitle(v string)`

SetDisplaySubtitle sets DisplaySubtitle field to given value.

### HasDisplaySubtitle

`func (o *VintedItemDetail) HasDisplaySubtitle() bool`

HasDisplaySubtitle returns a boolean if a field has been set.

### SetDisplaySubtitleNil

`func (o *VintedItemDetail) SetDisplaySubtitleNil(b bool)`

 SetDisplaySubtitleNil sets the value for DisplaySubtitle to be an explicit nil

### UnsetDisplaySubtitle
`func (o *VintedItemDetail) UnsetDisplaySubtitle()`

UnsetDisplaySubtitle ensures that no value is present for DisplaySubtitle, not even an explicit nil
### GetSizeTitle

`func (o *VintedItemDetail) GetSizeTitle() string`

GetSizeTitle returns the SizeTitle field if non-nil, zero value otherwise.

### GetSizeTitleOk

`func (o *VintedItemDetail) GetSizeTitleOk() (*string, bool)`

GetSizeTitleOk returns a tuple with the SizeTitle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSizeTitle

`func (o *VintedItemDetail) SetSizeTitle(v string)`

SetSizeTitle sets SizeTitle field to given value.

### HasSizeTitle

`func (o *VintedItemDetail) HasSizeTitle() bool`

HasSizeTitle returns a boolean if a field has been set.

### SetSizeTitleNil

`func (o *VintedItemDetail) SetSizeTitleNil(b bool)`

 SetSizeTitleNil sets the value for SizeTitle to be an explicit nil

### UnsetSizeTitle
`func (o *VintedItemDetail) UnsetSizeTitle()`

UnsetSizeTitle ensures that no value is present for SizeTitle, not even an explicit nil
### GetStatus

`func (o *VintedItemDetail) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *VintedItemDetail) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *VintedItemDetail) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *VintedItemDetail) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### SetStatusNil

`func (o *VintedItemDetail) SetStatusNil(b bool)`

 SetStatusNil sets the value for Status to be an explicit nil

### UnsetStatus
`func (o *VintedItemDetail) UnsetStatus()`

UnsetStatus ensures that no value is present for Status, not even an explicit nil
### GetUrl

`func (o *VintedItemDetail) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *VintedItemDetail) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *VintedItemDetail) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetPath

`func (o *VintedItemDetail) GetPath() string`

GetPath returns the Path field if non-nil, zero value otherwise.

### GetPathOk

`func (o *VintedItemDetail) GetPathOk() (*string, bool)`

GetPathOk returns a tuple with the Path field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPath

`func (o *VintedItemDetail) SetPath(v string)`

SetPath sets Path field to given value.

### HasPath

`func (o *VintedItemDetail) HasPath() bool`

HasPath returns a boolean if a field has been set.

### SetPathNil

`func (o *VintedItemDetail) SetPathNil(b bool)`

 SetPathNil sets the value for Path to be an explicit nil

### UnsetPath
`func (o *VintedItemDetail) UnsetPath()`

UnsetPath ensures that no value is present for Path, not even an explicit nil
### GetIsVisible

`func (o *VintedItemDetail) GetIsVisible() bool`

GetIsVisible returns the IsVisible field if non-nil, zero value otherwise.

### GetIsVisibleOk

`func (o *VintedItemDetail) GetIsVisibleOk() (*bool, bool)`

GetIsVisibleOk returns a tuple with the IsVisible field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsVisible

`func (o *VintedItemDetail) SetIsVisible(v bool)`

SetIsVisible sets IsVisible field to given value.

### HasIsVisible

`func (o *VintedItemDetail) HasIsVisible() bool`

HasIsVisible returns a boolean if a field has been set.

### GetPromoted

`func (o *VintedItemDetail) GetPromoted() bool`

GetPromoted returns the Promoted field if non-nil, zero value otherwise.

### GetPromotedOk

`func (o *VintedItemDetail) GetPromotedOk() (*bool, bool)`

GetPromotedOk returns a tuple with the Promoted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPromoted

`func (o *VintedItemDetail) SetPromoted(v bool)`

SetPromoted sets Promoted field to given value.

### HasPromoted

`func (o *VintedItemDetail) HasPromoted() bool`

HasPromoted returns a boolean if a field has been set.

### GetFavouriteCount

`func (o *VintedItemDetail) GetFavouriteCount() int32`

GetFavouriteCount returns the FavouriteCount field if non-nil, zero value otherwise.

### GetFavouriteCountOk

`func (o *VintedItemDetail) GetFavouriteCountOk() (*int32, bool)`

GetFavouriteCountOk returns a tuple with the FavouriteCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFavouriteCount

`func (o *VintedItemDetail) SetFavouriteCount(v int32)`

SetFavouriteCount sets FavouriteCount field to given value.

### HasFavouriteCount

`func (o *VintedItemDetail) HasFavouriteCount() bool`

HasFavouriteCount returns a boolean if a field has been set.

### GetViewCount

`func (o *VintedItemDetail) GetViewCount() int32`

GetViewCount returns the ViewCount field if non-nil, zero value otherwise.

### GetViewCountOk

`func (o *VintedItemDetail) GetViewCountOk() (*int32, bool)`

GetViewCountOk returns a tuple with the ViewCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetViewCount

`func (o *VintedItemDetail) SetViewCount(v int32)`

SetViewCount sets ViewCount field to given value.

### HasViewCount

`func (o *VintedItemDetail) HasViewCount() bool`

HasViewCount returns a boolean if a field has been set.

### GetServiceFee

`func (o *VintedItemDetail) GetServiceFee() string`

GetServiceFee returns the ServiceFee field if non-nil, zero value otherwise.

### GetServiceFeeOk

`func (o *VintedItemDetail) GetServiceFeeOk() (*string, bool)`

GetServiceFeeOk returns a tuple with the ServiceFee field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetServiceFee

`func (o *VintedItemDetail) SetServiceFee(v string)`

SetServiceFee sets ServiceFee field to given value.

### HasServiceFee

`func (o *VintedItemDetail) HasServiceFee() bool`

HasServiceFee returns a boolean if a field has been set.

### SetServiceFeeNil

`func (o *VintedItemDetail) SetServiceFeeNil(b bool)`

 SetServiceFeeNil sets the value for ServiceFee to be an explicit nil

### UnsetServiceFee
`func (o *VintedItemDetail) UnsetServiceFee()`

UnsetServiceFee ensures that no value is present for ServiceFee, not even an explicit nil
### GetTotalItemPrice

`func (o *VintedItemDetail) GetTotalItemPrice() string`

GetTotalItemPrice returns the TotalItemPrice field if non-nil, zero value otherwise.

### GetTotalItemPriceOk

`func (o *VintedItemDetail) GetTotalItemPriceOk() (*string, bool)`

GetTotalItemPriceOk returns a tuple with the TotalItemPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalItemPrice

`func (o *VintedItemDetail) SetTotalItemPrice(v string)`

SetTotalItemPrice sets TotalItemPrice field to given value.

### HasTotalItemPrice

`func (o *VintedItemDetail) HasTotalItemPrice() bool`

HasTotalItemPrice returns a boolean if a field has been set.

### SetTotalItemPriceNil

`func (o *VintedItemDetail) SetTotalItemPriceNil(b bool)`

 SetTotalItemPriceNil sets the value for TotalItemPrice to be an explicit nil

### UnsetTotalItemPrice
`func (o *VintedItemDetail) UnsetTotalItemPrice()`

UnsetTotalItemPrice ensures that no value is present for TotalItemPrice, not even an explicit nil
### GetContentSource

`func (o *VintedItemDetail) GetContentSource() string`

GetContentSource returns the ContentSource field if non-nil, zero value otherwise.

### GetContentSourceOk

`func (o *VintedItemDetail) GetContentSourceOk() (*string, bool)`

GetContentSourceOk returns a tuple with the ContentSource field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContentSource

`func (o *VintedItemDetail) SetContentSource(v string)`

SetContentSource sets ContentSource field to given value.

### HasContentSource

`func (o *VintedItemDetail) HasContentSource() bool`

HasContentSource returns a boolean if a field has been set.

### SetContentSourceNil

`func (o *VintedItemDetail) SetContentSourceNil(b bool)`

 SetContentSourceNil sets the value for ContentSource to be an explicit nil

### UnsetContentSource
`func (o *VintedItemDetail) UnsetContentSource()`

UnsetContentSource ensures that no value is present for ContentSource, not even an explicit nil
### GetSellerCountryCode

`func (o *VintedItemDetail) GetSellerCountryCode() string`

GetSellerCountryCode returns the SellerCountryCode field if non-nil, zero value otherwise.

### GetSellerCountryCodeOk

`func (o *VintedItemDetail) GetSellerCountryCodeOk() (*string, bool)`

GetSellerCountryCodeOk returns a tuple with the SellerCountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSellerCountryCode

`func (o *VintedItemDetail) SetSellerCountryCode(v string)`

SetSellerCountryCode sets SellerCountryCode field to given value.

### HasSellerCountryCode

`func (o *VintedItemDetail) HasSellerCountryCode() bool`

HasSellerCountryCode returns a boolean if a field has been set.

### SetSellerCountryCodeNil

`func (o *VintedItemDetail) SetSellerCountryCodeNil(b bool)`

 SetSellerCountryCodeNil sets the value for SellerCountryCode to be an explicit nil

### UnsetSellerCountryCode
`func (o *VintedItemDetail) UnsetSellerCountryCode()`

UnsetSellerCountryCode ensures that no value is present for SellerCountryCode, not even an explicit nil
### GetSimilarityScore

`func (o *VintedItemDetail) GetSimilarityScore() float32`

GetSimilarityScore returns the SimilarityScore field if non-nil, zero value otherwise.

### GetSimilarityScoreOk

`func (o *VintedItemDetail) GetSimilarityScoreOk() (*float32, bool)`

GetSimilarityScoreOk returns a tuple with the SimilarityScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSimilarityScore

`func (o *VintedItemDetail) SetSimilarityScore(v float32)`

SetSimilarityScore sets SimilarityScore field to given value.

### HasSimilarityScore

`func (o *VintedItemDetail) HasSimilarityScore() bool`

HasSimilarityScore returns a boolean if a field has been set.

### SetSimilarityScoreNil

`func (o *VintedItemDetail) SetSimilarityScoreNil(b bool)`

 SetSimilarityScoreNil sets the value for SimilarityScore to be an explicit nil

### UnsetSimilarityScore
`func (o *VintedItemDetail) UnsetSimilarityScore()`

UnsetSimilarityScore ensures that no value is present for SimilarityScore, not even an explicit nil
### GetUser

`func (o *VintedItemDetail) GetUser() VintedUserSummary`

GetUser returns the User field if non-nil, zero value otherwise.

### GetUserOk

`func (o *VintedItemDetail) GetUserOk() (*VintedUserSummary, bool)`

GetUserOk returns a tuple with the User field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUser

`func (o *VintedItemDetail) SetUser(v VintedUserSummary)`

SetUser sets User field to given value.

### HasUser

`func (o *VintedItemDetail) HasUser() bool`

HasUser returns a boolean if a field has been set.

### SetUserNil

`func (o *VintedItemDetail) SetUserNil(b bool)`

 SetUserNil sets the value for User to be an explicit nil

### UnsetUser
`func (o *VintedItemDetail) UnsetUser()`

UnsetUser ensures that no value is present for User, not even an explicit nil
### GetPhoto

`func (o *VintedItemDetail) GetPhoto() VintedPhoto`

GetPhoto returns the Photo field if non-nil, zero value otherwise.

### GetPhotoOk

`func (o *VintedItemDetail) GetPhotoOk() (*VintedPhoto, bool)`

GetPhotoOk returns a tuple with the Photo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhoto

`func (o *VintedItemDetail) SetPhoto(v VintedPhoto)`

SetPhoto sets Photo field to given value.

### HasPhoto

`func (o *VintedItemDetail) HasPhoto() bool`

HasPhoto returns a boolean if a field has been set.

### SetPhotoNil

`func (o *VintedItemDetail) SetPhotoNil(b bool)`

 SetPhotoNil sets the value for Photo to be an explicit nil

### UnsetPhoto
`func (o *VintedItemDetail) UnsetPhoto()`

UnsetPhoto ensures that no value is present for Photo, not even an explicit nil
### GetPhotos

`func (o *VintedItemDetail) GetPhotos() []VintedPhoto`

GetPhotos returns the Photos field if non-nil, zero value otherwise.

### GetPhotosOk

`func (o *VintedItemDetail) GetPhotosOk() (*[]VintedPhoto, bool)`

GetPhotosOk returns a tuple with the Photos field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhotos

`func (o *VintedItemDetail) SetPhotos(v []VintedPhoto)`

SetPhotos sets Photos field to given value.

### HasPhotos

`func (o *VintedItemDetail) HasPhotos() bool`

HasPhotos returns a boolean if a field has been set.

### GetDescription

`func (o *VintedItemDetail) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *VintedItemDetail) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *VintedItemDetail) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *VintedItemDetail) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *VintedItemDetail) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *VintedItemDetail) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetCatalogId

`func (o *VintedItemDetail) GetCatalogId() int32`

GetCatalogId returns the CatalogId field if non-nil, zero value otherwise.

### GetCatalogIdOk

`func (o *VintedItemDetail) GetCatalogIdOk() (*int32, bool)`

GetCatalogIdOk returns a tuple with the CatalogId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCatalogId

`func (o *VintedItemDetail) SetCatalogId(v int32)`

SetCatalogId sets CatalogId field to given value.

### HasCatalogId

`func (o *VintedItemDetail) HasCatalogId() bool`

HasCatalogId returns a boolean if a field has been set.

### SetCatalogIdNil

`func (o *VintedItemDetail) SetCatalogIdNil(b bool)`

 SetCatalogIdNil sets the value for CatalogId to be an explicit nil

### UnsetCatalogId
`func (o *VintedItemDetail) UnsetCatalogId()`

UnsetCatalogId ensures that no value is present for CatalogId, not even an explicit nil
### GetColor1

`func (o *VintedItemDetail) GetColor1() string`

GetColor1 returns the Color1 field if non-nil, zero value otherwise.

### GetColor1Ok

`func (o *VintedItemDetail) GetColor1Ok() (*string, bool)`

GetColor1Ok returns a tuple with the Color1 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColor1

`func (o *VintedItemDetail) SetColor1(v string)`

SetColor1 sets Color1 field to given value.

### HasColor1

`func (o *VintedItemDetail) HasColor1() bool`

HasColor1 returns a boolean if a field has been set.

### SetColor1Nil

`func (o *VintedItemDetail) SetColor1Nil(b bool)`

 SetColor1Nil sets the value for Color1 to be an explicit nil

### UnsetColor1
`func (o *VintedItemDetail) UnsetColor1()`

UnsetColor1 ensures that no value is present for Color1, not even an explicit nil
### GetColor2

`func (o *VintedItemDetail) GetColor2() string`

GetColor2 returns the Color2 field if non-nil, zero value otherwise.

### GetColor2Ok

`func (o *VintedItemDetail) GetColor2Ok() (*string, bool)`

GetColor2Ok returns a tuple with the Color2 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColor2

`func (o *VintedItemDetail) SetColor2(v string)`

SetColor2 sets Color2 field to given value.

### HasColor2

`func (o *VintedItemDetail) HasColor2() bool`

HasColor2 returns a boolean if a field has been set.

### SetColor2Nil

`func (o *VintedItemDetail) SetColor2Nil(b bool)`

 SetColor2Nil sets the value for Color2 to be an explicit nil

### UnsetColor2
`func (o *VintedItemDetail) UnsetColor2()`

UnsetColor2 ensures that no value is present for Color2, not even an explicit nil
### GetPackageSizeId

`func (o *VintedItemDetail) GetPackageSizeId() int32`

GetPackageSizeId returns the PackageSizeId field if non-nil, zero value otherwise.

### GetPackageSizeIdOk

`func (o *VintedItemDetail) GetPackageSizeIdOk() (*int32, bool)`

GetPackageSizeIdOk returns a tuple with the PackageSizeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPackageSizeId

`func (o *VintedItemDetail) SetPackageSizeId(v int32)`

SetPackageSizeId sets PackageSizeId field to given value.

### HasPackageSizeId

`func (o *VintedItemDetail) HasPackageSizeId() bool`

HasPackageSizeId returns a boolean if a field has been set.

### SetPackageSizeIdNil

`func (o *VintedItemDetail) SetPackageSizeIdNil(b bool)`

 SetPackageSizeIdNil sets the value for PackageSizeId to be an explicit nil

### UnsetPackageSizeId
`func (o *VintedItemDetail) UnsetPackageSizeId()`

UnsetPackageSizeId ensures that no value is present for PackageSizeId, not even an explicit nil
### GetIsFavourite

`func (o *VintedItemDetail) GetIsFavourite() bool`

GetIsFavourite returns the IsFavourite field if non-nil, zero value otherwise.

### GetIsFavouriteOk

`func (o *VintedItemDetail) GetIsFavouriteOk() (*bool, bool)`

GetIsFavouriteOk returns a tuple with the IsFavourite field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsFavourite

`func (o *VintedItemDetail) SetIsFavourite(v bool)`

SetIsFavourite sets IsFavourite field to given value.

### HasIsFavourite

`func (o *VintedItemDetail) HasIsFavourite() bool`

HasIsFavourite returns a boolean if a field has been set.

### GetCanBuy

`func (o *VintedItemDetail) GetCanBuy() bool`

GetCanBuy returns the CanBuy field if non-nil, zero value otherwise.

### GetCanBuyOk

`func (o *VintedItemDetail) GetCanBuyOk() (*bool, bool)`

GetCanBuyOk returns a tuple with the CanBuy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCanBuy

`func (o *VintedItemDetail) SetCanBuy(v bool)`

SetCanBuy sets CanBuy field to given value.

### HasCanBuy

`func (o *VintedItemDetail) HasCanBuy() bool`

HasCanBuy returns a boolean if a field has been set.

### GetCanBundle

`func (o *VintedItemDetail) GetCanBundle() bool`

GetCanBundle returns the CanBundle field if non-nil, zero value otherwise.

### GetCanBundleOk

`func (o *VintedItemDetail) GetCanBundleOk() (*bool, bool)`

GetCanBundleOk returns a tuple with the CanBundle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCanBundle

`func (o *VintedItemDetail) SetCanBundle(v bool)`

SetCanBundle sets CanBundle field to given value.

### HasCanBundle

`func (o *VintedItemDetail) HasCanBundle() bool`

HasCanBundle returns a boolean if a field has been set.

### GetCanReserve

`func (o *VintedItemDetail) GetCanReserve() bool`

GetCanReserve returns the CanReserve field if non-nil, zero value otherwise.

### GetCanReserveOk

`func (o *VintedItemDetail) GetCanReserveOk() (*bool, bool)`

GetCanReserveOk returns a tuple with the CanReserve field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCanReserve

`func (o *VintedItemDetail) SetCanReserve(v bool)`

SetCanReserve sets CanReserve field to given value.

### HasCanReserve

`func (o *VintedItemDetail) HasCanReserve() bool`

HasCanReserve returns a boolean if a field has been set.

### GetInstantBuy

`func (o *VintedItemDetail) GetInstantBuy() bool`

GetInstantBuy returns the InstantBuy field if non-nil, zero value otherwise.

### GetInstantBuyOk

`func (o *VintedItemDetail) GetInstantBuyOk() (*bool, bool)`

GetInstantBuyOk returns a tuple with the InstantBuy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInstantBuy

`func (o *VintedItemDetail) SetInstantBuy(v bool)`

SetInstantBuy sets InstantBuy field to given value.

### HasInstantBuy

`func (o *VintedItemDetail) HasInstantBuy() bool`

HasInstantBuy returns a boolean if a field has been set.

### GetIsHidden

`func (o *VintedItemDetail) GetIsHidden() bool`

GetIsHidden returns the IsHidden field if non-nil, zero value otherwise.

### GetIsHiddenOk

`func (o *VintedItemDetail) GetIsHiddenOk() (*bool, bool)`

GetIsHiddenOk returns a tuple with the IsHidden field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsHidden

`func (o *VintedItemDetail) SetIsHidden(v bool)`

SetIsHidden sets IsHidden field to given value.

### HasIsHidden

`func (o *VintedItemDetail) HasIsHidden() bool`

HasIsHidden returns a boolean if a field has been set.

### GetIsReserved

`func (o *VintedItemDetail) GetIsReserved() bool`

GetIsReserved returns the IsReserved field if non-nil, zero value otherwise.

### GetIsReservedOk

`func (o *VintedItemDetail) GetIsReservedOk() (*bool, bool)`

GetIsReservedOk returns a tuple with the IsReserved field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsReserved

`func (o *VintedItemDetail) SetIsReserved(v bool)`

SetIsReserved sets IsReserved field to given value.

### HasIsReserved

`func (o *VintedItemDetail) HasIsReserved() bool`

HasIsReserved returns a boolean if a field has been set.

### GetIsClosed

`func (o *VintedItemDetail) GetIsClosed() bool`

GetIsClosed returns the IsClosed field if non-nil, zero value otherwise.

### GetIsClosedOk

`func (o *VintedItemDetail) GetIsClosedOk() (*bool, bool)`

GetIsClosedOk returns a tuple with the IsClosed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsClosed

`func (o *VintedItemDetail) SetIsClosed(v bool)`

SetIsClosed sets IsClosed field to given value.

### HasIsClosed

`func (o *VintedItemDetail) HasIsClosed() bool`

HasIsClosed returns a boolean if a field has been set.

### GetSeller

`func (o *VintedItemDetail) GetSeller() VintedSellerSummary`

GetSeller returns the Seller field if non-nil, zero value otherwise.

### GetSellerOk

`func (o *VintedItemDetail) GetSellerOk() (*VintedSellerSummary, bool)`

GetSellerOk returns a tuple with the Seller field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeller

`func (o *VintedItemDetail) SetSeller(v VintedSellerSummary)`

SetSeller sets Seller field to given value.

### HasSeller

`func (o *VintedItemDetail) HasSeller() bool`

HasSeller returns a boolean if a field has been set.

### SetSellerNil

`func (o *VintedItemDetail) SetSellerNil(b bool)`

 SetSellerNil sets the value for Seller to be an explicit nil

### UnsetSeller
`func (o *VintedItemDetail) UnsetSeller()`

UnsetSeller ensures that no value is present for Seller, not even an explicit nil
### GetSizeId

`func (o *VintedItemDetail) GetSizeId() int32`

GetSizeId returns the SizeId field if non-nil, zero value otherwise.

### GetSizeIdOk

`func (o *VintedItemDetail) GetSizeIdOk() (*int32, bool)`

GetSizeIdOk returns a tuple with the SizeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSizeId

`func (o *VintedItemDetail) SetSizeId(v int32)`

SetSizeId sets SizeId field to given value.

### HasSizeId

`func (o *VintedItemDetail) HasSizeId() bool`

HasSizeId returns a boolean if a field has been set.

### SetSizeIdNil

`func (o *VintedItemDetail) SetSizeIdNil(b bool)`

 SetSizeIdNil sets the value for SizeId to be an explicit nil

### UnsetSizeId
`func (o *VintedItemDetail) UnsetSizeId()`

UnsetSizeId ensures that no value is present for SizeId, not even an explicit nil
### GetStatusId

`func (o *VintedItemDetail) GetStatusId() int32`

GetStatusId returns the StatusId field if non-nil, zero value otherwise.

### GetStatusIdOk

`func (o *VintedItemDetail) GetStatusIdOk() (*int32, bool)`

GetStatusIdOk returns a tuple with the StatusId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusId

`func (o *VintedItemDetail) SetStatusId(v int32)`

SetStatusId sets StatusId field to given value.

### HasStatusId

`func (o *VintedItemDetail) HasStatusId() bool`

HasStatusId returns a boolean if a field has been set.

### SetStatusIdNil

`func (o *VintedItemDetail) SetStatusIdNil(b bool)`

 SetStatusIdNil sets the value for StatusId to be an explicit nil

### UnsetStatusId
`func (o *VintedItemDetail) UnsetStatusId()`

UnsetStatusId ensures that no value is present for StatusId, not even an explicit nil
### GetBrandId

`func (o *VintedItemDetail) GetBrandId() int32`

GetBrandId returns the BrandId field if non-nil, zero value otherwise.

### GetBrandIdOk

`func (o *VintedItemDetail) GetBrandIdOk() (*int32, bool)`

GetBrandIdOk returns a tuple with the BrandId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBrandId

`func (o *VintedItemDetail) SetBrandId(v int32)`

SetBrandId sets BrandId field to given value.

### HasBrandId

`func (o *VintedItemDetail) HasBrandId() bool`

HasBrandId returns a boolean if a field has been set.

### SetBrandIdNil

`func (o *VintedItemDetail) SetBrandIdNil(b bool)`

 SetBrandIdNil sets the value for BrandId to be an explicit nil

### UnsetBrandId
`func (o *VintedItemDetail) UnsetBrandId()`

UnsetBrandId ensures that no value is present for BrandId, not even an explicit nil
### GetCategory

`func (o *VintedItemDetail) GetCategory() []string`

GetCategory returns the Category field if non-nil, zero value otherwise.

### GetCategoryOk

`func (o *VintedItemDetail) GetCategoryOk() (*[]string, bool)`

GetCategoryOk returns a tuple with the Category field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategory

`func (o *VintedItemDetail) SetCategory(v []string)`

SetCategory sets Category field to given value.

### HasCategory

`func (o *VintedItemDetail) HasCategory() bool`

HasCategory returns a boolean if a field has been set.

### GetUploadDate

`func (o *VintedItemDetail) GetUploadDate() string`

GetUploadDate returns the UploadDate field if non-nil, zero value otherwise.

### GetUploadDateOk

`func (o *VintedItemDetail) GetUploadDateOk() (*string, bool)`

GetUploadDateOk returns a tuple with the UploadDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUploadDate

`func (o *VintedItemDetail) SetUploadDate(v string)`

SetUploadDate sets UploadDate field to given value.

### HasUploadDate

`func (o *VintedItemDetail) HasUploadDate() bool`

HasUploadDate returns a boolean if a field has been set.

### SetUploadDateNil

`func (o *VintedItemDetail) SetUploadDateNil(b bool)`

 SetUploadDateNil sets the value for UploadDate to be an explicit nil

### UnsetUploadDate
`func (o *VintedItemDetail) UnsetUploadDate()`

UnsetUploadDate ensures that no value is present for UploadDate, not even an explicit nil
### GetUploadedAt

`func (o *VintedItemDetail) GetUploadedAt() string`

GetUploadedAt returns the UploadedAt field if non-nil, zero value otherwise.

### GetUploadedAtOk

`func (o *VintedItemDetail) GetUploadedAtOk() (*string, bool)`

GetUploadedAtOk returns a tuple with the UploadedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUploadedAt

`func (o *VintedItemDetail) SetUploadedAt(v string)`

SetUploadedAt sets UploadedAt field to given value.

### HasUploadedAt

`func (o *VintedItemDetail) HasUploadedAt() bool`

HasUploadedAt returns a boolean if a field has been set.

### SetUploadedAtNil

`func (o *VintedItemDetail) SetUploadedAtNil(b bool)`

 SetUploadedAtNil sets the value for UploadedAt to be an explicit nil

### UnsetUploadedAt
`func (o *VintedItemDetail) UnsetUploadedAt()`

UnsetUploadedAt ensures that no value is present for UploadedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# VintedItemSummary

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

## Methods

### NewVintedItemSummary

`func NewVintedItemSummary(id int32, title string, price VintedPrice, url string, ) *VintedItemSummary`

NewVintedItemSummary instantiates a new VintedItemSummary object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVintedItemSummaryWithDefaults

`func NewVintedItemSummaryWithDefaults() *VintedItemSummary`

NewVintedItemSummaryWithDefaults instantiates a new VintedItemSummary object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *VintedItemSummary) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *VintedItemSummary) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *VintedItemSummary) SetId(v int32)`

SetId sets Id field to given value.


### GetTitle

`func (o *VintedItemSummary) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *VintedItemSummary) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *VintedItemSummary) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetPrice

`func (o *VintedItemSummary) GetPrice() VintedPrice`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *VintedItemSummary) GetPriceOk() (*VintedPrice, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *VintedItemSummary) SetPrice(v VintedPrice)`

SetPrice sets Price field to given value.


### GetBrandTitle

`func (o *VintedItemSummary) GetBrandTitle() string`

GetBrandTitle returns the BrandTitle field if non-nil, zero value otherwise.

### GetBrandTitleOk

`func (o *VintedItemSummary) GetBrandTitleOk() (*string, bool)`

GetBrandTitleOk returns a tuple with the BrandTitle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBrandTitle

`func (o *VintedItemSummary) SetBrandTitle(v string)`

SetBrandTitle sets BrandTitle field to given value.

### HasBrandTitle

`func (o *VintedItemSummary) HasBrandTitle() bool`

HasBrandTitle returns a boolean if a field has been set.

### SetBrandTitleNil

`func (o *VintedItemSummary) SetBrandTitleNil(b bool)`

 SetBrandTitleNil sets the value for BrandTitle to be an explicit nil

### UnsetBrandTitle
`func (o *VintedItemSummary) UnsetBrandTitle()`

UnsetBrandTitle ensures that no value is present for BrandTitle, not even an explicit nil
### GetDisplayTitle

`func (o *VintedItemSummary) GetDisplayTitle() string`

GetDisplayTitle returns the DisplayTitle field if non-nil, zero value otherwise.

### GetDisplayTitleOk

`func (o *VintedItemSummary) GetDisplayTitleOk() (*string, bool)`

GetDisplayTitleOk returns a tuple with the DisplayTitle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayTitle

`func (o *VintedItemSummary) SetDisplayTitle(v string)`

SetDisplayTitle sets DisplayTitle field to given value.

### HasDisplayTitle

`func (o *VintedItemSummary) HasDisplayTitle() bool`

HasDisplayTitle returns a boolean if a field has been set.

### SetDisplayTitleNil

`func (o *VintedItemSummary) SetDisplayTitleNil(b bool)`

 SetDisplayTitleNil sets the value for DisplayTitle to be an explicit nil

### UnsetDisplayTitle
`func (o *VintedItemSummary) UnsetDisplayTitle()`

UnsetDisplayTitle ensures that no value is present for DisplayTitle, not even an explicit nil
### GetDisplaySubtitle

`func (o *VintedItemSummary) GetDisplaySubtitle() string`

GetDisplaySubtitle returns the DisplaySubtitle field if non-nil, zero value otherwise.

### GetDisplaySubtitleOk

`func (o *VintedItemSummary) GetDisplaySubtitleOk() (*string, bool)`

GetDisplaySubtitleOk returns a tuple with the DisplaySubtitle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplaySubtitle

`func (o *VintedItemSummary) SetDisplaySubtitle(v string)`

SetDisplaySubtitle sets DisplaySubtitle field to given value.

### HasDisplaySubtitle

`func (o *VintedItemSummary) HasDisplaySubtitle() bool`

HasDisplaySubtitle returns a boolean if a field has been set.

### SetDisplaySubtitleNil

`func (o *VintedItemSummary) SetDisplaySubtitleNil(b bool)`

 SetDisplaySubtitleNil sets the value for DisplaySubtitle to be an explicit nil

### UnsetDisplaySubtitle
`func (o *VintedItemSummary) UnsetDisplaySubtitle()`

UnsetDisplaySubtitle ensures that no value is present for DisplaySubtitle, not even an explicit nil
### GetSizeTitle

`func (o *VintedItemSummary) GetSizeTitle() string`

GetSizeTitle returns the SizeTitle field if non-nil, zero value otherwise.

### GetSizeTitleOk

`func (o *VintedItemSummary) GetSizeTitleOk() (*string, bool)`

GetSizeTitleOk returns a tuple with the SizeTitle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSizeTitle

`func (o *VintedItemSummary) SetSizeTitle(v string)`

SetSizeTitle sets SizeTitle field to given value.

### HasSizeTitle

`func (o *VintedItemSummary) HasSizeTitle() bool`

HasSizeTitle returns a boolean if a field has been set.

### SetSizeTitleNil

`func (o *VintedItemSummary) SetSizeTitleNil(b bool)`

 SetSizeTitleNil sets the value for SizeTitle to be an explicit nil

### UnsetSizeTitle
`func (o *VintedItemSummary) UnsetSizeTitle()`

UnsetSizeTitle ensures that no value is present for SizeTitle, not even an explicit nil
### GetStatus

`func (o *VintedItemSummary) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *VintedItemSummary) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *VintedItemSummary) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *VintedItemSummary) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### SetStatusNil

`func (o *VintedItemSummary) SetStatusNil(b bool)`

 SetStatusNil sets the value for Status to be an explicit nil

### UnsetStatus
`func (o *VintedItemSummary) UnsetStatus()`

UnsetStatus ensures that no value is present for Status, not even an explicit nil
### GetUrl

`func (o *VintedItemSummary) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *VintedItemSummary) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *VintedItemSummary) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetPath

`func (o *VintedItemSummary) GetPath() string`

GetPath returns the Path field if non-nil, zero value otherwise.

### GetPathOk

`func (o *VintedItemSummary) GetPathOk() (*string, bool)`

GetPathOk returns a tuple with the Path field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPath

`func (o *VintedItemSummary) SetPath(v string)`

SetPath sets Path field to given value.

### HasPath

`func (o *VintedItemSummary) HasPath() bool`

HasPath returns a boolean if a field has been set.

### SetPathNil

`func (o *VintedItemSummary) SetPathNil(b bool)`

 SetPathNil sets the value for Path to be an explicit nil

### UnsetPath
`func (o *VintedItemSummary) UnsetPath()`

UnsetPath ensures that no value is present for Path, not even an explicit nil
### GetIsVisible

`func (o *VintedItemSummary) GetIsVisible() bool`

GetIsVisible returns the IsVisible field if non-nil, zero value otherwise.

### GetIsVisibleOk

`func (o *VintedItemSummary) GetIsVisibleOk() (*bool, bool)`

GetIsVisibleOk returns a tuple with the IsVisible field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsVisible

`func (o *VintedItemSummary) SetIsVisible(v bool)`

SetIsVisible sets IsVisible field to given value.

### HasIsVisible

`func (o *VintedItemSummary) HasIsVisible() bool`

HasIsVisible returns a boolean if a field has been set.

### GetPromoted

`func (o *VintedItemSummary) GetPromoted() bool`

GetPromoted returns the Promoted field if non-nil, zero value otherwise.

### GetPromotedOk

`func (o *VintedItemSummary) GetPromotedOk() (*bool, bool)`

GetPromotedOk returns a tuple with the Promoted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPromoted

`func (o *VintedItemSummary) SetPromoted(v bool)`

SetPromoted sets Promoted field to given value.

### HasPromoted

`func (o *VintedItemSummary) HasPromoted() bool`

HasPromoted returns a boolean if a field has been set.

### GetFavouriteCount

`func (o *VintedItemSummary) GetFavouriteCount() int32`

GetFavouriteCount returns the FavouriteCount field if non-nil, zero value otherwise.

### GetFavouriteCountOk

`func (o *VintedItemSummary) GetFavouriteCountOk() (*int32, bool)`

GetFavouriteCountOk returns a tuple with the FavouriteCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFavouriteCount

`func (o *VintedItemSummary) SetFavouriteCount(v int32)`

SetFavouriteCount sets FavouriteCount field to given value.

### HasFavouriteCount

`func (o *VintedItemSummary) HasFavouriteCount() bool`

HasFavouriteCount returns a boolean if a field has been set.

### GetViewCount

`func (o *VintedItemSummary) GetViewCount() int32`

GetViewCount returns the ViewCount field if non-nil, zero value otherwise.

### GetViewCountOk

`func (o *VintedItemSummary) GetViewCountOk() (*int32, bool)`

GetViewCountOk returns a tuple with the ViewCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetViewCount

`func (o *VintedItemSummary) SetViewCount(v int32)`

SetViewCount sets ViewCount field to given value.

### HasViewCount

`func (o *VintedItemSummary) HasViewCount() bool`

HasViewCount returns a boolean if a field has been set.

### GetServiceFee

`func (o *VintedItemSummary) GetServiceFee() string`

GetServiceFee returns the ServiceFee field if non-nil, zero value otherwise.

### GetServiceFeeOk

`func (o *VintedItemSummary) GetServiceFeeOk() (*string, bool)`

GetServiceFeeOk returns a tuple with the ServiceFee field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetServiceFee

`func (o *VintedItemSummary) SetServiceFee(v string)`

SetServiceFee sets ServiceFee field to given value.

### HasServiceFee

`func (o *VintedItemSummary) HasServiceFee() bool`

HasServiceFee returns a boolean if a field has been set.

### SetServiceFeeNil

`func (o *VintedItemSummary) SetServiceFeeNil(b bool)`

 SetServiceFeeNil sets the value for ServiceFee to be an explicit nil

### UnsetServiceFee
`func (o *VintedItemSummary) UnsetServiceFee()`

UnsetServiceFee ensures that no value is present for ServiceFee, not even an explicit nil
### GetTotalItemPrice

`func (o *VintedItemSummary) GetTotalItemPrice() string`

GetTotalItemPrice returns the TotalItemPrice field if non-nil, zero value otherwise.

### GetTotalItemPriceOk

`func (o *VintedItemSummary) GetTotalItemPriceOk() (*string, bool)`

GetTotalItemPriceOk returns a tuple with the TotalItemPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalItemPrice

`func (o *VintedItemSummary) SetTotalItemPrice(v string)`

SetTotalItemPrice sets TotalItemPrice field to given value.

### HasTotalItemPrice

`func (o *VintedItemSummary) HasTotalItemPrice() bool`

HasTotalItemPrice returns a boolean if a field has been set.

### SetTotalItemPriceNil

`func (o *VintedItemSummary) SetTotalItemPriceNil(b bool)`

 SetTotalItemPriceNil sets the value for TotalItemPrice to be an explicit nil

### UnsetTotalItemPrice
`func (o *VintedItemSummary) UnsetTotalItemPrice()`

UnsetTotalItemPrice ensures that no value is present for TotalItemPrice, not even an explicit nil
### GetContentSource

`func (o *VintedItemSummary) GetContentSource() string`

GetContentSource returns the ContentSource field if non-nil, zero value otherwise.

### GetContentSourceOk

`func (o *VintedItemSummary) GetContentSourceOk() (*string, bool)`

GetContentSourceOk returns a tuple with the ContentSource field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContentSource

`func (o *VintedItemSummary) SetContentSource(v string)`

SetContentSource sets ContentSource field to given value.

### HasContentSource

`func (o *VintedItemSummary) HasContentSource() bool`

HasContentSource returns a boolean if a field has been set.

### SetContentSourceNil

`func (o *VintedItemSummary) SetContentSourceNil(b bool)`

 SetContentSourceNil sets the value for ContentSource to be an explicit nil

### UnsetContentSource
`func (o *VintedItemSummary) UnsetContentSource()`

UnsetContentSource ensures that no value is present for ContentSource, not even an explicit nil
### GetSellerCountryCode

`func (o *VintedItemSummary) GetSellerCountryCode() string`

GetSellerCountryCode returns the SellerCountryCode field if non-nil, zero value otherwise.

### GetSellerCountryCodeOk

`func (o *VintedItemSummary) GetSellerCountryCodeOk() (*string, bool)`

GetSellerCountryCodeOk returns a tuple with the SellerCountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSellerCountryCode

`func (o *VintedItemSummary) SetSellerCountryCode(v string)`

SetSellerCountryCode sets SellerCountryCode field to given value.

### HasSellerCountryCode

`func (o *VintedItemSummary) HasSellerCountryCode() bool`

HasSellerCountryCode returns a boolean if a field has been set.

### SetSellerCountryCodeNil

`func (o *VintedItemSummary) SetSellerCountryCodeNil(b bool)`

 SetSellerCountryCodeNil sets the value for SellerCountryCode to be an explicit nil

### UnsetSellerCountryCode
`func (o *VintedItemSummary) UnsetSellerCountryCode()`

UnsetSellerCountryCode ensures that no value is present for SellerCountryCode, not even an explicit nil
### GetSimilarityScore

`func (o *VintedItemSummary) GetSimilarityScore() float32`

GetSimilarityScore returns the SimilarityScore field if non-nil, zero value otherwise.

### GetSimilarityScoreOk

`func (o *VintedItemSummary) GetSimilarityScoreOk() (*float32, bool)`

GetSimilarityScoreOk returns a tuple with the SimilarityScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSimilarityScore

`func (o *VintedItemSummary) SetSimilarityScore(v float32)`

SetSimilarityScore sets SimilarityScore field to given value.

### HasSimilarityScore

`func (o *VintedItemSummary) HasSimilarityScore() bool`

HasSimilarityScore returns a boolean if a field has been set.

### SetSimilarityScoreNil

`func (o *VintedItemSummary) SetSimilarityScoreNil(b bool)`

 SetSimilarityScoreNil sets the value for SimilarityScore to be an explicit nil

### UnsetSimilarityScore
`func (o *VintedItemSummary) UnsetSimilarityScore()`

UnsetSimilarityScore ensures that no value is present for SimilarityScore, not even an explicit nil
### GetUser

`func (o *VintedItemSummary) GetUser() VintedUserSummary`

GetUser returns the User field if non-nil, zero value otherwise.

### GetUserOk

`func (o *VintedItemSummary) GetUserOk() (*VintedUserSummary, bool)`

GetUserOk returns a tuple with the User field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUser

`func (o *VintedItemSummary) SetUser(v VintedUserSummary)`

SetUser sets User field to given value.

### HasUser

`func (o *VintedItemSummary) HasUser() bool`

HasUser returns a boolean if a field has been set.

### SetUserNil

`func (o *VintedItemSummary) SetUserNil(b bool)`

 SetUserNil sets the value for User to be an explicit nil

### UnsetUser
`func (o *VintedItemSummary) UnsetUser()`

UnsetUser ensures that no value is present for User, not even an explicit nil
### GetPhoto

`func (o *VintedItemSummary) GetPhoto() VintedPhoto`

GetPhoto returns the Photo field if non-nil, zero value otherwise.

### GetPhotoOk

`func (o *VintedItemSummary) GetPhotoOk() (*VintedPhoto, bool)`

GetPhotoOk returns a tuple with the Photo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhoto

`func (o *VintedItemSummary) SetPhoto(v VintedPhoto)`

SetPhoto sets Photo field to given value.

### HasPhoto

`func (o *VintedItemSummary) HasPhoto() bool`

HasPhoto returns a boolean if a field has been set.

### SetPhotoNil

`func (o *VintedItemSummary) SetPhotoNil(b bool)`

 SetPhotoNil sets the value for Photo to be an explicit nil

### UnsetPhoto
`func (o *VintedItemSummary) UnsetPhoto()`

UnsetPhoto ensures that no value is present for Photo, not even an explicit nil
### GetPhotos

`func (o *VintedItemSummary) GetPhotos() []VintedPhoto`

GetPhotos returns the Photos field if non-nil, zero value otherwise.

### GetPhotosOk

`func (o *VintedItemSummary) GetPhotosOk() (*[]VintedPhoto, bool)`

GetPhotosOk returns a tuple with the Photos field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhotos

`func (o *VintedItemSummary) SetPhotos(v []VintedPhoto)`

SetPhotos sets Photos field to given value.

### HasPhotos

`func (o *VintedItemSummary) HasPhotos() bool`

HasPhotos returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



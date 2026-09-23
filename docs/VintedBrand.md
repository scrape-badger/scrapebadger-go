# VintedBrand

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **int32** |  | 
**Title** | **string** |  | 
**Slug** | **string** |  | 
**ItemCount** | Pointer to **int32** |  | [optional] [default to 0]
**FavouriteCount** | Pointer to **int32** |  | [optional] [default to 0]
**IsLuxury** | Pointer to **bool** |  | [optional] [default to false]
**Url** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewVintedBrand

`func NewVintedBrand(id int32, title string, slug string, ) *VintedBrand`

NewVintedBrand instantiates a new VintedBrand object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVintedBrandWithDefaults

`func NewVintedBrandWithDefaults() *VintedBrand`

NewVintedBrandWithDefaults instantiates a new VintedBrand object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *VintedBrand) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *VintedBrand) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *VintedBrand) SetId(v int32)`

SetId sets Id field to given value.


### GetTitle

`func (o *VintedBrand) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *VintedBrand) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *VintedBrand) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetSlug

`func (o *VintedBrand) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *VintedBrand) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *VintedBrand) SetSlug(v string)`

SetSlug sets Slug field to given value.


### GetItemCount

`func (o *VintedBrand) GetItemCount() int32`

GetItemCount returns the ItemCount field if non-nil, zero value otherwise.

### GetItemCountOk

`func (o *VintedBrand) GetItemCountOk() (*int32, bool)`

GetItemCountOk returns a tuple with the ItemCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItemCount

`func (o *VintedBrand) SetItemCount(v int32)`

SetItemCount sets ItemCount field to given value.

### HasItemCount

`func (o *VintedBrand) HasItemCount() bool`

HasItemCount returns a boolean if a field has been set.

### GetFavouriteCount

`func (o *VintedBrand) GetFavouriteCount() int32`

GetFavouriteCount returns the FavouriteCount field if non-nil, zero value otherwise.

### GetFavouriteCountOk

`func (o *VintedBrand) GetFavouriteCountOk() (*int32, bool)`

GetFavouriteCountOk returns a tuple with the FavouriteCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFavouriteCount

`func (o *VintedBrand) SetFavouriteCount(v int32)`

SetFavouriteCount sets FavouriteCount field to given value.

### HasFavouriteCount

`func (o *VintedBrand) HasFavouriteCount() bool`

HasFavouriteCount returns a boolean if a field has been set.

### GetIsLuxury

`func (o *VintedBrand) GetIsLuxury() bool`

GetIsLuxury returns the IsLuxury field if non-nil, zero value otherwise.

### GetIsLuxuryOk

`func (o *VintedBrand) GetIsLuxuryOk() (*bool, bool)`

GetIsLuxuryOk returns a tuple with the IsLuxury field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsLuxury

`func (o *VintedBrand) SetIsLuxury(v bool)`

SetIsLuxury sets IsLuxury field to given value.

### HasIsLuxury

`func (o *VintedBrand) HasIsLuxury() bool`

HasIsLuxury returns a boolean if a field has been set.

### GetUrl

`func (o *VintedBrand) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *VintedBrand) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *VintedBrand) SetUrl(v string)`

SetUrl sets Url field to given value.

### HasUrl

`func (o *VintedBrand) HasUrl() bool`

HasUrl returns a boolean if a field has been set.

### SetUrlNil

`func (o *VintedBrand) SetUrlNil(b bool)`

 SetUrlNil sets the value for Url to be an explicit nil

### UnsetUrl
`func (o *VintedBrand) UnsetUrl()`

UnsetUrl ensures that no value is present for Url, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



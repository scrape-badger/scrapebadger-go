# VintedPhoto

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **int32** |  | 
**Url** | **string** |  | 
**DominantColor** | Pointer to **NullableString** |  | [optional] 
**IsMain** | Pointer to **bool** |  | [optional] [default to false]
**Width** | Pointer to **NullableInt32** |  | [optional] 
**Height** | Pointer to **NullableInt32** |  | [optional] 
**FullSizeUrl** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewVintedPhoto

`func NewVintedPhoto(id int32, url string, ) *VintedPhoto`

NewVintedPhoto instantiates a new VintedPhoto object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVintedPhotoWithDefaults

`func NewVintedPhotoWithDefaults() *VintedPhoto`

NewVintedPhotoWithDefaults instantiates a new VintedPhoto object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *VintedPhoto) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *VintedPhoto) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *VintedPhoto) SetId(v int32)`

SetId sets Id field to given value.


### GetUrl

`func (o *VintedPhoto) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *VintedPhoto) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *VintedPhoto) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetDominantColor

`func (o *VintedPhoto) GetDominantColor() string`

GetDominantColor returns the DominantColor field if non-nil, zero value otherwise.

### GetDominantColorOk

`func (o *VintedPhoto) GetDominantColorOk() (*string, bool)`

GetDominantColorOk returns a tuple with the DominantColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDominantColor

`func (o *VintedPhoto) SetDominantColor(v string)`

SetDominantColor sets DominantColor field to given value.

### HasDominantColor

`func (o *VintedPhoto) HasDominantColor() bool`

HasDominantColor returns a boolean if a field has been set.

### SetDominantColorNil

`func (o *VintedPhoto) SetDominantColorNil(b bool)`

 SetDominantColorNil sets the value for DominantColor to be an explicit nil

### UnsetDominantColor
`func (o *VintedPhoto) UnsetDominantColor()`

UnsetDominantColor ensures that no value is present for DominantColor, not even an explicit nil
### GetIsMain

`func (o *VintedPhoto) GetIsMain() bool`

GetIsMain returns the IsMain field if non-nil, zero value otherwise.

### GetIsMainOk

`func (o *VintedPhoto) GetIsMainOk() (*bool, bool)`

GetIsMainOk returns a tuple with the IsMain field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsMain

`func (o *VintedPhoto) SetIsMain(v bool)`

SetIsMain sets IsMain field to given value.

### HasIsMain

`func (o *VintedPhoto) HasIsMain() bool`

HasIsMain returns a boolean if a field has been set.

### GetWidth

`func (o *VintedPhoto) GetWidth() int32`

GetWidth returns the Width field if non-nil, zero value otherwise.

### GetWidthOk

`func (o *VintedPhoto) GetWidthOk() (*int32, bool)`

GetWidthOk returns a tuple with the Width field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWidth

`func (o *VintedPhoto) SetWidth(v int32)`

SetWidth sets Width field to given value.

### HasWidth

`func (o *VintedPhoto) HasWidth() bool`

HasWidth returns a boolean if a field has been set.

### SetWidthNil

`func (o *VintedPhoto) SetWidthNil(b bool)`

 SetWidthNil sets the value for Width to be an explicit nil

### UnsetWidth
`func (o *VintedPhoto) UnsetWidth()`

UnsetWidth ensures that no value is present for Width, not even an explicit nil
### GetHeight

`func (o *VintedPhoto) GetHeight() int32`

GetHeight returns the Height field if non-nil, zero value otherwise.

### GetHeightOk

`func (o *VintedPhoto) GetHeightOk() (*int32, bool)`

GetHeightOk returns a tuple with the Height field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeight

`func (o *VintedPhoto) SetHeight(v int32)`

SetHeight sets Height field to given value.

### HasHeight

`func (o *VintedPhoto) HasHeight() bool`

HasHeight returns a boolean if a field has been set.

### SetHeightNil

`func (o *VintedPhoto) SetHeightNil(b bool)`

 SetHeightNil sets the value for Height to be an explicit nil

### UnsetHeight
`func (o *VintedPhoto) UnsetHeight()`

UnsetHeight ensures that no value is present for Height, not even an explicit nil
### GetFullSizeUrl

`func (o *VintedPhoto) GetFullSizeUrl() string`

GetFullSizeUrl returns the FullSizeUrl field if non-nil, zero value otherwise.

### GetFullSizeUrlOk

`func (o *VintedPhoto) GetFullSizeUrlOk() (*string, bool)`

GetFullSizeUrlOk returns a tuple with the FullSizeUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFullSizeUrl

`func (o *VintedPhoto) SetFullSizeUrl(v string)`

SetFullSizeUrl sets FullSizeUrl field to given value.

### HasFullSizeUrl

`func (o *VintedPhoto) HasFullSizeUrl() bool`

HasFullSizeUrl returns a boolean if a field has been set.

### SetFullSizeUrlNil

`func (o *VintedPhoto) SetFullSizeUrlNil(b bool)`

 SetFullSizeUrlNil sets the value for FullSizeUrl to be an explicit nil

### UnsetFullSizeUrl
`func (o *VintedPhoto) UnsetFullSizeUrl()`

UnsetFullSizeUrl ensures that no value is present for FullSizeUrl, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



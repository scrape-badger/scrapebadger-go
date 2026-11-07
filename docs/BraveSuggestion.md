# BraveSuggestion

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Query** | **string** |  | 
**Type** | **string** |  | 
**IsEntity** | Pointer to **bool** |  | [optional] [default to false]
**Name** | Pointer to **NullableString** |  | [optional] 
**Desc** | Pointer to **NullableString** |  | [optional] 
**Img** | Pointer to **NullableString** |  | [optional] 
**Category** | Pointer to **NullableString** |  | [optional] 
**Logo** | Pointer to **NullableBool** |  | [optional] 

## Methods

### NewBraveSuggestion

`func NewBraveSuggestion(query string, type_ string, ) *BraveSuggestion`

NewBraveSuggestion instantiates a new BraveSuggestion object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBraveSuggestionWithDefaults

`func NewBraveSuggestionWithDefaults() *BraveSuggestion`

NewBraveSuggestionWithDefaults instantiates a new BraveSuggestion object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetQuery

`func (o *BraveSuggestion) GetQuery() string`

GetQuery returns the Query field if non-nil, zero value otherwise.

### GetQueryOk

`func (o *BraveSuggestion) GetQueryOk() (*string, bool)`

GetQueryOk returns a tuple with the Query field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuery

`func (o *BraveSuggestion) SetQuery(v string)`

SetQuery sets Query field to given value.


### GetType

`func (o *BraveSuggestion) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *BraveSuggestion) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *BraveSuggestion) SetType(v string)`

SetType sets Type field to given value.


### GetIsEntity

`func (o *BraveSuggestion) GetIsEntity() bool`

GetIsEntity returns the IsEntity field if non-nil, zero value otherwise.

### GetIsEntityOk

`func (o *BraveSuggestion) GetIsEntityOk() (*bool, bool)`

GetIsEntityOk returns a tuple with the IsEntity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsEntity

`func (o *BraveSuggestion) SetIsEntity(v bool)`

SetIsEntity sets IsEntity field to given value.

### HasIsEntity

`func (o *BraveSuggestion) HasIsEntity() bool`

HasIsEntity returns a boolean if a field has been set.

### GetName

`func (o *BraveSuggestion) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *BraveSuggestion) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *BraveSuggestion) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *BraveSuggestion) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *BraveSuggestion) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *BraveSuggestion) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetDesc

`func (o *BraveSuggestion) GetDesc() string`

GetDesc returns the Desc field if non-nil, zero value otherwise.

### GetDescOk

`func (o *BraveSuggestion) GetDescOk() (*string, bool)`

GetDescOk returns a tuple with the Desc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDesc

`func (o *BraveSuggestion) SetDesc(v string)`

SetDesc sets Desc field to given value.

### HasDesc

`func (o *BraveSuggestion) HasDesc() bool`

HasDesc returns a boolean if a field has been set.

### SetDescNil

`func (o *BraveSuggestion) SetDescNil(b bool)`

 SetDescNil sets the value for Desc to be an explicit nil

### UnsetDesc
`func (o *BraveSuggestion) UnsetDesc()`

UnsetDesc ensures that no value is present for Desc, not even an explicit nil
### GetImg

`func (o *BraveSuggestion) GetImg() string`

GetImg returns the Img field if non-nil, zero value otherwise.

### GetImgOk

`func (o *BraveSuggestion) GetImgOk() (*string, bool)`

GetImgOk returns a tuple with the Img field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImg

`func (o *BraveSuggestion) SetImg(v string)`

SetImg sets Img field to given value.

### HasImg

`func (o *BraveSuggestion) HasImg() bool`

HasImg returns a boolean if a field has been set.

### SetImgNil

`func (o *BraveSuggestion) SetImgNil(b bool)`

 SetImgNil sets the value for Img to be an explicit nil

### UnsetImg
`func (o *BraveSuggestion) UnsetImg()`

UnsetImg ensures that no value is present for Img, not even an explicit nil
### GetCategory

`func (o *BraveSuggestion) GetCategory() string`

GetCategory returns the Category field if non-nil, zero value otherwise.

### GetCategoryOk

`func (o *BraveSuggestion) GetCategoryOk() (*string, bool)`

GetCategoryOk returns a tuple with the Category field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategory

`func (o *BraveSuggestion) SetCategory(v string)`

SetCategory sets Category field to given value.

### HasCategory

`func (o *BraveSuggestion) HasCategory() bool`

HasCategory returns a boolean if a field has been set.

### SetCategoryNil

`func (o *BraveSuggestion) SetCategoryNil(b bool)`

 SetCategoryNil sets the value for Category to be an explicit nil

### UnsetCategory
`func (o *BraveSuggestion) UnsetCategory()`

UnsetCategory ensures that no value is present for Category, not even an explicit nil
### GetLogo

`func (o *BraveSuggestion) GetLogo() bool`

GetLogo returns the Logo field if non-nil, zero value otherwise.

### GetLogoOk

`func (o *BraveSuggestion) GetLogoOk() (*bool, bool)`

GetLogoOk returns a tuple with the Logo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogo

`func (o *BraveSuggestion) SetLogo(v bool)`

SetLogo sets Logo field to given value.

### HasLogo

`func (o *BraveSuggestion) HasLogo() bool`

HasLogo returns a boolean if a field has been set.

### SetLogoNil

`func (o *BraveSuggestion) SetLogoNil(b bool)`

 SetLogoNil sets the value for Logo to be an explicit nil

### UnsetLogo
`func (o *BraveSuggestion) UnsetLogo()`

UnsetLogo ensures that no value is present for Logo, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



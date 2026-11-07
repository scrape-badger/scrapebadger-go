# YelpCategory

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Title** | **string** |  | 
**Alias** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewYelpCategory

`func NewYelpCategory(title string, ) *YelpCategory`

NewYelpCategory instantiates a new YelpCategory object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewYelpCategoryWithDefaults

`func NewYelpCategoryWithDefaults() *YelpCategory`

NewYelpCategoryWithDefaults instantiates a new YelpCategory object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTitle

`func (o *YelpCategory) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *YelpCategory) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *YelpCategory) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetAlias

`func (o *YelpCategory) GetAlias() string`

GetAlias returns the Alias field if non-nil, zero value otherwise.

### GetAliasOk

`func (o *YelpCategory) GetAliasOk() (*string, bool)`

GetAliasOk returns a tuple with the Alias field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAlias

`func (o *YelpCategory) SetAlias(v string)`

SetAlias sets Alias field to given value.

### HasAlias

`func (o *YelpCategory) HasAlias() bool`

HasAlias returns a boolean if a field has been set.

### SetAliasNil

`func (o *YelpCategory) SetAliasNil(b bool)`

 SetAliasNil sets the value for Alias to be an explicit nil

### UnsetAlias
`func (o *YelpCategory) UnsetAlias()`

UnsetAlias ensures that no value is present for Alias, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



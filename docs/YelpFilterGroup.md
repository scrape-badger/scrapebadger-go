# YelpFilterGroup

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Title** | **string** |  | 
**Type** | **string** |  | 
**Options** | [**[]YelpFilterOption**](YelpFilterOption.md) |  | 

## Methods

### NewYelpFilterGroup

`func NewYelpFilterGroup(title string, type_ string, options []YelpFilterOption, ) *YelpFilterGroup`

NewYelpFilterGroup instantiates a new YelpFilterGroup object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewYelpFilterGroupWithDefaults

`func NewYelpFilterGroupWithDefaults() *YelpFilterGroup`

NewYelpFilterGroupWithDefaults instantiates a new YelpFilterGroup object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTitle

`func (o *YelpFilterGroup) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *YelpFilterGroup) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *YelpFilterGroup) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetType

`func (o *YelpFilterGroup) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *YelpFilterGroup) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *YelpFilterGroup) SetType(v string)`

SetType sets Type field to given value.


### GetOptions

`func (o *YelpFilterGroup) GetOptions() []YelpFilterOption`

GetOptions returns the Options field if non-nil, zero value otherwise.

### GetOptionsOk

`func (o *YelpFilterGroup) GetOptionsOk() (*[]YelpFilterOption, bool)`

GetOptionsOk returns a tuple with the Options field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptions

`func (o *YelpFilterGroup) SetOptions(v []YelpFilterOption)`

SetOptions sets Options field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



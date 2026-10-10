# ExtractRule

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Selector** | **string** | CSS or XPath selector. | 
**Type** | Pointer to **NullableString** |  | [optional] 
**All** | Pointer to **bool** | Return every match as a list, not just the first. | [optional] [default to false]
**Output** | Pointer to **string** | An element&#39;s text content, or its outer HTML. | [optional] [default to "text"]

## Methods

### NewExtractRule

`func NewExtractRule(selector string, ) *ExtractRule`

NewExtractRule instantiates a new ExtractRule object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExtractRuleWithDefaults

`func NewExtractRuleWithDefaults() *ExtractRule`

NewExtractRuleWithDefaults instantiates a new ExtractRule object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSelector

`func (o *ExtractRule) GetSelector() string`

GetSelector returns the Selector field if non-nil, zero value otherwise.

### GetSelectorOk

`func (o *ExtractRule) GetSelectorOk() (*string, bool)`

GetSelectorOk returns a tuple with the Selector field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSelector

`func (o *ExtractRule) SetSelector(v string)`

SetSelector sets Selector field to given value.


### GetType

`func (o *ExtractRule) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ExtractRule) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ExtractRule) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ExtractRule) HasType() bool`

HasType returns a boolean if a field has been set.

### SetTypeNil

`func (o *ExtractRule) SetTypeNil(b bool)`

 SetTypeNil sets the value for Type to be an explicit nil

### UnsetType
`func (o *ExtractRule) UnsetType()`

UnsetType ensures that no value is present for Type, not even an explicit nil
### GetAll

`func (o *ExtractRule) GetAll() bool`

GetAll returns the All field if non-nil, zero value otherwise.

### GetAllOk

`func (o *ExtractRule) GetAllOk() (*bool, bool)`

GetAllOk returns a tuple with the All field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAll

`func (o *ExtractRule) SetAll(v bool)`

SetAll sets All field to given value.

### HasAll

`func (o *ExtractRule) HasAll() bool`

HasAll returns a boolean if a field has been set.

### GetOutput

`func (o *ExtractRule) GetOutput() string`

GetOutput returns the Output field if non-nil, zero value otherwise.

### GetOutputOk

`func (o *ExtractRule) GetOutputOk() (*string, bool)`

GetOutputOk returns a tuple with the Output field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOutput

`func (o *ExtractRule) SetOutput(v string)`

SetOutput sets Output field to given value.

### HasOutput

`func (o *ExtractRule) HasOutput() bool`

HasOutput returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



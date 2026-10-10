# ExtractRequestExtractRulesValue

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Selector** | **string** | CSS or XPath selector. | 
**Type** | Pointer to **string** |  | [optional] 
**All** | Pointer to **bool** | Return every match as a list, not just the first. | [optional] [default to false]
**Output** | Pointer to **string** | An element&#39;s text content, or its outer HTML. | [optional] [default to "text"]

## Methods

### NewExtractRequestExtractRulesValue

`func NewExtractRequestExtractRulesValue(selector string, ) *ExtractRequestExtractRulesValue`

NewExtractRequestExtractRulesValue instantiates a new ExtractRequestExtractRulesValue object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExtractRequestExtractRulesValueWithDefaults

`func NewExtractRequestExtractRulesValueWithDefaults() *ExtractRequestExtractRulesValue`

NewExtractRequestExtractRulesValueWithDefaults instantiates a new ExtractRequestExtractRulesValue object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSelector

`func (o *ExtractRequestExtractRulesValue) GetSelector() string`

GetSelector returns the Selector field if non-nil, zero value otherwise.

### GetSelectorOk

`func (o *ExtractRequestExtractRulesValue) GetSelectorOk() (*string, bool)`

GetSelectorOk returns a tuple with the Selector field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSelector

`func (o *ExtractRequestExtractRulesValue) SetSelector(v string)`

SetSelector sets Selector field to given value.


### GetType

`func (o *ExtractRequestExtractRulesValue) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ExtractRequestExtractRulesValue) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ExtractRequestExtractRulesValue) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ExtractRequestExtractRulesValue) HasType() bool`

HasType returns a boolean if a field has been set.

### GetAll

`func (o *ExtractRequestExtractRulesValue) GetAll() bool`

GetAll returns the All field if non-nil, zero value otherwise.

### GetAllOk

`func (o *ExtractRequestExtractRulesValue) GetAllOk() (*bool, bool)`

GetAllOk returns a tuple with the All field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAll

`func (o *ExtractRequestExtractRulesValue) SetAll(v bool)`

SetAll sets All field to given value.

### HasAll

`func (o *ExtractRequestExtractRulesValue) HasAll() bool`

HasAll returns a boolean if a field has been set.

### GetOutput

`func (o *ExtractRequestExtractRulesValue) GetOutput() string`

GetOutput returns the Output field if non-nil, zero value otherwise.

### GetOutputOk

`func (o *ExtractRequestExtractRulesValue) GetOutputOk() (*string, bool)`

GetOutputOk returns a tuple with the Output field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOutput

`func (o *ExtractRequestExtractRulesValue) SetOutput(v string)`

SetOutput sets Output field to given value.

### HasOutput

`func (o *ExtractRequestExtractRulesValue) HasOutput() bool`

HasOutput returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



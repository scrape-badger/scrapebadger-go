# PriceValue

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Value** | Pointer to **NullableFloat32** |  | [optional] 
**Text** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewPriceValue

`func NewPriceValue() *PriceValue`

NewPriceValue instantiates a new PriceValue object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPriceValueWithDefaults

`func NewPriceValueWithDefaults() *PriceValue`

NewPriceValueWithDefaults instantiates a new PriceValue object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetValue

`func (o *PriceValue) GetValue() float32`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *PriceValue) GetValueOk() (*float32, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *PriceValue) SetValue(v float32)`

SetValue sets Value field to given value.

### HasValue

`func (o *PriceValue) HasValue() bool`

HasValue returns a boolean if a field has been set.

### SetValueNil

`func (o *PriceValue) SetValueNil(b bool)`

 SetValueNil sets the value for Value to be an explicit nil

### UnsetValue
`func (o *PriceValue) UnsetValue()`

UnsetValue ensures that no value is present for Value, not even an explicit nil
### GetText

`func (o *PriceValue) GetText() string`

GetText returns the Text field if non-nil, zero value otherwise.

### GetTextOk

`func (o *PriceValue) GetTextOk() (*string, bool)`

GetTextOk returns a tuple with the Text field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetText

`func (o *PriceValue) SetText(v string)`

SetText sets Text field to given value.

### HasText

`func (o *PriceValue) HasText() bool`

HasText returns a boolean if a field has been set.

### SetTextNil

`func (o *PriceValue) SetTextNil(b bool)`

 SetTextNil sets the value for Text to be an explicit nil

### UnsetText
`func (o *PriceValue) UnsetText()`

UnsetText ensures that no value is present for Text, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



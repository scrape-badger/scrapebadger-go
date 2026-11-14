# RufusAskRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Prompt** | **string** |  | 
**Asin** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewRufusAskRequest

`func NewRufusAskRequest(prompt string, ) *RufusAskRequest`

NewRufusAskRequest instantiates a new RufusAskRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRufusAskRequestWithDefaults

`func NewRufusAskRequestWithDefaults() *RufusAskRequest`

NewRufusAskRequestWithDefaults instantiates a new RufusAskRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPrompt

`func (o *RufusAskRequest) GetPrompt() string`

GetPrompt returns the Prompt field if non-nil, zero value otherwise.

### GetPromptOk

`func (o *RufusAskRequest) GetPromptOk() (*string, bool)`

GetPromptOk returns a tuple with the Prompt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrompt

`func (o *RufusAskRequest) SetPrompt(v string)`

SetPrompt sets Prompt field to given value.


### GetAsin

`func (o *RufusAskRequest) GetAsin() string`

GetAsin returns the Asin field if non-nil, zero value otherwise.

### GetAsinOk

`func (o *RufusAskRequest) GetAsinOk() (*string, bool)`

GetAsinOk returns a tuple with the Asin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAsin

`func (o *RufusAskRequest) SetAsin(v string)`

SetAsin sets Asin field to given value.

### HasAsin

`func (o *RufusAskRequest) HasAsin() bool`

HasAsin returns a boolean if a field has been set.

### SetAsinNil

`func (o *RufusAskRequest) SetAsinNil(b bool)`

 SetAsinNil sets the value for Asin to be an explicit nil

### UnsetAsin
`func (o *RufusAskRequest) UnsetAsin()`

UnsetAsin ensures that no value is present for Asin, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



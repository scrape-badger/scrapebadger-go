# BraveLocalesResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Countries** | [**[]BraveLocaleOption**](BraveLocaleOption.md) |  | 
**UiLanguages** | [**[]BraveLocaleOption**](BraveLocaleOption.md) |  | 

## Methods

### NewBraveLocalesResponse

`func NewBraveLocalesResponse(countries []BraveLocaleOption, uiLanguages []BraveLocaleOption, ) *BraveLocalesResponse`

NewBraveLocalesResponse instantiates a new BraveLocalesResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBraveLocalesResponseWithDefaults

`func NewBraveLocalesResponseWithDefaults() *BraveLocalesResponse`

NewBraveLocalesResponseWithDefaults instantiates a new BraveLocalesResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCountries

`func (o *BraveLocalesResponse) GetCountries() []BraveLocaleOption`

GetCountries returns the Countries field if non-nil, zero value otherwise.

### GetCountriesOk

`func (o *BraveLocalesResponse) GetCountriesOk() (*[]BraveLocaleOption, bool)`

GetCountriesOk returns a tuple with the Countries field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountries

`func (o *BraveLocalesResponse) SetCountries(v []BraveLocaleOption)`

SetCountries sets Countries field to given value.


### GetUiLanguages

`func (o *BraveLocalesResponse) GetUiLanguages() []BraveLocaleOption`

GetUiLanguages returns the UiLanguages field if non-nil, zero value otherwise.

### GetUiLanguagesOk

`func (o *BraveLocalesResponse) GetUiLanguagesOk() (*[]BraveLocaleOption, bool)`

GetUiLanguagesOk returns a tuple with the UiLanguages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUiLanguages

`func (o *BraveLocalesResponse) SetUiLanguages(v []BraveLocaleOption)`

SetUiLanguages sets UiLanguages field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



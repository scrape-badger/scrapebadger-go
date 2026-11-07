# BraveAutocompleteResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Query** | **string** |  | 
**Country** | **string** |  | 
**Suggestions** | [**[]BraveSuggestion**](BraveSuggestion.md) |  | 
**ResultCount** | **int32** |  | 
**SourceUrl** | **string** |  | 
**FetchedAt** | **string** |  | 
**FetchedUtc** | **float32** |  | 

## Methods

### NewBraveAutocompleteResponse

`func NewBraveAutocompleteResponse(query string, country string, suggestions []BraveSuggestion, resultCount int32, sourceUrl string, fetchedAt string, fetchedUtc float32, ) *BraveAutocompleteResponse`

NewBraveAutocompleteResponse instantiates a new BraveAutocompleteResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBraveAutocompleteResponseWithDefaults

`func NewBraveAutocompleteResponseWithDefaults() *BraveAutocompleteResponse`

NewBraveAutocompleteResponseWithDefaults instantiates a new BraveAutocompleteResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetQuery

`func (o *BraveAutocompleteResponse) GetQuery() string`

GetQuery returns the Query field if non-nil, zero value otherwise.

### GetQueryOk

`func (o *BraveAutocompleteResponse) GetQueryOk() (*string, bool)`

GetQueryOk returns a tuple with the Query field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuery

`func (o *BraveAutocompleteResponse) SetQuery(v string)`

SetQuery sets Query field to given value.


### GetCountry

`func (o *BraveAutocompleteResponse) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *BraveAutocompleteResponse) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *BraveAutocompleteResponse) SetCountry(v string)`

SetCountry sets Country field to given value.


### GetSuggestions

`func (o *BraveAutocompleteResponse) GetSuggestions() []BraveSuggestion`

GetSuggestions returns the Suggestions field if non-nil, zero value otherwise.

### GetSuggestionsOk

`func (o *BraveAutocompleteResponse) GetSuggestionsOk() (*[]BraveSuggestion, bool)`

GetSuggestionsOk returns a tuple with the Suggestions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuggestions

`func (o *BraveAutocompleteResponse) SetSuggestions(v []BraveSuggestion)`

SetSuggestions sets Suggestions field to given value.


### GetResultCount

`func (o *BraveAutocompleteResponse) GetResultCount() int32`

GetResultCount returns the ResultCount field if non-nil, zero value otherwise.

### GetResultCountOk

`func (o *BraveAutocompleteResponse) GetResultCountOk() (*int32, bool)`

GetResultCountOk returns a tuple with the ResultCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResultCount

`func (o *BraveAutocompleteResponse) SetResultCount(v int32)`

SetResultCount sets ResultCount field to given value.


### GetSourceUrl

`func (o *BraveAutocompleteResponse) GetSourceUrl() string`

GetSourceUrl returns the SourceUrl field if non-nil, zero value otherwise.

### GetSourceUrlOk

`func (o *BraveAutocompleteResponse) GetSourceUrlOk() (*string, bool)`

GetSourceUrlOk returns a tuple with the SourceUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceUrl

`func (o *BraveAutocompleteResponse) SetSourceUrl(v string)`

SetSourceUrl sets SourceUrl field to given value.


### GetFetchedAt

`func (o *BraveAutocompleteResponse) GetFetchedAt() string`

GetFetchedAt returns the FetchedAt field if non-nil, zero value otherwise.

### GetFetchedAtOk

`func (o *BraveAutocompleteResponse) GetFetchedAtOk() (*string, bool)`

GetFetchedAtOk returns a tuple with the FetchedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFetchedAt

`func (o *BraveAutocompleteResponse) SetFetchedAt(v string)`

SetFetchedAt sets FetchedAt field to given value.


### GetFetchedUtc

`func (o *BraveAutocompleteResponse) GetFetchedUtc() float32`

GetFetchedUtc returns the FetchedUtc field if non-nil, zero value otherwise.

### GetFetchedUtcOk

`func (o *BraveAutocompleteResponse) GetFetchedUtcOk() (*float32, bool)`

GetFetchedUtcOk returns a tuple with the FetchedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFetchedUtc

`func (o *BraveAutocompleteResponse) SetFetchedUtc(v float32)`

SetFetchedUtc sets FetchedUtc field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# BraveResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Query** | **string** |  | 
**Country** | **string** |  | 
**UiLanguage** | **string** |  | 
**SafeSearch** | **string** |  | 
**ResultCount** | **int32** |  | 
**Results** | [**[]BraveResult**](BraveResult.md) |  | 
**QueryInfo** | **map[string]interface{}** |  | 
**SourceUrl** | **string** |  | 
**FetchedAt** | **string** |  | 
**FetchedUtc** | **float32** |  | 

## Methods

### NewBraveResponse

`func NewBraveResponse(query string, country string, uiLanguage string, safeSearch string, resultCount int32, results []BraveResult, queryInfo map[string]interface{}, sourceUrl string, fetchedAt string, fetchedUtc float32, ) *BraveResponse`

NewBraveResponse instantiates a new BraveResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBraveResponseWithDefaults

`func NewBraveResponseWithDefaults() *BraveResponse`

NewBraveResponseWithDefaults instantiates a new BraveResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetQuery

`func (o *BraveResponse) GetQuery() string`

GetQuery returns the Query field if non-nil, zero value otherwise.

### GetQueryOk

`func (o *BraveResponse) GetQueryOk() (*string, bool)`

GetQueryOk returns a tuple with the Query field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuery

`func (o *BraveResponse) SetQuery(v string)`

SetQuery sets Query field to given value.


### GetCountry

`func (o *BraveResponse) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *BraveResponse) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *BraveResponse) SetCountry(v string)`

SetCountry sets Country field to given value.


### GetUiLanguage

`func (o *BraveResponse) GetUiLanguage() string`

GetUiLanguage returns the UiLanguage field if non-nil, zero value otherwise.

### GetUiLanguageOk

`func (o *BraveResponse) GetUiLanguageOk() (*string, bool)`

GetUiLanguageOk returns a tuple with the UiLanguage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUiLanguage

`func (o *BraveResponse) SetUiLanguage(v string)`

SetUiLanguage sets UiLanguage field to given value.


### GetSafeSearch

`func (o *BraveResponse) GetSafeSearch() string`

GetSafeSearch returns the SafeSearch field if non-nil, zero value otherwise.

### GetSafeSearchOk

`func (o *BraveResponse) GetSafeSearchOk() (*string, bool)`

GetSafeSearchOk returns a tuple with the SafeSearch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSafeSearch

`func (o *BraveResponse) SetSafeSearch(v string)`

SetSafeSearch sets SafeSearch field to given value.


### GetResultCount

`func (o *BraveResponse) GetResultCount() int32`

GetResultCount returns the ResultCount field if non-nil, zero value otherwise.

### GetResultCountOk

`func (o *BraveResponse) GetResultCountOk() (*int32, bool)`

GetResultCountOk returns a tuple with the ResultCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResultCount

`func (o *BraveResponse) SetResultCount(v int32)`

SetResultCount sets ResultCount field to given value.


### GetResults

`func (o *BraveResponse) GetResults() []BraveResult`

GetResults returns the Results field if non-nil, zero value otherwise.

### GetResultsOk

`func (o *BraveResponse) GetResultsOk() (*[]BraveResult, bool)`

GetResultsOk returns a tuple with the Results field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResults

`func (o *BraveResponse) SetResults(v []BraveResult)`

SetResults sets Results field to given value.


### GetQueryInfo

`func (o *BraveResponse) GetQueryInfo() map[string]interface{}`

GetQueryInfo returns the QueryInfo field if non-nil, zero value otherwise.

### GetQueryInfoOk

`func (o *BraveResponse) GetQueryInfoOk() (*map[string]interface{}, bool)`

GetQueryInfoOk returns a tuple with the QueryInfo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueryInfo

`func (o *BraveResponse) SetQueryInfo(v map[string]interface{})`

SetQueryInfo sets QueryInfo field to given value.


### GetSourceUrl

`func (o *BraveResponse) GetSourceUrl() string`

GetSourceUrl returns the SourceUrl field if non-nil, zero value otherwise.

### GetSourceUrlOk

`func (o *BraveResponse) GetSourceUrlOk() (*string, bool)`

GetSourceUrlOk returns a tuple with the SourceUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceUrl

`func (o *BraveResponse) SetSourceUrl(v string)`

SetSourceUrl sets SourceUrl field to given value.


### GetFetchedAt

`func (o *BraveResponse) GetFetchedAt() string`

GetFetchedAt returns the FetchedAt field if non-nil, zero value otherwise.

### GetFetchedAtOk

`func (o *BraveResponse) GetFetchedAtOk() (*string, bool)`

GetFetchedAtOk returns a tuple with the FetchedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFetchedAt

`func (o *BraveResponse) SetFetchedAt(v string)`

SetFetchedAt sets FetchedAt field to given value.


### GetFetchedUtc

`func (o *BraveResponse) GetFetchedUtc() float32`

GetFetchedUtc returns the FetchedUtc field if non-nil, zero value otherwise.

### GetFetchedUtcOk

`func (o *BraveResponse) GetFetchedUtcOk() (*float32, bool)`

GetFetchedUtcOk returns a tuple with the FetchedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFetchedUtc

`func (o *BraveResponse) SetFetchedUtc(v float32)`

SetFetchedUtc sets FetchedUtc field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



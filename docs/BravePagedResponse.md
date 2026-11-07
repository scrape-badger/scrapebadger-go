# BravePagedResponse

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
**Page** | **int32** |  | 
**HasNext** | **bool** |  | 
**NextPage** | Pointer to [**NullableNextPage**](NextPage.md) |  | [optional] 

## Methods

### NewBravePagedResponse

`func NewBravePagedResponse(query string, country string, uiLanguage string, safeSearch string, resultCount int32, results []BraveResult, queryInfo map[string]interface{}, sourceUrl string, fetchedAt string, fetchedUtc float32, page int32, hasNext bool, ) *BravePagedResponse`

NewBravePagedResponse instantiates a new BravePagedResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBravePagedResponseWithDefaults

`func NewBravePagedResponseWithDefaults() *BravePagedResponse`

NewBravePagedResponseWithDefaults instantiates a new BravePagedResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetQuery

`func (o *BravePagedResponse) GetQuery() string`

GetQuery returns the Query field if non-nil, zero value otherwise.

### GetQueryOk

`func (o *BravePagedResponse) GetQueryOk() (*string, bool)`

GetQueryOk returns a tuple with the Query field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuery

`func (o *BravePagedResponse) SetQuery(v string)`

SetQuery sets Query field to given value.


### GetCountry

`func (o *BravePagedResponse) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *BravePagedResponse) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *BravePagedResponse) SetCountry(v string)`

SetCountry sets Country field to given value.


### GetUiLanguage

`func (o *BravePagedResponse) GetUiLanguage() string`

GetUiLanguage returns the UiLanguage field if non-nil, zero value otherwise.

### GetUiLanguageOk

`func (o *BravePagedResponse) GetUiLanguageOk() (*string, bool)`

GetUiLanguageOk returns a tuple with the UiLanguage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUiLanguage

`func (o *BravePagedResponse) SetUiLanguage(v string)`

SetUiLanguage sets UiLanguage field to given value.


### GetSafeSearch

`func (o *BravePagedResponse) GetSafeSearch() string`

GetSafeSearch returns the SafeSearch field if non-nil, zero value otherwise.

### GetSafeSearchOk

`func (o *BravePagedResponse) GetSafeSearchOk() (*string, bool)`

GetSafeSearchOk returns a tuple with the SafeSearch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSafeSearch

`func (o *BravePagedResponse) SetSafeSearch(v string)`

SetSafeSearch sets SafeSearch field to given value.


### GetResultCount

`func (o *BravePagedResponse) GetResultCount() int32`

GetResultCount returns the ResultCount field if non-nil, zero value otherwise.

### GetResultCountOk

`func (o *BravePagedResponse) GetResultCountOk() (*int32, bool)`

GetResultCountOk returns a tuple with the ResultCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResultCount

`func (o *BravePagedResponse) SetResultCount(v int32)`

SetResultCount sets ResultCount field to given value.


### GetResults

`func (o *BravePagedResponse) GetResults() []BraveResult`

GetResults returns the Results field if non-nil, zero value otherwise.

### GetResultsOk

`func (o *BravePagedResponse) GetResultsOk() (*[]BraveResult, bool)`

GetResultsOk returns a tuple with the Results field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResults

`func (o *BravePagedResponse) SetResults(v []BraveResult)`

SetResults sets Results field to given value.


### GetQueryInfo

`func (o *BravePagedResponse) GetQueryInfo() map[string]interface{}`

GetQueryInfo returns the QueryInfo field if non-nil, zero value otherwise.

### GetQueryInfoOk

`func (o *BravePagedResponse) GetQueryInfoOk() (*map[string]interface{}, bool)`

GetQueryInfoOk returns a tuple with the QueryInfo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueryInfo

`func (o *BravePagedResponse) SetQueryInfo(v map[string]interface{})`

SetQueryInfo sets QueryInfo field to given value.


### GetSourceUrl

`func (o *BravePagedResponse) GetSourceUrl() string`

GetSourceUrl returns the SourceUrl field if non-nil, zero value otherwise.

### GetSourceUrlOk

`func (o *BravePagedResponse) GetSourceUrlOk() (*string, bool)`

GetSourceUrlOk returns a tuple with the SourceUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceUrl

`func (o *BravePagedResponse) SetSourceUrl(v string)`

SetSourceUrl sets SourceUrl field to given value.


### GetFetchedAt

`func (o *BravePagedResponse) GetFetchedAt() string`

GetFetchedAt returns the FetchedAt field if non-nil, zero value otherwise.

### GetFetchedAtOk

`func (o *BravePagedResponse) GetFetchedAtOk() (*string, bool)`

GetFetchedAtOk returns a tuple with the FetchedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFetchedAt

`func (o *BravePagedResponse) SetFetchedAt(v string)`

SetFetchedAt sets FetchedAt field to given value.


### GetFetchedUtc

`func (o *BravePagedResponse) GetFetchedUtc() float32`

GetFetchedUtc returns the FetchedUtc field if non-nil, zero value otherwise.

### GetFetchedUtcOk

`func (o *BravePagedResponse) GetFetchedUtcOk() (*float32, bool)`

GetFetchedUtcOk returns a tuple with the FetchedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFetchedUtc

`func (o *BravePagedResponse) SetFetchedUtc(v float32)`

SetFetchedUtc sets FetchedUtc field to given value.


### GetPage

`func (o *BravePagedResponse) GetPage() int32`

GetPage returns the Page field if non-nil, zero value otherwise.

### GetPageOk

`func (o *BravePagedResponse) GetPageOk() (*int32, bool)`

GetPageOk returns a tuple with the Page field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPage

`func (o *BravePagedResponse) SetPage(v int32)`

SetPage sets Page field to given value.


### GetHasNext

`func (o *BravePagedResponse) GetHasNext() bool`

GetHasNext returns the HasNext field if non-nil, zero value otherwise.

### GetHasNextOk

`func (o *BravePagedResponse) GetHasNextOk() (*bool, bool)`

GetHasNextOk returns a tuple with the HasNext field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasNext

`func (o *BravePagedResponse) SetHasNext(v bool)`

SetHasNext sets HasNext field to given value.


### GetNextPage

`func (o *BravePagedResponse) GetNextPage() NextPage`

GetNextPage returns the NextPage field if non-nil, zero value otherwise.

### GetNextPageOk

`func (o *BravePagedResponse) GetNextPageOk() (*NextPage, bool)`

GetNextPageOk returns a tuple with the NextPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPage

`func (o *BravePagedResponse) SetNextPage(v NextPage)`

SetNextPage sets NextPage field to given value.

### HasNextPage

`func (o *BravePagedResponse) HasNextPage() bool`

HasNextPage returns a boolean if a field has been set.

### SetNextPageNil

`func (o *BravePagedResponse) SetNextPageNil(b bool)`

 SetNextPageNil sets the value for NextPage to be an explicit nil

### UnsetNextPage
`func (o *BravePagedResponse) UnsetNextPage()`

UnsetNextPage ensures that no value is present for NextPage, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



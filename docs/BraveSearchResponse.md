# BraveSearchResponse

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
**Faq** | Pointer to **[]map[string]interface{}** |  | [optional] 
**Discussions** | Pointer to [**[]BraveResult**](BraveResult.md) |  | [optional] 
**Videos** | Pointer to [**[]BraveResult**](BraveResult.md) |  | [optional] 
**News** | Pointer to [**[]BraveResult**](BraveResult.md) |  | [optional] 
**Images** | Pointer to [**[]BraveResult**](BraveResult.md) |  | [optional] 
**RelatedSearches** | Pointer to **[]map[string]string** |  | [optional] 
**RichBlocks** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewBraveSearchResponse

`func NewBraveSearchResponse(query string, country string, uiLanguage string, safeSearch string, resultCount int32, results []BraveResult, queryInfo map[string]interface{}, sourceUrl string, fetchedAt string, fetchedUtc float32, page int32, hasNext bool, ) *BraveSearchResponse`

NewBraveSearchResponse instantiates a new BraveSearchResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBraveSearchResponseWithDefaults

`func NewBraveSearchResponseWithDefaults() *BraveSearchResponse`

NewBraveSearchResponseWithDefaults instantiates a new BraveSearchResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetQuery

`func (o *BraveSearchResponse) GetQuery() string`

GetQuery returns the Query field if non-nil, zero value otherwise.

### GetQueryOk

`func (o *BraveSearchResponse) GetQueryOk() (*string, bool)`

GetQueryOk returns a tuple with the Query field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuery

`func (o *BraveSearchResponse) SetQuery(v string)`

SetQuery sets Query field to given value.


### GetCountry

`func (o *BraveSearchResponse) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *BraveSearchResponse) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *BraveSearchResponse) SetCountry(v string)`

SetCountry sets Country field to given value.


### GetUiLanguage

`func (o *BraveSearchResponse) GetUiLanguage() string`

GetUiLanguage returns the UiLanguage field if non-nil, zero value otherwise.

### GetUiLanguageOk

`func (o *BraveSearchResponse) GetUiLanguageOk() (*string, bool)`

GetUiLanguageOk returns a tuple with the UiLanguage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUiLanguage

`func (o *BraveSearchResponse) SetUiLanguage(v string)`

SetUiLanguage sets UiLanguage field to given value.


### GetSafeSearch

`func (o *BraveSearchResponse) GetSafeSearch() string`

GetSafeSearch returns the SafeSearch field if non-nil, zero value otherwise.

### GetSafeSearchOk

`func (o *BraveSearchResponse) GetSafeSearchOk() (*string, bool)`

GetSafeSearchOk returns a tuple with the SafeSearch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSafeSearch

`func (o *BraveSearchResponse) SetSafeSearch(v string)`

SetSafeSearch sets SafeSearch field to given value.


### GetResultCount

`func (o *BraveSearchResponse) GetResultCount() int32`

GetResultCount returns the ResultCount field if non-nil, zero value otherwise.

### GetResultCountOk

`func (o *BraveSearchResponse) GetResultCountOk() (*int32, bool)`

GetResultCountOk returns a tuple with the ResultCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResultCount

`func (o *BraveSearchResponse) SetResultCount(v int32)`

SetResultCount sets ResultCount field to given value.


### GetResults

`func (o *BraveSearchResponse) GetResults() []BraveResult`

GetResults returns the Results field if non-nil, zero value otherwise.

### GetResultsOk

`func (o *BraveSearchResponse) GetResultsOk() (*[]BraveResult, bool)`

GetResultsOk returns a tuple with the Results field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResults

`func (o *BraveSearchResponse) SetResults(v []BraveResult)`

SetResults sets Results field to given value.


### GetQueryInfo

`func (o *BraveSearchResponse) GetQueryInfo() map[string]interface{}`

GetQueryInfo returns the QueryInfo field if non-nil, zero value otherwise.

### GetQueryInfoOk

`func (o *BraveSearchResponse) GetQueryInfoOk() (*map[string]interface{}, bool)`

GetQueryInfoOk returns a tuple with the QueryInfo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueryInfo

`func (o *BraveSearchResponse) SetQueryInfo(v map[string]interface{})`

SetQueryInfo sets QueryInfo field to given value.


### GetSourceUrl

`func (o *BraveSearchResponse) GetSourceUrl() string`

GetSourceUrl returns the SourceUrl field if non-nil, zero value otherwise.

### GetSourceUrlOk

`func (o *BraveSearchResponse) GetSourceUrlOk() (*string, bool)`

GetSourceUrlOk returns a tuple with the SourceUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceUrl

`func (o *BraveSearchResponse) SetSourceUrl(v string)`

SetSourceUrl sets SourceUrl field to given value.


### GetFetchedAt

`func (o *BraveSearchResponse) GetFetchedAt() string`

GetFetchedAt returns the FetchedAt field if non-nil, zero value otherwise.

### GetFetchedAtOk

`func (o *BraveSearchResponse) GetFetchedAtOk() (*string, bool)`

GetFetchedAtOk returns a tuple with the FetchedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFetchedAt

`func (o *BraveSearchResponse) SetFetchedAt(v string)`

SetFetchedAt sets FetchedAt field to given value.


### GetFetchedUtc

`func (o *BraveSearchResponse) GetFetchedUtc() float32`

GetFetchedUtc returns the FetchedUtc field if non-nil, zero value otherwise.

### GetFetchedUtcOk

`func (o *BraveSearchResponse) GetFetchedUtcOk() (*float32, bool)`

GetFetchedUtcOk returns a tuple with the FetchedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFetchedUtc

`func (o *BraveSearchResponse) SetFetchedUtc(v float32)`

SetFetchedUtc sets FetchedUtc field to given value.


### GetPage

`func (o *BraveSearchResponse) GetPage() int32`

GetPage returns the Page field if non-nil, zero value otherwise.

### GetPageOk

`func (o *BraveSearchResponse) GetPageOk() (*int32, bool)`

GetPageOk returns a tuple with the Page field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPage

`func (o *BraveSearchResponse) SetPage(v int32)`

SetPage sets Page field to given value.


### GetHasNext

`func (o *BraveSearchResponse) GetHasNext() bool`

GetHasNext returns the HasNext field if non-nil, zero value otherwise.

### GetHasNextOk

`func (o *BraveSearchResponse) GetHasNextOk() (*bool, bool)`

GetHasNextOk returns a tuple with the HasNext field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasNext

`func (o *BraveSearchResponse) SetHasNext(v bool)`

SetHasNext sets HasNext field to given value.


### GetNextPage

`func (o *BraveSearchResponse) GetNextPage() NextPage`

GetNextPage returns the NextPage field if non-nil, zero value otherwise.

### GetNextPageOk

`func (o *BraveSearchResponse) GetNextPageOk() (*NextPage, bool)`

GetNextPageOk returns a tuple with the NextPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPage

`func (o *BraveSearchResponse) SetNextPage(v NextPage)`

SetNextPage sets NextPage field to given value.

### HasNextPage

`func (o *BraveSearchResponse) HasNextPage() bool`

HasNextPage returns a boolean if a field has been set.

### SetNextPageNil

`func (o *BraveSearchResponse) SetNextPageNil(b bool)`

 SetNextPageNil sets the value for NextPage to be an explicit nil

### UnsetNextPage
`func (o *BraveSearchResponse) UnsetNextPage()`

UnsetNextPage ensures that no value is present for NextPage, not even an explicit nil
### GetFaq

`func (o *BraveSearchResponse) GetFaq() []*map[string]interface{}`

GetFaq returns the Faq field if non-nil, zero value otherwise.

### GetFaqOk

`func (o *BraveSearchResponse) GetFaqOk() (*[]*map[string]interface{}, bool)`

GetFaqOk returns a tuple with the Faq field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFaq

`func (o *BraveSearchResponse) SetFaq(v []*map[string]interface{})`

SetFaq sets Faq field to given value.

### HasFaq

`func (o *BraveSearchResponse) HasFaq() bool`

HasFaq returns a boolean if a field has been set.

### GetDiscussions

`func (o *BraveSearchResponse) GetDiscussions() []BraveResult`

GetDiscussions returns the Discussions field if non-nil, zero value otherwise.

### GetDiscussionsOk

`func (o *BraveSearchResponse) GetDiscussionsOk() (*[]BraveResult, bool)`

GetDiscussionsOk returns a tuple with the Discussions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiscussions

`func (o *BraveSearchResponse) SetDiscussions(v []BraveResult)`

SetDiscussions sets Discussions field to given value.

### HasDiscussions

`func (o *BraveSearchResponse) HasDiscussions() bool`

HasDiscussions returns a boolean if a field has been set.

### GetVideos

`func (o *BraveSearchResponse) GetVideos() []BraveResult`

GetVideos returns the Videos field if non-nil, zero value otherwise.

### GetVideosOk

`func (o *BraveSearchResponse) GetVideosOk() (*[]BraveResult, bool)`

GetVideosOk returns a tuple with the Videos field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVideos

`func (o *BraveSearchResponse) SetVideos(v []BraveResult)`

SetVideos sets Videos field to given value.

### HasVideos

`func (o *BraveSearchResponse) HasVideos() bool`

HasVideos returns a boolean if a field has been set.

### GetNews

`func (o *BraveSearchResponse) GetNews() []BraveResult`

GetNews returns the News field if non-nil, zero value otherwise.

### GetNewsOk

`func (o *BraveSearchResponse) GetNewsOk() (*[]BraveResult, bool)`

GetNewsOk returns a tuple with the News field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNews

`func (o *BraveSearchResponse) SetNews(v []BraveResult)`

SetNews sets News field to given value.

### HasNews

`func (o *BraveSearchResponse) HasNews() bool`

HasNews returns a boolean if a field has been set.

### GetImages

`func (o *BraveSearchResponse) GetImages() []BraveResult`

GetImages returns the Images field if non-nil, zero value otherwise.

### GetImagesOk

`func (o *BraveSearchResponse) GetImagesOk() (*[]BraveResult, bool)`

GetImagesOk returns a tuple with the Images field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImages

`func (o *BraveSearchResponse) SetImages(v []BraveResult)`

SetImages sets Images field to given value.

### HasImages

`func (o *BraveSearchResponse) HasImages() bool`

HasImages returns a boolean if a field has been set.

### GetRelatedSearches

`func (o *BraveSearchResponse) GetRelatedSearches() []map[string]string`

GetRelatedSearches returns the RelatedSearches field if non-nil, zero value otherwise.

### GetRelatedSearchesOk

`func (o *BraveSearchResponse) GetRelatedSearchesOk() (*[]map[string]string, bool)`

GetRelatedSearchesOk returns a tuple with the RelatedSearches field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRelatedSearches

`func (o *BraveSearchResponse) SetRelatedSearches(v []map[string]string)`

SetRelatedSearches sets RelatedSearches field to given value.

### HasRelatedSearches

`func (o *BraveSearchResponse) HasRelatedSearches() bool`

HasRelatedSearches returns a boolean if a field has been set.

### GetRichBlocks

`func (o *BraveSearchResponse) GetRichBlocks() map[string]interface{}`

GetRichBlocks returns the RichBlocks field if non-nil, zero value otherwise.

### GetRichBlocksOk

`func (o *BraveSearchResponse) GetRichBlocksOk() (*map[string]interface{}, bool)`

GetRichBlocksOk returns a tuple with the RichBlocks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRichBlocks

`func (o *BraveSearchResponse) SetRichBlocks(v map[string]interface{})`

SetRichBlocks sets RichBlocks field to given value.

### HasRichBlocks

`func (o *BraveSearchResponse) HasRichBlocks() bool`

HasRichBlocks returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



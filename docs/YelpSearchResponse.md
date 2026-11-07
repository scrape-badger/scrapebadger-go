# YelpSearchResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Market** | **string** |  | 
**Query** | **NullableString** |  | 
**Location** | **string** |  | 
**LocationResolved** | [**YelpResolvedLocation**](YelpResolvedLocation.md) |  | 
**DidYouMean** | Pointer to **NullableString** |  | [optional] 
**QueryMatched** | **bool** | False when Yelp could not place the query; results are then Yelp&#39;s broader ranking for the location, as Yelp shows them. | 
**TotalResults** | **int32** | Yelp&#39;s reported total; at most 110 are browsable. | 
**Page** | **int32** |  | 
**PageSize** | **int32** |  | 
**TotalPages** | **int32** |  | 
**HasNextPage** | **bool** |  | 
**NextPage** | Pointer to **NullableInt32** |  | [optional] 
**Results** | [**[]YelpBusiness**](YelpBusiness.md) |  | 
**Ads** | [**[]YelpBusiness**](YelpBusiness.md) |  | 
**Filters** | [**map[string]YelpFilterGroup**](YelpFilterGroup.md) |  | 
**RelatedSearches** | [**[]YelpLink**](YelpLink.md) |  | 
**SourceUrl** | **string** |  | 
**FetchedAt** | **string** |  | 
**FetchedUtc** | **float32** |  | 

## Methods

### NewYelpSearchResponse

`func NewYelpSearchResponse(market string, query NullableString, location string, locationResolved YelpResolvedLocation, queryMatched bool, totalResults int32, page int32, pageSize int32, totalPages int32, hasNextPage bool, results []YelpBusiness, ads []YelpBusiness, filters map[string]YelpFilterGroup, relatedSearches []YelpLink, sourceUrl string, fetchedAt string, fetchedUtc float32, ) *YelpSearchResponse`

NewYelpSearchResponse instantiates a new YelpSearchResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewYelpSearchResponseWithDefaults

`func NewYelpSearchResponseWithDefaults() *YelpSearchResponse`

NewYelpSearchResponseWithDefaults instantiates a new YelpSearchResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMarket

`func (o *YelpSearchResponse) GetMarket() string`

GetMarket returns the Market field if non-nil, zero value otherwise.

### GetMarketOk

`func (o *YelpSearchResponse) GetMarketOk() (*string, bool)`

GetMarketOk returns a tuple with the Market field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMarket

`func (o *YelpSearchResponse) SetMarket(v string)`

SetMarket sets Market field to given value.


### GetQuery

`func (o *YelpSearchResponse) GetQuery() string`

GetQuery returns the Query field if non-nil, zero value otherwise.

### GetQueryOk

`func (o *YelpSearchResponse) GetQueryOk() (*string, bool)`

GetQueryOk returns a tuple with the Query field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuery

`func (o *YelpSearchResponse) SetQuery(v string)`

SetQuery sets Query field to given value.


### SetQueryNil

`func (o *YelpSearchResponse) SetQueryNil(b bool)`

 SetQueryNil sets the value for Query to be an explicit nil

### UnsetQuery
`func (o *YelpSearchResponse) UnsetQuery()`

UnsetQuery ensures that no value is present for Query, not even an explicit nil
### GetLocation

`func (o *YelpSearchResponse) GetLocation() string`

GetLocation returns the Location field if non-nil, zero value otherwise.

### GetLocationOk

`func (o *YelpSearchResponse) GetLocationOk() (*string, bool)`

GetLocationOk returns a tuple with the Location field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocation

`func (o *YelpSearchResponse) SetLocation(v string)`

SetLocation sets Location field to given value.


### GetLocationResolved

`func (o *YelpSearchResponse) GetLocationResolved() YelpResolvedLocation`

GetLocationResolved returns the LocationResolved field if non-nil, zero value otherwise.

### GetLocationResolvedOk

`func (o *YelpSearchResponse) GetLocationResolvedOk() (*YelpResolvedLocation, bool)`

GetLocationResolvedOk returns a tuple with the LocationResolved field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocationResolved

`func (o *YelpSearchResponse) SetLocationResolved(v YelpResolvedLocation)`

SetLocationResolved sets LocationResolved field to given value.


### GetDidYouMean

`func (o *YelpSearchResponse) GetDidYouMean() string`

GetDidYouMean returns the DidYouMean field if non-nil, zero value otherwise.

### GetDidYouMeanOk

`func (o *YelpSearchResponse) GetDidYouMeanOk() (*string, bool)`

GetDidYouMeanOk returns a tuple with the DidYouMean field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDidYouMean

`func (o *YelpSearchResponse) SetDidYouMean(v string)`

SetDidYouMean sets DidYouMean field to given value.

### HasDidYouMean

`func (o *YelpSearchResponse) HasDidYouMean() bool`

HasDidYouMean returns a boolean if a field has been set.

### SetDidYouMeanNil

`func (o *YelpSearchResponse) SetDidYouMeanNil(b bool)`

 SetDidYouMeanNil sets the value for DidYouMean to be an explicit nil

### UnsetDidYouMean
`func (o *YelpSearchResponse) UnsetDidYouMean()`

UnsetDidYouMean ensures that no value is present for DidYouMean, not even an explicit nil
### GetQueryMatched

`func (o *YelpSearchResponse) GetQueryMatched() bool`

GetQueryMatched returns the QueryMatched field if non-nil, zero value otherwise.

### GetQueryMatchedOk

`func (o *YelpSearchResponse) GetQueryMatchedOk() (*bool, bool)`

GetQueryMatchedOk returns a tuple with the QueryMatched field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueryMatched

`func (o *YelpSearchResponse) SetQueryMatched(v bool)`

SetQueryMatched sets QueryMatched field to given value.


### GetTotalResults

`func (o *YelpSearchResponse) GetTotalResults() int32`

GetTotalResults returns the TotalResults field if non-nil, zero value otherwise.

### GetTotalResultsOk

`func (o *YelpSearchResponse) GetTotalResultsOk() (*int32, bool)`

GetTotalResultsOk returns a tuple with the TotalResults field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalResults

`func (o *YelpSearchResponse) SetTotalResults(v int32)`

SetTotalResults sets TotalResults field to given value.


### GetPage

`func (o *YelpSearchResponse) GetPage() int32`

GetPage returns the Page field if non-nil, zero value otherwise.

### GetPageOk

`func (o *YelpSearchResponse) GetPageOk() (*int32, bool)`

GetPageOk returns a tuple with the Page field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPage

`func (o *YelpSearchResponse) SetPage(v int32)`

SetPage sets Page field to given value.


### GetPageSize

`func (o *YelpSearchResponse) GetPageSize() int32`

GetPageSize returns the PageSize field if non-nil, zero value otherwise.

### GetPageSizeOk

`func (o *YelpSearchResponse) GetPageSizeOk() (*int32, bool)`

GetPageSizeOk returns a tuple with the PageSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageSize

`func (o *YelpSearchResponse) SetPageSize(v int32)`

SetPageSize sets PageSize field to given value.


### GetTotalPages

`func (o *YelpSearchResponse) GetTotalPages() int32`

GetTotalPages returns the TotalPages field if non-nil, zero value otherwise.

### GetTotalPagesOk

`func (o *YelpSearchResponse) GetTotalPagesOk() (*int32, bool)`

GetTotalPagesOk returns a tuple with the TotalPages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalPages

`func (o *YelpSearchResponse) SetTotalPages(v int32)`

SetTotalPages sets TotalPages field to given value.


### GetHasNextPage

`func (o *YelpSearchResponse) GetHasNextPage() bool`

GetHasNextPage returns the HasNextPage field if non-nil, zero value otherwise.

### GetHasNextPageOk

`func (o *YelpSearchResponse) GetHasNextPageOk() (*bool, bool)`

GetHasNextPageOk returns a tuple with the HasNextPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasNextPage

`func (o *YelpSearchResponse) SetHasNextPage(v bool)`

SetHasNextPage sets HasNextPage field to given value.


### GetNextPage

`func (o *YelpSearchResponse) GetNextPage() int32`

GetNextPage returns the NextPage field if non-nil, zero value otherwise.

### GetNextPageOk

`func (o *YelpSearchResponse) GetNextPageOk() (*int32, bool)`

GetNextPageOk returns a tuple with the NextPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPage

`func (o *YelpSearchResponse) SetNextPage(v int32)`

SetNextPage sets NextPage field to given value.

### HasNextPage

`func (o *YelpSearchResponse) HasNextPage() bool`

HasNextPage returns a boolean if a field has been set.

### SetNextPageNil

`func (o *YelpSearchResponse) SetNextPageNil(b bool)`

 SetNextPageNil sets the value for NextPage to be an explicit nil

### UnsetNextPage
`func (o *YelpSearchResponse) UnsetNextPage()`

UnsetNextPage ensures that no value is present for NextPage, not even an explicit nil
### GetResults

`func (o *YelpSearchResponse) GetResults() []YelpBusiness`

GetResults returns the Results field if non-nil, zero value otherwise.

### GetResultsOk

`func (o *YelpSearchResponse) GetResultsOk() (*[]YelpBusiness, bool)`

GetResultsOk returns a tuple with the Results field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResults

`func (o *YelpSearchResponse) SetResults(v []YelpBusiness)`

SetResults sets Results field to given value.


### GetAds

`func (o *YelpSearchResponse) GetAds() []YelpBusiness`

GetAds returns the Ads field if non-nil, zero value otherwise.

### GetAdsOk

`func (o *YelpSearchResponse) GetAdsOk() (*[]YelpBusiness, bool)`

GetAdsOk returns a tuple with the Ads field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAds

`func (o *YelpSearchResponse) SetAds(v []YelpBusiness)`

SetAds sets Ads field to given value.


### GetFilters

`func (o *YelpSearchResponse) GetFilters() map[string]YelpFilterGroup`

GetFilters returns the Filters field if non-nil, zero value otherwise.

### GetFiltersOk

`func (o *YelpSearchResponse) GetFiltersOk() (*map[string]YelpFilterGroup, bool)`

GetFiltersOk returns a tuple with the Filters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilters

`func (o *YelpSearchResponse) SetFilters(v map[string]YelpFilterGroup)`

SetFilters sets Filters field to given value.


### GetRelatedSearches

`func (o *YelpSearchResponse) GetRelatedSearches() []YelpLink`

GetRelatedSearches returns the RelatedSearches field if non-nil, zero value otherwise.

### GetRelatedSearchesOk

`func (o *YelpSearchResponse) GetRelatedSearchesOk() (*[]YelpLink, bool)`

GetRelatedSearchesOk returns a tuple with the RelatedSearches field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRelatedSearches

`func (o *YelpSearchResponse) SetRelatedSearches(v []YelpLink)`

SetRelatedSearches sets RelatedSearches field to given value.


### GetSourceUrl

`func (o *YelpSearchResponse) GetSourceUrl() string`

GetSourceUrl returns the SourceUrl field if non-nil, zero value otherwise.

### GetSourceUrlOk

`func (o *YelpSearchResponse) GetSourceUrlOk() (*string, bool)`

GetSourceUrlOk returns a tuple with the SourceUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceUrl

`func (o *YelpSearchResponse) SetSourceUrl(v string)`

SetSourceUrl sets SourceUrl field to given value.


### GetFetchedAt

`func (o *YelpSearchResponse) GetFetchedAt() string`

GetFetchedAt returns the FetchedAt field if non-nil, zero value otherwise.

### GetFetchedAtOk

`func (o *YelpSearchResponse) GetFetchedAtOk() (*string, bool)`

GetFetchedAtOk returns a tuple with the FetchedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFetchedAt

`func (o *YelpSearchResponse) SetFetchedAt(v string)`

SetFetchedAt sets FetchedAt field to given value.


### GetFetchedUtc

`func (o *YelpSearchResponse) GetFetchedUtc() float32`

GetFetchedUtc returns the FetchedUtc field if non-nil, zero value otherwise.

### GetFetchedUtcOk

`func (o *YelpSearchResponse) GetFetchedUtcOk() (*float32, bool)`

GetFetchedUtcOk returns a tuple with the FetchedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFetchedUtc

`func (o *YelpSearchResponse) SetFetchedUtc(v float32)`

SetFetchedUtc sets FetchedUtc field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



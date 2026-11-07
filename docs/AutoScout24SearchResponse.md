# AutoScout24SearchResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Market** | **string** |  | 
**SourceUrl** | **string** |  | 
**TotalResults** | **int32** |  | 
**TotalPages** | **int32** |  | 
**Page** | **int32** |  | 
**PageSize** | Pointer to **int32** |  | [optional] [default to 20]
**HasNextPage** | **bool** |  | 
**NextPage** | **NullableInt32** |  | 
**PaginationCap** | Pointer to **int32** |  | [optional] [default to 200]
**Results** | [**[]AutoScout24Listing**](AutoScout24Listing.md) |  | 
**Filters** | **map[string]interface{}** |  | 
**AppliedFilters** | **map[string]interface{}** |  | 
**LatencyMs** | **int32** |  | 

## Methods

### NewAutoScout24SearchResponse

`func NewAutoScout24SearchResponse(market string, sourceUrl string, totalResults int32, totalPages int32, page int32, hasNextPage bool, nextPage NullableInt32, results []AutoScout24Listing, filters map[string]interface{}, appliedFilters map[string]interface{}, latencyMs int32, ) *AutoScout24SearchResponse`

NewAutoScout24SearchResponse instantiates a new AutoScout24SearchResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAutoScout24SearchResponseWithDefaults

`func NewAutoScout24SearchResponseWithDefaults() *AutoScout24SearchResponse`

NewAutoScout24SearchResponseWithDefaults instantiates a new AutoScout24SearchResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMarket

`func (o *AutoScout24SearchResponse) GetMarket() string`

GetMarket returns the Market field if non-nil, zero value otherwise.

### GetMarketOk

`func (o *AutoScout24SearchResponse) GetMarketOk() (*string, bool)`

GetMarketOk returns a tuple with the Market field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMarket

`func (o *AutoScout24SearchResponse) SetMarket(v string)`

SetMarket sets Market field to given value.


### GetSourceUrl

`func (o *AutoScout24SearchResponse) GetSourceUrl() string`

GetSourceUrl returns the SourceUrl field if non-nil, zero value otherwise.

### GetSourceUrlOk

`func (o *AutoScout24SearchResponse) GetSourceUrlOk() (*string, bool)`

GetSourceUrlOk returns a tuple with the SourceUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceUrl

`func (o *AutoScout24SearchResponse) SetSourceUrl(v string)`

SetSourceUrl sets SourceUrl field to given value.


### GetTotalResults

`func (o *AutoScout24SearchResponse) GetTotalResults() int32`

GetTotalResults returns the TotalResults field if non-nil, zero value otherwise.

### GetTotalResultsOk

`func (o *AutoScout24SearchResponse) GetTotalResultsOk() (*int32, bool)`

GetTotalResultsOk returns a tuple with the TotalResults field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalResults

`func (o *AutoScout24SearchResponse) SetTotalResults(v int32)`

SetTotalResults sets TotalResults field to given value.


### GetTotalPages

`func (o *AutoScout24SearchResponse) GetTotalPages() int32`

GetTotalPages returns the TotalPages field if non-nil, zero value otherwise.

### GetTotalPagesOk

`func (o *AutoScout24SearchResponse) GetTotalPagesOk() (*int32, bool)`

GetTotalPagesOk returns a tuple with the TotalPages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalPages

`func (o *AutoScout24SearchResponse) SetTotalPages(v int32)`

SetTotalPages sets TotalPages field to given value.


### GetPage

`func (o *AutoScout24SearchResponse) GetPage() int32`

GetPage returns the Page field if non-nil, zero value otherwise.

### GetPageOk

`func (o *AutoScout24SearchResponse) GetPageOk() (*int32, bool)`

GetPageOk returns a tuple with the Page field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPage

`func (o *AutoScout24SearchResponse) SetPage(v int32)`

SetPage sets Page field to given value.


### GetPageSize

`func (o *AutoScout24SearchResponse) GetPageSize() int32`

GetPageSize returns the PageSize field if non-nil, zero value otherwise.

### GetPageSizeOk

`func (o *AutoScout24SearchResponse) GetPageSizeOk() (*int32, bool)`

GetPageSizeOk returns a tuple with the PageSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageSize

`func (o *AutoScout24SearchResponse) SetPageSize(v int32)`

SetPageSize sets PageSize field to given value.

### HasPageSize

`func (o *AutoScout24SearchResponse) HasPageSize() bool`

HasPageSize returns a boolean if a field has been set.

### GetHasNextPage

`func (o *AutoScout24SearchResponse) GetHasNextPage() bool`

GetHasNextPage returns the HasNextPage field if non-nil, zero value otherwise.

### GetHasNextPageOk

`func (o *AutoScout24SearchResponse) GetHasNextPageOk() (*bool, bool)`

GetHasNextPageOk returns a tuple with the HasNextPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasNextPage

`func (o *AutoScout24SearchResponse) SetHasNextPage(v bool)`

SetHasNextPage sets HasNextPage field to given value.


### GetNextPage

`func (o *AutoScout24SearchResponse) GetNextPage() int32`

GetNextPage returns the NextPage field if non-nil, zero value otherwise.

### GetNextPageOk

`func (o *AutoScout24SearchResponse) GetNextPageOk() (*int32, bool)`

GetNextPageOk returns a tuple with the NextPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPage

`func (o *AutoScout24SearchResponse) SetNextPage(v int32)`

SetNextPage sets NextPage field to given value.


### SetNextPageNil

`func (o *AutoScout24SearchResponse) SetNextPageNil(b bool)`

 SetNextPageNil sets the value for NextPage to be an explicit nil

### UnsetNextPage
`func (o *AutoScout24SearchResponse) UnsetNextPage()`

UnsetNextPage ensures that no value is present for NextPage, not even an explicit nil
### GetPaginationCap

`func (o *AutoScout24SearchResponse) GetPaginationCap() int32`

GetPaginationCap returns the PaginationCap field if non-nil, zero value otherwise.

### GetPaginationCapOk

`func (o *AutoScout24SearchResponse) GetPaginationCapOk() (*int32, bool)`

GetPaginationCapOk returns a tuple with the PaginationCap field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaginationCap

`func (o *AutoScout24SearchResponse) SetPaginationCap(v int32)`

SetPaginationCap sets PaginationCap field to given value.

### HasPaginationCap

`func (o *AutoScout24SearchResponse) HasPaginationCap() bool`

HasPaginationCap returns a boolean if a field has been set.

### GetResults

`func (o *AutoScout24SearchResponse) GetResults() []AutoScout24Listing`

GetResults returns the Results field if non-nil, zero value otherwise.

### GetResultsOk

`func (o *AutoScout24SearchResponse) GetResultsOk() (*[]AutoScout24Listing, bool)`

GetResultsOk returns a tuple with the Results field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResults

`func (o *AutoScout24SearchResponse) SetResults(v []AutoScout24Listing)`

SetResults sets Results field to given value.


### GetFilters

`func (o *AutoScout24SearchResponse) GetFilters() map[string]interface{}`

GetFilters returns the Filters field if non-nil, zero value otherwise.

### GetFiltersOk

`func (o *AutoScout24SearchResponse) GetFiltersOk() (*map[string]interface{}, bool)`

GetFiltersOk returns a tuple with the Filters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilters

`func (o *AutoScout24SearchResponse) SetFilters(v map[string]interface{})`

SetFilters sets Filters field to given value.


### GetAppliedFilters

`func (o *AutoScout24SearchResponse) GetAppliedFilters() map[string]interface{}`

GetAppliedFilters returns the AppliedFilters field if non-nil, zero value otherwise.

### GetAppliedFiltersOk

`func (o *AutoScout24SearchResponse) GetAppliedFiltersOk() (*map[string]interface{}, bool)`

GetAppliedFiltersOk returns a tuple with the AppliedFilters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAppliedFilters

`func (o *AutoScout24SearchResponse) SetAppliedFilters(v map[string]interface{})`

SetAppliedFilters sets AppliedFilters field to given value.


### GetLatencyMs

`func (o *AutoScout24SearchResponse) GetLatencyMs() int32`

GetLatencyMs returns the LatencyMs field if non-nil, zero value otherwise.

### GetLatencyMsOk

`func (o *AutoScout24SearchResponse) GetLatencyMsOk() (*int32, bool)`

GetLatencyMsOk returns a tuple with the LatencyMs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatencyMs

`func (o *AutoScout24SearchResponse) SetLatencyMs(v int32)`

SetLatencyMs sets LatencyMs field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



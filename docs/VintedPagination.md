# VintedPagination

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CurrentPage** | **int32** |  | 
**TotalPages** | **int32** |  | 
**TotalEntries** | **int32** |  | 
**PerPage** | **int32** |  | 
**Time** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewVintedPagination

`func NewVintedPagination(currentPage int32, totalPages int32, totalEntries int32, perPage int32, ) *VintedPagination`

NewVintedPagination instantiates a new VintedPagination object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVintedPaginationWithDefaults

`func NewVintedPaginationWithDefaults() *VintedPagination`

NewVintedPaginationWithDefaults instantiates a new VintedPagination object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCurrentPage

`func (o *VintedPagination) GetCurrentPage() int32`

GetCurrentPage returns the CurrentPage field if non-nil, zero value otherwise.

### GetCurrentPageOk

`func (o *VintedPagination) GetCurrentPageOk() (*int32, bool)`

GetCurrentPageOk returns a tuple with the CurrentPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrentPage

`func (o *VintedPagination) SetCurrentPage(v int32)`

SetCurrentPage sets CurrentPage field to given value.


### GetTotalPages

`func (o *VintedPagination) GetTotalPages() int32`

GetTotalPages returns the TotalPages field if non-nil, zero value otherwise.

### GetTotalPagesOk

`func (o *VintedPagination) GetTotalPagesOk() (*int32, bool)`

GetTotalPagesOk returns a tuple with the TotalPages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalPages

`func (o *VintedPagination) SetTotalPages(v int32)`

SetTotalPages sets TotalPages field to given value.


### GetTotalEntries

`func (o *VintedPagination) GetTotalEntries() int32`

GetTotalEntries returns the TotalEntries field if non-nil, zero value otherwise.

### GetTotalEntriesOk

`func (o *VintedPagination) GetTotalEntriesOk() (*int32, bool)`

GetTotalEntriesOk returns a tuple with the TotalEntries field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalEntries

`func (o *VintedPagination) SetTotalEntries(v int32)`

SetTotalEntries sets TotalEntries field to given value.


### GetPerPage

`func (o *VintedPagination) GetPerPage() int32`

GetPerPage returns the PerPage field if non-nil, zero value otherwise.

### GetPerPageOk

`func (o *VintedPagination) GetPerPageOk() (*int32, bool)`

GetPerPageOk returns a tuple with the PerPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPerPage

`func (o *VintedPagination) SetPerPage(v int32)`

SetPerPage sets PerPage field to given value.


### GetTime

`func (o *VintedPagination) GetTime() int32`

GetTime returns the Time field if non-nil, zero value otherwise.

### GetTimeOk

`func (o *VintedPagination) GetTimeOk() (*int32, bool)`

GetTimeOk returns a tuple with the Time field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTime

`func (o *VintedPagination) SetTime(v int32)`

SetTime sets Time field to given value.

### HasTime

`func (o *VintedPagination) HasTime() bool`

HasTime returns a boolean if a field has been set.

### SetTimeNil

`func (o *VintedPagination) SetTimeNil(b bool)`

 SetTimeNil sets the value for Time to be an explicit nil

### UnsetTime
`func (o *VintedPagination) UnsetTime()`

UnsetTime ensures that no value is present for Time, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



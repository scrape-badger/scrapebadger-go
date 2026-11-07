# GitHubPagination

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**HasNext** | **bool** |  | 
**Page** | Pointer to **NullableInt32** |  | [optional] 
**NextPage** | Pointer to **NullableInt32** |  | [optional] 
**NextPageToken** | Pointer to **NullableString** |  | [optional] 
**Total** | Pointer to **NullableInt32** |  | [optional] 
**PageCount** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewGitHubPagination

`func NewGitHubPagination(hasNext bool, ) *GitHubPagination`

NewGitHubPagination instantiates a new GitHubPagination object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubPaginationWithDefaults

`func NewGitHubPaginationWithDefaults() *GitHubPagination`

NewGitHubPaginationWithDefaults instantiates a new GitHubPagination object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetHasNext

`func (o *GitHubPagination) GetHasNext() bool`

GetHasNext returns the HasNext field if non-nil, zero value otherwise.

### GetHasNextOk

`func (o *GitHubPagination) GetHasNextOk() (*bool, bool)`

GetHasNextOk returns a tuple with the HasNext field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasNext

`func (o *GitHubPagination) SetHasNext(v bool)`

SetHasNext sets HasNext field to given value.


### GetPage

`func (o *GitHubPagination) GetPage() int32`

GetPage returns the Page field if non-nil, zero value otherwise.

### GetPageOk

`func (o *GitHubPagination) GetPageOk() (*int32, bool)`

GetPageOk returns a tuple with the Page field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPage

`func (o *GitHubPagination) SetPage(v int32)`

SetPage sets Page field to given value.

### HasPage

`func (o *GitHubPagination) HasPage() bool`

HasPage returns a boolean if a field has been set.

### SetPageNil

`func (o *GitHubPagination) SetPageNil(b bool)`

 SetPageNil sets the value for Page to be an explicit nil

### UnsetPage
`func (o *GitHubPagination) UnsetPage()`

UnsetPage ensures that no value is present for Page, not even an explicit nil
### GetNextPage

`func (o *GitHubPagination) GetNextPage() int32`

GetNextPage returns the NextPage field if non-nil, zero value otherwise.

### GetNextPageOk

`func (o *GitHubPagination) GetNextPageOk() (*int32, bool)`

GetNextPageOk returns a tuple with the NextPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPage

`func (o *GitHubPagination) SetNextPage(v int32)`

SetNextPage sets NextPage field to given value.

### HasNextPage

`func (o *GitHubPagination) HasNextPage() bool`

HasNextPage returns a boolean if a field has been set.

### SetNextPageNil

`func (o *GitHubPagination) SetNextPageNil(b bool)`

 SetNextPageNil sets the value for NextPage to be an explicit nil

### UnsetNextPage
`func (o *GitHubPagination) UnsetNextPage()`

UnsetNextPage ensures that no value is present for NextPage, not even an explicit nil
### GetNextPageToken

`func (o *GitHubPagination) GetNextPageToken() string`

GetNextPageToken returns the NextPageToken field if non-nil, zero value otherwise.

### GetNextPageTokenOk

`func (o *GitHubPagination) GetNextPageTokenOk() (*string, bool)`

GetNextPageTokenOk returns a tuple with the NextPageToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPageToken

`func (o *GitHubPagination) SetNextPageToken(v string)`

SetNextPageToken sets NextPageToken field to given value.

### HasNextPageToken

`func (o *GitHubPagination) HasNextPageToken() bool`

HasNextPageToken returns a boolean if a field has been set.

### SetNextPageTokenNil

`func (o *GitHubPagination) SetNextPageTokenNil(b bool)`

 SetNextPageTokenNil sets the value for NextPageToken to be an explicit nil

### UnsetNextPageToken
`func (o *GitHubPagination) UnsetNextPageToken()`

UnsetNextPageToken ensures that no value is present for NextPageToken, not even an explicit nil
### GetTotal

`func (o *GitHubPagination) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *GitHubPagination) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *GitHubPagination) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *GitHubPagination) HasTotal() bool`

HasTotal returns a boolean if a field has been set.

### SetTotalNil

`func (o *GitHubPagination) SetTotalNil(b bool)`

 SetTotalNil sets the value for Total to be an explicit nil

### UnsetTotal
`func (o *GitHubPagination) UnsetTotal()`

UnsetTotal ensures that no value is present for Total, not even an explicit nil
### GetPageCount

`func (o *GitHubPagination) GetPageCount() int32`

GetPageCount returns the PageCount field if non-nil, zero value otherwise.

### GetPageCountOk

`func (o *GitHubPagination) GetPageCountOk() (*int32, bool)`

GetPageCountOk returns a tuple with the PageCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageCount

`func (o *GitHubPagination) SetPageCount(v int32)`

SetPageCount sets PageCount field to given value.

### HasPageCount

`func (o *GitHubPagination) HasPageCount() bool`

HasPageCount returns a boolean if a field has been set.

### SetPageCountNil

`func (o *GitHubPagination) SetPageCountNil(b bool)`

 SetPageCountNil sets the value for PageCount to be an explicit nil

### UnsetPageCount
`func (o *GitHubPagination) UnsetPageCount()`

UnsetPageCount ensures that no value is present for PageCount, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



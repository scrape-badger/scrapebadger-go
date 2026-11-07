# GitHubActivityBlock

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** |  | 
**Summary** | **string** |  | 
**Count** | Pointer to **NullableInt32** |  | [optional] 
**Rows** | [**[]GitHubActivityRow**](GitHubActivityRow.md) |  | 

## Methods

### NewGitHubActivityBlock

`func NewGitHubActivityBlock(type_ string, summary string, rows []GitHubActivityRow, ) *GitHubActivityBlock`

NewGitHubActivityBlock instantiates a new GitHubActivityBlock object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubActivityBlockWithDefaults

`func NewGitHubActivityBlockWithDefaults() *GitHubActivityBlock`

NewGitHubActivityBlockWithDefaults instantiates a new GitHubActivityBlock object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *GitHubActivityBlock) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *GitHubActivityBlock) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *GitHubActivityBlock) SetType(v string)`

SetType sets Type field to given value.


### GetSummary

`func (o *GitHubActivityBlock) GetSummary() string`

GetSummary returns the Summary field if non-nil, zero value otherwise.

### GetSummaryOk

`func (o *GitHubActivityBlock) GetSummaryOk() (*string, bool)`

GetSummaryOk returns a tuple with the Summary field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSummary

`func (o *GitHubActivityBlock) SetSummary(v string)`

SetSummary sets Summary field to given value.


### GetCount

`func (o *GitHubActivityBlock) GetCount() int32`

GetCount returns the Count field if non-nil, zero value otherwise.

### GetCountOk

`func (o *GitHubActivityBlock) GetCountOk() (*int32, bool)`

GetCountOk returns a tuple with the Count field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCount

`func (o *GitHubActivityBlock) SetCount(v int32)`

SetCount sets Count field to given value.

### HasCount

`func (o *GitHubActivityBlock) HasCount() bool`

HasCount returns a boolean if a field has been set.

### SetCountNil

`func (o *GitHubActivityBlock) SetCountNil(b bool)`

 SetCountNil sets the value for Count to be an explicit nil

### UnsetCount
`func (o *GitHubActivityBlock) UnsetCount()`

UnsetCount ensures that no value is present for Count, not even an explicit nil
### GetRows

`func (o *GitHubActivityBlock) GetRows() []GitHubActivityRow`

GetRows returns the Rows field if non-nil, zero value otherwise.

### GetRowsOk

`func (o *GitHubActivityBlock) GetRowsOk() (*[]GitHubActivityRow, bool)`

GetRowsOk returns a tuple with the Rows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRows

`func (o *GitHubActivityBlock) SetRows(v []GitHubActivityRow)`

SetRows sets Rows field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



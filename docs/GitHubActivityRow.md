# GitHubActivityRow

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Text** | **string** |  | 
**Count** | Pointer to **NullableInt32** |  | [optional] 
**Title** | Pointer to **NullableString** |  | [optional] 
**Link** | Pointer to **NullableString** |  | [optional] 
**Repository** | Pointer to **NullableString** |  | [optional] 
**RepositoryLink** | Pointer to **NullableString** |  | [optional] 
**Links** | Pointer to [**[]GitHubTextLink**](GitHubTextLink.md) |  | [optional] 
**CreatedAt** | Pointer to **NullableString** |  | [optional] 
**CreatedUtc** | Pointer to **NullableFloat32** |  | [optional] 

## Methods

### NewGitHubActivityRow

`func NewGitHubActivityRow(text string, ) *GitHubActivityRow`

NewGitHubActivityRow instantiates a new GitHubActivityRow object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubActivityRowWithDefaults

`func NewGitHubActivityRowWithDefaults() *GitHubActivityRow`

NewGitHubActivityRowWithDefaults instantiates a new GitHubActivityRow object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetText

`func (o *GitHubActivityRow) GetText() string`

GetText returns the Text field if non-nil, zero value otherwise.

### GetTextOk

`func (o *GitHubActivityRow) GetTextOk() (*string, bool)`

GetTextOk returns a tuple with the Text field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetText

`func (o *GitHubActivityRow) SetText(v string)`

SetText sets Text field to given value.


### GetCount

`func (o *GitHubActivityRow) GetCount() int32`

GetCount returns the Count field if non-nil, zero value otherwise.

### GetCountOk

`func (o *GitHubActivityRow) GetCountOk() (*int32, bool)`

GetCountOk returns a tuple with the Count field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCount

`func (o *GitHubActivityRow) SetCount(v int32)`

SetCount sets Count field to given value.

### HasCount

`func (o *GitHubActivityRow) HasCount() bool`

HasCount returns a boolean if a field has been set.

### SetCountNil

`func (o *GitHubActivityRow) SetCountNil(b bool)`

 SetCountNil sets the value for Count to be an explicit nil

### UnsetCount
`func (o *GitHubActivityRow) UnsetCount()`

UnsetCount ensures that no value is present for Count, not even an explicit nil
### GetTitle

`func (o *GitHubActivityRow) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *GitHubActivityRow) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *GitHubActivityRow) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *GitHubActivityRow) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### SetTitleNil

`func (o *GitHubActivityRow) SetTitleNil(b bool)`

 SetTitleNil sets the value for Title to be an explicit nil

### UnsetTitle
`func (o *GitHubActivityRow) UnsetTitle()`

UnsetTitle ensures that no value is present for Title, not even an explicit nil
### GetLink

`func (o *GitHubActivityRow) GetLink() string`

GetLink returns the Link field if non-nil, zero value otherwise.

### GetLinkOk

`func (o *GitHubActivityRow) GetLinkOk() (*string, bool)`

GetLinkOk returns a tuple with the Link field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLink

`func (o *GitHubActivityRow) SetLink(v string)`

SetLink sets Link field to given value.

### HasLink

`func (o *GitHubActivityRow) HasLink() bool`

HasLink returns a boolean if a field has been set.

### SetLinkNil

`func (o *GitHubActivityRow) SetLinkNil(b bool)`

 SetLinkNil sets the value for Link to be an explicit nil

### UnsetLink
`func (o *GitHubActivityRow) UnsetLink()`

UnsetLink ensures that no value is present for Link, not even an explicit nil
### GetRepository

`func (o *GitHubActivityRow) GetRepository() string`

GetRepository returns the Repository field if non-nil, zero value otherwise.

### GetRepositoryOk

`func (o *GitHubActivityRow) GetRepositoryOk() (*string, bool)`

GetRepositoryOk returns a tuple with the Repository field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRepository

`func (o *GitHubActivityRow) SetRepository(v string)`

SetRepository sets Repository field to given value.

### HasRepository

`func (o *GitHubActivityRow) HasRepository() bool`

HasRepository returns a boolean if a field has been set.

### SetRepositoryNil

`func (o *GitHubActivityRow) SetRepositoryNil(b bool)`

 SetRepositoryNil sets the value for Repository to be an explicit nil

### UnsetRepository
`func (o *GitHubActivityRow) UnsetRepository()`

UnsetRepository ensures that no value is present for Repository, not even an explicit nil
### GetRepositoryLink

`func (o *GitHubActivityRow) GetRepositoryLink() string`

GetRepositoryLink returns the RepositoryLink field if non-nil, zero value otherwise.

### GetRepositoryLinkOk

`func (o *GitHubActivityRow) GetRepositoryLinkOk() (*string, bool)`

GetRepositoryLinkOk returns a tuple with the RepositoryLink field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRepositoryLink

`func (o *GitHubActivityRow) SetRepositoryLink(v string)`

SetRepositoryLink sets RepositoryLink field to given value.

### HasRepositoryLink

`func (o *GitHubActivityRow) HasRepositoryLink() bool`

HasRepositoryLink returns a boolean if a field has been set.

### SetRepositoryLinkNil

`func (o *GitHubActivityRow) SetRepositoryLinkNil(b bool)`

 SetRepositoryLinkNil sets the value for RepositoryLink to be an explicit nil

### UnsetRepositoryLink
`func (o *GitHubActivityRow) UnsetRepositoryLink()`

UnsetRepositoryLink ensures that no value is present for RepositoryLink, not even an explicit nil
### GetLinks

`func (o *GitHubActivityRow) GetLinks() []GitHubTextLink`

GetLinks returns the Links field if non-nil, zero value otherwise.

### GetLinksOk

`func (o *GitHubActivityRow) GetLinksOk() (*[]GitHubTextLink, bool)`

GetLinksOk returns a tuple with the Links field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLinks

`func (o *GitHubActivityRow) SetLinks(v []GitHubTextLink)`

SetLinks sets Links field to given value.

### HasLinks

`func (o *GitHubActivityRow) HasLinks() bool`

HasLinks returns a boolean if a field has been set.

### SetLinksNil

`func (o *GitHubActivityRow) SetLinksNil(b bool)`

 SetLinksNil sets the value for Links to be an explicit nil

### UnsetLinks
`func (o *GitHubActivityRow) UnsetLinks()`

UnsetLinks ensures that no value is present for Links, not even an explicit nil
### GetCreatedAt

`func (o *GitHubActivityRow) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *GitHubActivityRow) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *GitHubActivityRow) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *GitHubActivityRow) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### SetCreatedAtNil

`func (o *GitHubActivityRow) SetCreatedAtNil(b bool)`

 SetCreatedAtNil sets the value for CreatedAt to be an explicit nil

### UnsetCreatedAt
`func (o *GitHubActivityRow) UnsetCreatedAt()`

UnsetCreatedAt ensures that no value is present for CreatedAt, not even an explicit nil
### GetCreatedUtc

`func (o *GitHubActivityRow) GetCreatedUtc() float32`

GetCreatedUtc returns the CreatedUtc field if non-nil, zero value otherwise.

### GetCreatedUtcOk

`func (o *GitHubActivityRow) GetCreatedUtcOk() (*float32, bool)`

GetCreatedUtcOk returns a tuple with the CreatedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedUtc

`func (o *GitHubActivityRow) SetCreatedUtc(v float32)`

SetCreatedUtc sets CreatedUtc field to given value.

### HasCreatedUtc

`func (o *GitHubActivityRow) HasCreatedUtc() bool`

HasCreatedUtc returns a boolean if a field has been set.

### SetCreatedUtcNil

`func (o *GitHubActivityRow) SetCreatedUtcNil(b bool)`

 SetCreatedUtcNil sets the value for CreatedUtc to be an explicit nil

### UnsetCreatedUtc
`func (o *GitHubActivityRow) UnsetCreatedUtc()`

UnsetCreatedUtc ensures that no value is present for CreatedUtc, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



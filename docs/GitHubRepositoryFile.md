# GitHubRepositoryFile

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**Path** | **string** |  | 
**Type** | **string** |  | 
**Link** | **string** |  | 
**HasSimplifiedPath** | Pointer to **NullableBool** |  | [optional] 
**LatestCommit** | Pointer to [**NullableGitHubLatestCommit**](GitHubLatestCommit.md) |  | [optional] 

## Methods

### NewGitHubRepositoryFile

`func NewGitHubRepositoryFile(name string, path string, type_ string, link string, ) *GitHubRepositoryFile`

NewGitHubRepositoryFile instantiates a new GitHubRepositoryFile object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubRepositoryFileWithDefaults

`func NewGitHubRepositoryFileWithDefaults() *GitHubRepositoryFile`

NewGitHubRepositoryFileWithDefaults instantiates a new GitHubRepositoryFile object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *GitHubRepositoryFile) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *GitHubRepositoryFile) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *GitHubRepositoryFile) SetName(v string)`

SetName sets Name field to given value.


### GetPath

`func (o *GitHubRepositoryFile) GetPath() string`

GetPath returns the Path field if non-nil, zero value otherwise.

### GetPathOk

`func (o *GitHubRepositoryFile) GetPathOk() (*string, bool)`

GetPathOk returns a tuple with the Path field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPath

`func (o *GitHubRepositoryFile) SetPath(v string)`

SetPath sets Path field to given value.


### GetType

`func (o *GitHubRepositoryFile) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *GitHubRepositoryFile) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *GitHubRepositoryFile) SetType(v string)`

SetType sets Type field to given value.


### GetLink

`func (o *GitHubRepositoryFile) GetLink() string`

GetLink returns the Link field if non-nil, zero value otherwise.

### GetLinkOk

`func (o *GitHubRepositoryFile) GetLinkOk() (*string, bool)`

GetLinkOk returns a tuple with the Link field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLink

`func (o *GitHubRepositoryFile) SetLink(v string)`

SetLink sets Link field to given value.


### GetHasSimplifiedPath

`func (o *GitHubRepositoryFile) GetHasSimplifiedPath() bool`

GetHasSimplifiedPath returns the HasSimplifiedPath field if non-nil, zero value otherwise.

### GetHasSimplifiedPathOk

`func (o *GitHubRepositoryFile) GetHasSimplifiedPathOk() (*bool, bool)`

GetHasSimplifiedPathOk returns a tuple with the HasSimplifiedPath field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasSimplifiedPath

`func (o *GitHubRepositoryFile) SetHasSimplifiedPath(v bool)`

SetHasSimplifiedPath sets HasSimplifiedPath field to given value.

### HasHasSimplifiedPath

`func (o *GitHubRepositoryFile) HasHasSimplifiedPath() bool`

HasHasSimplifiedPath returns a boolean if a field has been set.

### SetHasSimplifiedPathNil

`func (o *GitHubRepositoryFile) SetHasSimplifiedPathNil(b bool)`

 SetHasSimplifiedPathNil sets the value for HasSimplifiedPath to be an explicit nil

### UnsetHasSimplifiedPath
`func (o *GitHubRepositoryFile) UnsetHasSimplifiedPath()`

UnsetHasSimplifiedPath ensures that no value is present for HasSimplifiedPath, not even an explicit nil
### GetLatestCommit

`func (o *GitHubRepositoryFile) GetLatestCommit() GitHubLatestCommit`

GetLatestCommit returns the LatestCommit field if non-nil, zero value otherwise.

### GetLatestCommitOk

`func (o *GitHubRepositoryFile) GetLatestCommitOk() (*GitHubLatestCommit, bool)`

GetLatestCommitOk returns a tuple with the LatestCommit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatestCommit

`func (o *GitHubRepositoryFile) SetLatestCommit(v GitHubLatestCommit)`

SetLatestCommit sets LatestCommit field to given value.

### HasLatestCommit

`func (o *GitHubRepositoryFile) HasLatestCommit() bool`

HasLatestCommit returns a boolean if a field has been set.

### SetLatestCommitNil

`func (o *GitHubRepositoryFile) SetLatestCommitNil(b bool)`

 SetLatestCommitNil sets the value for LatestCommit to be an explicit nil

### UnsetLatestCommit
`func (o *GitHubRepositoryFile) UnsetLatestCommit()`

UnsetLatestCommit ensures that no value is present for LatestCommit, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



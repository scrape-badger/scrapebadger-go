# GitHubRepositoryResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Repository** | [**GitHubRepositoryIdentity**](GitHubRepositoryIdentity.md) |  | 
**LatestCommit** | Pointer to [**NullableGitHubLatestCommit**](GitHubLatestCommit.md) |  | [optional] 
**Readme** | Pointer to [**NullableGitHubRepositoryReadme**](GitHubRepositoryReadme.md) |  | [optional] 
**Files** | Pointer to [**[]GitHubRepositoryFile**](GitHubRepositoryFile.md) |  | [optional] 
**Languages** | Pointer to [**[]GitHubRepositoryLanguage**](GitHubRepositoryLanguage.md) |  | [optional] 
**LatestRelease** | Pointer to [**NullableGitHubRepositoryRelease**](GitHubRepositoryRelease.md) |  | [optional] 
**Contributors** | Pointer to [**[]GitHubRepositoryAccount**](GitHubRepositoryAccount.md) |  | [optional] 
**ContributorsTruncated** | Pointer to **NullableBool** |  | [optional] 
**Dependents** | Pointer to [**[]GitHubRepositoryAccount**](GitHubRepositoryAccount.md) |  | [optional] 
**DependentsTruncated** | Pointer to **NullableBool** |  | [optional] 
**Funding** | Pointer to [**NullableGitHubRepositoryFunding**](GitHubRepositoryFunding.md) |  | [optional] 
**CommunityFiles** | Pointer to [**[]GitHubCommunityFile**](GitHubCommunityFile.md) |  | [optional] 
**MetadataAvailable** | Pointer to **NullableBool** |  | [optional] 

## Methods

### NewGitHubRepositoryResponse

`func NewGitHubRepositoryResponse(repository GitHubRepositoryIdentity, ) *GitHubRepositoryResponse`

NewGitHubRepositoryResponse instantiates a new GitHubRepositoryResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubRepositoryResponseWithDefaults

`func NewGitHubRepositoryResponseWithDefaults() *GitHubRepositoryResponse`

NewGitHubRepositoryResponseWithDefaults instantiates a new GitHubRepositoryResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRepository

`func (o *GitHubRepositoryResponse) GetRepository() GitHubRepositoryIdentity`

GetRepository returns the Repository field if non-nil, zero value otherwise.

### GetRepositoryOk

`func (o *GitHubRepositoryResponse) GetRepositoryOk() (*GitHubRepositoryIdentity, bool)`

GetRepositoryOk returns a tuple with the Repository field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRepository

`func (o *GitHubRepositoryResponse) SetRepository(v GitHubRepositoryIdentity)`

SetRepository sets Repository field to given value.


### GetLatestCommit

`func (o *GitHubRepositoryResponse) GetLatestCommit() GitHubLatestCommit`

GetLatestCommit returns the LatestCommit field if non-nil, zero value otherwise.

### GetLatestCommitOk

`func (o *GitHubRepositoryResponse) GetLatestCommitOk() (*GitHubLatestCommit, bool)`

GetLatestCommitOk returns a tuple with the LatestCommit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatestCommit

`func (o *GitHubRepositoryResponse) SetLatestCommit(v GitHubLatestCommit)`

SetLatestCommit sets LatestCommit field to given value.

### HasLatestCommit

`func (o *GitHubRepositoryResponse) HasLatestCommit() bool`

HasLatestCommit returns a boolean if a field has been set.

### SetLatestCommitNil

`func (o *GitHubRepositoryResponse) SetLatestCommitNil(b bool)`

 SetLatestCommitNil sets the value for LatestCommit to be an explicit nil

### UnsetLatestCommit
`func (o *GitHubRepositoryResponse) UnsetLatestCommit()`

UnsetLatestCommit ensures that no value is present for LatestCommit, not even an explicit nil
### GetReadme

`func (o *GitHubRepositoryResponse) GetReadme() GitHubRepositoryReadme`

GetReadme returns the Readme field if non-nil, zero value otherwise.

### GetReadmeOk

`func (o *GitHubRepositoryResponse) GetReadmeOk() (*GitHubRepositoryReadme, bool)`

GetReadmeOk returns a tuple with the Readme field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReadme

`func (o *GitHubRepositoryResponse) SetReadme(v GitHubRepositoryReadme)`

SetReadme sets Readme field to given value.

### HasReadme

`func (o *GitHubRepositoryResponse) HasReadme() bool`

HasReadme returns a boolean if a field has been set.

### SetReadmeNil

`func (o *GitHubRepositoryResponse) SetReadmeNil(b bool)`

 SetReadmeNil sets the value for Readme to be an explicit nil

### UnsetReadme
`func (o *GitHubRepositoryResponse) UnsetReadme()`

UnsetReadme ensures that no value is present for Readme, not even an explicit nil
### GetFiles

`func (o *GitHubRepositoryResponse) GetFiles() []GitHubRepositoryFile`

GetFiles returns the Files field if non-nil, zero value otherwise.

### GetFilesOk

`func (o *GitHubRepositoryResponse) GetFilesOk() (*[]GitHubRepositoryFile, bool)`

GetFilesOk returns a tuple with the Files field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFiles

`func (o *GitHubRepositoryResponse) SetFiles(v []GitHubRepositoryFile)`

SetFiles sets Files field to given value.

### HasFiles

`func (o *GitHubRepositoryResponse) HasFiles() bool`

HasFiles returns a boolean if a field has been set.

### SetFilesNil

`func (o *GitHubRepositoryResponse) SetFilesNil(b bool)`

 SetFilesNil sets the value for Files to be an explicit nil

### UnsetFiles
`func (o *GitHubRepositoryResponse) UnsetFiles()`

UnsetFiles ensures that no value is present for Files, not even an explicit nil
### GetLanguages

`func (o *GitHubRepositoryResponse) GetLanguages() []GitHubRepositoryLanguage`

GetLanguages returns the Languages field if non-nil, zero value otherwise.

### GetLanguagesOk

`func (o *GitHubRepositoryResponse) GetLanguagesOk() (*[]GitHubRepositoryLanguage, bool)`

GetLanguagesOk returns a tuple with the Languages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLanguages

`func (o *GitHubRepositoryResponse) SetLanguages(v []GitHubRepositoryLanguage)`

SetLanguages sets Languages field to given value.

### HasLanguages

`func (o *GitHubRepositoryResponse) HasLanguages() bool`

HasLanguages returns a boolean if a field has been set.

### SetLanguagesNil

`func (o *GitHubRepositoryResponse) SetLanguagesNil(b bool)`

 SetLanguagesNil sets the value for Languages to be an explicit nil

### UnsetLanguages
`func (o *GitHubRepositoryResponse) UnsetLanguages()`

UnsetLanguages ensures that no value is present for Languages, not even an explicit nil
### GetLatestRelease

`func (o *GitHubRepositoryResponse) GetLatestRelease() GitHubRepositoryRelease`

GetLatestRelease returns the LatestRelease field if non-nil, zero value otherwise.

### GetLatestReleaseOk

`func (o *GitHubRepositoryResponse) GetLatestReleaseOk() (*GitHubRepositoryRelease, bool)`

GetLatestReleaseOk returns a tuple with the LatestRelease field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatestRelease

`func (o *GitHubRepositoryResponse) SetLatestRelease(v GitHubRepositoryRelease)`

SetLatestRelease sets LatestRelease field to given value.

### HasLatestRelease

`func (o *GitHubRepositoryResponse) HasLatestRelease() bool`

HasLatestRelease returns a boolean if a field has been set.

### SetLatestReleaseNil

`func (o *GitHubRepositoryResponse) SetLatestReleaseNil(b bool)`

 SetLatestReleaseNil sets the value for LatestRelease to be an explicit nil

### UnsetLatestRelease
`func (o *GitHubRepositoryResponse) UnsetLatestRelease()`

UnsetLatestRelease ensures that no value is present for LatestRelease, not even an explicit nil
### GetContributors

`func (o *GitHubRepositoryResponse) GetContributors() []GitHubRepositoryAccount`

GetContributors returns the Contributors field if non-nil, zero value otherwise.

### GetContributorsOk

`func (o *GitHubRepositoryResponse) GetContributorsOk() (*[]GitHubRepositoryAccount, bool)`

GetContributorsOk returns a tuple with the Contributors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContributors

`func (o *GitHubRepositoryResponse) SetContributors(v []GitHubRepositoryAccount)`

SetContributors sets Contributors field to given value.

### HasContributors

`func (o *GitHubRepositoryResponse) HasContributors() bool`

HasContributors returns a boolean if a field has been set.

### SetContributorsNil

`func (o *GitHubRepositoryResponse) SetContributorsNil(b bool)`

 SetContributorsNil sets the value for Contributors to be an explicit nil

### UnsetContributors
`func (o *GitHubRepositoryResponse) UnsetContributors()`

UnsetContributors ensures that no value is present for Contributors, not even an explicit nil
### GetContributorsTruncated

`func (o *GitHubRepositoryResponse) GetContributorsTruncated() bool`

GetContributorsTruncated returns the ContributorsTruncated field if non-nil, zero value otherwise.

### GetContributorsTruncatedOk

`func (o *GitHubRepositoryResponse) GetContributorsTruncatedOk() (*bool, bool)`

GetContributorsTruncatedOk returns a tuple with the ContributorsTruncated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContributorsTruncated

`func (o *GitHubRepositoryResponse) SetContributorsTruncated(v bool)`

SetContributorsTruncated sets ContributorsTruncated field to given value.

### HasContributorsTruncated

`func (o *GitHubRepositoryResponse) HasContributorsTruncated() bool`

HasContributorsTruncated returns a boolean if a field has been set.

### SetContributorsTruncatedNil

`func (o *GitHubRepositoryResponse) SetContributorsTruncatedNil(b bool)`

 SetContributorsTruncatedNil sets the value for ContributorsTruncated to be an explicit nil

### UnsetContributorsTruncated
`func (o *GitHubRepositoryResponse) UnsetContributorsTruncated()`

UnsetContributorsTruncated ensures that no value is present for ContributorsTruncated, not even an explicit nil
### GetDependents

`func (o *GitHubRepositoryResponse) GetDependents() []GitHubRepositoryAccount`

GetDependents returns the Dependents field if non-nil, zero value otherwise.

### GetDependentsOk

`func (o *GitHubRepositoryResponse) GetDependentsOk() (*[]GitHubRepositoryAccount, bool)`

GetDependentsOk returns a tuple with the Dependents field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDependents

`func (o *GitHubRepositoryResponse) SetDependents(v []GitHubRepositoryAccount)`

SetDependents sets Dependents field to given value.

### HasDependents

`func (o *GitHubRepositoryResponse) HasDependents() bool`

HasDependents returns a boolean if a field has been set.

### SetDependentsNil

`func (o *GitHubRepositoryResponse) SetDependentsNil(b bool)`

 SetDependentsNil sets the value for Dependents to be an explicit nil

### UnsetDependents
`func (o *GitHubRepositoryResponse) UnsetDependents()`

UnsetDependents ensures that no value is present for Dependents, not even an explicit nil
### GetDependentsTruncated

`func (o *GitHubRepositoryResponse) GetDependentsTruncated() bool`

GetDependentsTruncated returns the DependentsTruncated field if non-nil, zero value otherwise.

### GetDependentsTruncatedOk

`func (o *GitHubRepositoryResponse) GetDependentsTruncatedOk() (*bool, bool)`

GetDependentsTruncatedOk returns a tuple with the DependentsTruncated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDependentsTruncated

`func (o *GitHubRepositoryResponse) SetDependentsTruncated(v bool)`

SetDependentsTruncated sets DependentsTruncated field to given value.

### HasDependentsTruncated

`func (o *GitHubRepositoryResponse) HasDependentsTruncated() bool`

HasDependentsTruncated returns a boolean if a field has been set.

### SetDependentsTruncatedNil

`func (o *GitHubRepositoryResponse) SetDependentsTruncatedNil(b bool)`

 SetDependentsTruncatedNil sets the value for DependentsTruncated to be an explicit nil

### UnsetDependentsTruncated
`func (o *GitHubRepositoryResponse) UnsetDependentsTruncated()`

UnsetDependentsTruncated ensures that no value is present for DependentsTruncated, not even an explicit nil
### GetFunding

`func (o *GitHubRepositoryResponse) GetFunding() GitHubRepositoryFunding`

GetFunding returns the Funding field if non-nil, zero value otherwise.

### GetFundingOk

`func (o *GitHubRepositoryResponse) GetFundingOk() (*GitHubRepositoryFunding, bool)`

GetFundingOk returns a tuple with the Funding field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFunding

`func (o *GitHubRepositoryResponse) SetFunding(v GitHubRepositoryFunding)`

SetFunding sets Funding field to given value.

### HasFunding

`func (o *GitHubRepositoryResponse) HasFunding() bool`

HasFunding returns a boolean if a field has been set.

### SetFundingNil

`func (o *GitHubRepositoryResponse) SetFundingNil(b bool)`

 SetFundingNil sets the value for Funding to be an explicit nil

### UnsetFunding
`func (o *GitHubRepositoryResponse) UnsetFunding()`

UnsetFunding ensures that no value is present for Funding, not even an explicit nil
### GetCommunityFiles

`func (o *GitHubRepositoryResponse) GetCommunityFiles() []GitHubCommunityFile`

GetCommunityFiles returns the CommunityFiles field if non-nil, zero value otherwise.

### GetCommunityFilesOk

`func (o *GitHubRepositoryResponse) GetCommunityFilesOk() (*[]GitHubCommunityFile, bool)`

GetCommunityFilesOk returns a tuple with the CommunityFiles field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommunityFiles

`func (o *GitHubRepositoryResponse) SetCommunityFiles(v []GitHubCommunityFile)`

SetCommunityFiles sets CommunityFiles field to given value.

### HasCommunityFiles

`func (o *GitHubRepositoryResponse) HasCommunityFiles() bool`

HasCommunityFiles returns a boolean if a field has been set.

### SetCommunityFilesNil

`func (o *GitHubRepositoryResponse) SetCommunityFilesNil(b bool)`

 SetCommunityFilesNil sets the value for CommunityFiles to be an explicit nil

### UnsetCommunityFiles
`func (o *GitHubRepositoryResponse) UnsetCommunityFiles()`

UnsetCommunityFiles ensures that no value is present for CommunityFiles, not even an explicit nil
### GetMetadataAvailable

`func (o *GitHubRepositoryResponse) GetMetadataAvailable() bool`

GetMetadataAvailable returns the MetadataAvailable field if non-nil, zero value otherwise.

### GetMetadataAvailableOk

`func (o *GitHubRepositoryResponse) GetMetadataAvailableOk() (*bool, bool)`

GetMetadataAvailableOk returns a tuple with the MetadataAvailable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadataAvailable

`func (o *GitHubRepositoryResponse) SetMetadataAvailable(v bool)`

SetMetadataAvailable sets MetadataAvailable field to given value.

### HasMetadataAvailable

`func (o *GitHubRepositoryResponse) HasMetadataAvailable() bool`

HasMetadataAvailable returns a boolean if a field has been set.

### SetMetadataAvailableNil

`func (o *GitHubRepositoryResponse) SetMetadataAvailableNil(b bool)`

 SetMetadataAvailableNil sets the value for MetadataAvailable to be an explicit nil

### UnsetMetadataAvailable
`func (o *GitHubRepositoryResponse) UnsetMetadataAvailable()`

UnsetMetadataAvailable ensures that no value is present for MetadataAvailable, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



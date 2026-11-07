# GitHubActivityOverview

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Summary** | Pointer to **NullableString** |  | [optional] 
**Description** | Pointer to **NullableString** |  | [optional] 
**Repositories** | Pointer to [**[]GitHubNamedLink**](GitHubNamedLink.md) |  | [optional] 
**CommitsPercentage** | Pointer to **NullableInt32** |  | [optional] 
**CodeReviewPercentage** | Pointer to **NullableInt32** |  | [optional] 
**PullRequestsPercentage** | Pointer to **NullableInt32** |  | [optional] 
**IssuesPercentage** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewGitHubActivityOverview

`func NewGitHubActivityOverview() *GitHubActivityOverview`

NewGitHubActivityOverview instantiates a new GitHubActivityOverview object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubActivityOverviewWithDefaults

`func NewGitHubActivityOverviewWithDefaults() *GitHubActivityOverview`

NewGitHubActivityOverviewWithDefaults instantiates a new GitHubActivityOverview object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSummary

`func (o *GitHubActivityOverview) GetSummary() string`

GetSummary returns the Summary field if non-nil, zero value otherwise.

### GetSummaryOk

`func (o *GitHubActivityOverview) GetSummaryOk() (*string, bool)`

GetSummaryOk returns a tuple with the Summary field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSummary

`func (o *GitHubActivityOverview) SetSummary(v string)`

SetSummary sets Summary field to given value.

### HasSummary

`func (o *GitHubActivityOverview) HasSummary() bool`

HasSummary returns a boolean if a field has been set.

### SetSummaryNil

`func (o *GitHubActivityOverview) SetSummaryNil(b bool)`

 SetSummaryNil sets the value for Summary to be an explicit nil

### UnsetSummary
`func (o *GitHubActivityOverview) UnsetSummary()`

UnsetSummary ensures that no value is present for Summary, not even an explicit nil
### GetDescription

`func (o *GitHubActivityOverview) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *GitHubActivityOverview) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *GitHubActivityOverview) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *GitHubActivityOverview) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *GitHubActivityOverview) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *GitHubActivityOverview) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetRepositories

`func (o *GitHubActivityOverview) GetRepositories() []GitHubNamedLink`

GetRepositories returns the Repositories field if non-nil, zero value otherwise.

### GetRepositoriesOk

`func (o *GitHubActivityOverview) GetRepositoriesOk() (*[]GitHubNamedLink, bool)`

GetRepositoriesOk returns a tuple with the Repositories field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRepositories

`func (o *GitHubActivityOverview) SetRepositories(v []GitHubNamedLink)`

SetRepositories sets Repositories field to given value.

### HasRepositories

`func (o *GitHubActivityOverview) HasRepositories() bool`

HasRepositories returns a boolean if a field has been set.

### SetRepositoriesNil

`func (o *GitHubActivityOverview) SetRepositoriesNil(b bool)`

 SetRepositoriesNil sets the value for Repositories to be an explicit nil

### UnsetRepositories
`func (o *GitHubActivityOverview) UnsetRepositories()`

UnsetRepositories ensures that no value is present for Repositories, not even an explicit nil
### GetCommitsPercentage

`func (o *GitHubActivityOverview) GetCommitsPercentage() int32`

GetCommitsPercentage returns the CommitsPercentage field if non-nil, zero value otherwise.

### GetCommitsPercentageOk

`func (o *GitHubActivityOverview) GetCommitsPercentageOk() (*int32, bool)`

GetCommitsPercentageOk returns a tuple with the CommitsPercentage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommitsPercentage

`func (o *GitHubActivityOverview) SetCommitsPercentage(v int32)`

SetCommitsPercentage sets CommitsPercentage field to given value.

### HasCommitsPercentage

`func (o *GitHubActivityOverview) HasCommitsPercentage() bool`

HasCommitsPercentage returns a boolean if a field has been set.

### SetCommitsPercentageNil

`func (o *GitHubActivityOverview) SetCommitsPercentageNil(b bool)`

 SetCommitsPercentageNil sets the value for CommitsPercentage to be an explicit nil

### UnsetCommitsPercentage
`func (o *GitHubActivityOverview) UnsetCommitsPercentage()`

UnsetCommitsPercentage ensures that no value is present for CommitsPercentage, not even an explicit nil
### GetCodeReviewPercentage

`func (o *GitHubActivityOverview) GetCodeReviewPercentage() int32`

GetCodeReviewPercentage returns the CodeReviewPercentage field if non-nil, zero value otherwise.

### GetCodeReviewPercentageOk

`func (o *GitHubActivityOverview) GetCodeReviewPercentageOk() (*int32, bool)`

GetCodeReviewPercentageOk returns a tuple with the CodeReviewPercentage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCodeReviewPercentage

`func (o *GitHubActivityOverview) SetCodeReviewPercentage(v int32)`

SetCodeReviewPercentage sets CodeReviewPercentage field to given value.

### HasCodeReviewPercentage

`func (o *GitHubActivityOverview) HasCodeReviewPercentage() bool`

HasCodeReviewPercentage returns a boolean if a field has been set.

### SetCodeReviewPercentageNil

`func (o *GitHubActivityOverview) SetCodeReviewPercentageNil(b bool)`

 SetCodeReviewPercentageNil sets the value for CodeReviewPercentage to be an explicit nil

### UnsetCodeReviewPercentage
`func (o *GitHubActivityOverview) UnsetCodeReviewPercentage()`

UnsetCodeReviewPercentage ensures that no value is present for CodeReviewPercentage, not even an explicit nil
### GetPullRequestsPercentage

`func (o *GitHubActivityOverview) GetPullRequestsPercentage() int32`

GetPullRequestsPercentage returns the PullRequestsPercentage field if non-nil, zero value otherwise.

### GetPullRequestsPercentageOk

`func (o *GitHubActivityOverview) GetPullRequestsPercentageOk() (*int32, bool)`

GetPullRequestsPercentageOk returns a tuple with the PullRequestsPercentage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPullRequestsPercentage

`func (o *GitHubActivityOverview) SetPullRequestsPercentage(v int32)`

SetPullRequestsPercentage sets PullRequestsPercentage field to given value.

### HasPullRequestsPercentage

`func (o *GitHubActivityOverview) HasPullRequestsPercentage() bool`

HasPullRequestsPercentage returns a boolean if a field has been set.

### SetPullRequestsPercentageNil

`func (o *GitHubActivityOverview) SetPullRequestsPercentageNil(b bool)`

 SetPullRequestsPercentageNil sets the value for PullRequestsPercentage to be an explicit nil

### UnsetPullRequestsPercentage
`func (o *GitHubActivityOverview) UnsetPullRequestsPercentage()`

UnsetPullRequestsPercentage ensures that no value is present for PullRequestsPercentage, not even an explicit nil
### GetIssuesPercentage

`func (o *GitHubActivityOverview) GetIssuesPercentage() int32`

GetIssuesPercentage returns the IssuesPercentage field if non-nil, zero value otherwise.

### GetIssuesPercentageOk

`func (o *GitHubActivityOverview) GetIssuesPercentageOk() (*int32, bool)`

GetIssuesPercentageOk returns a tuple with the IssuesPercentage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssuesPercentage

`func (o *GitHubActivityOverview) SetIssuesPercentage(v int32)`

SetIssuesPercentage sets IssuesPercentage field to given value.

### HasIssuesPercentage

`func (o *GitHubActivityOverview) HasIssuesPercentage() bool`

HasIssuesPercentage returns a boolean if a field has been set.

### SetIssuesPercentageNil

`func (o *GitHubActivityOverview) SetIssuesPercentageNil(b bool)`

 SetIssuesPercentageNil sets the value for IssuesPercentage to be an explicit nil

### UnsetIssuesPercentage
`func (o *GitHubActivityOverview) UnsetIssuesPercentage()`

UnsetIssuesPercentage ensures that no value is present for IssuesPercentage, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



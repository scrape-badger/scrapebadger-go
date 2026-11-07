# GitHubRepositoryIdentity

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**FullName** | **string** |  | 
**Link** | **string** |  | 
**Owner** | [**GitHubRepositoryAccount**](GitHubRepositoryAccount.md) |  | 
**IsEmpty** | **bool** |  | 
**Id** | Pointer to **NullableInt32** |  | [optional] 
**NodeId** | Pointer to **NullableString** |  | [optional] 
**Description** | Pointer to **NullableString** |  | [optional] 
**Website** | Pointer to **NullableString** |  | [optional] 
**SocialImage** | Pointer to **NullableString** |  | [optional] 
**DefaultBranch** | Pointer to **NullableString** |  | [optional] 
**CurrentCommit** | Pointer to **NullableString** |  | [optional] 
**Visibility** | Pointer to **NullableString** |  | [optional] 
**IsFork** | Pointer to **NullableBool** |  | [optional] 
**ForkedFrom** | Pointer to **NullableString** |  | [optional] 
**Parent** | Pointer to [**NullableGitHubRepositoryReference**](GitHubRepositoryReference.md) |  | [optional] 
**Source** | Pointer to [**NullableGitHubRepositoryReference**](GitHubRepositoryReference.md) |  | [optional] 
**ForkComparison** | Pointer to [**NullableGitHubForkComparison**](GitHubForkComparison.md) |  | [optional] 
**IsArchived** | Pointer to **NullableBool** |  | [optional] 
**IsTemplate** | Pointer to **NullableBool** |  | [optional] 
**IsMirror** | Pointer to **NullableBool** |  | [optional] 
**IsDisabled** | Pointer to **NullableBool** |  | [optional] 
**Language** | Pointer to **NullableString** |  | [optional] 
**LanguageColor** | Pointer to **NullableString** |  | [optional] 
**License** | Pointer to [**NullableGitHubRepositoryLicense**](GitHubRepositoryLicense.md) |  | [optional] 
**Topics** | Pointer to **[]string** |  | [optional] 
**Stars** | Pointer to **NullableInt32** |  | [optional] 
**Watchers** | Pointer to **NullableInt32** |  | [optional] 
**Forks** | Pointer to **NullableInt32** |  | [optional] 
**NetworkCount** | Pointer to **NullableInt32** |  | [optional] 
**OpenIssuesCount** | Pointer to **NullableInt32** |  | [optional] 
**OpenPullRequestsCount** | Pointer to **NullableInt32** |  | [optional] 
**OpenIssuesCountApproximate** | Pointer to **NullableBool** |  | [optional] 
**OpenPullRequestsCountApproximate** | Pointer to **NullableBool** |  | [optional] 
**OpenIssuesDisplay** | Pointer to **NullableString** |  | [optional] 
**OpenPullRequestsDisplay** | Pointer to **NullableString** |  | [optional] 
**IsOpenIssuesCountCapped** | Pointer to **NullableBool** |  | [optional] 
**IsOpenPullRequestsCountCapped** | Pointer to **NullableBool** |  | [optional] 
**OpenIssuesAndPullRequestsCount** | Pointer to **NullableInt32** |  | [optional] 
**CommitsCount** | Pointer to **NullableInt32** |  | [optional] 
**CommitsDisplay** | Pointer to **NullableString** |  | [optional] 
**CommitsCountApproximate** | Pointer to **NullableBool** |  | [optional] 
**BranchesCount** | Pointer to **NullableInt32** |  | [optional] 
**BranchesCountApproximate** | Pointer to **NullableBool** |  | [optional] 
**TagsCount** | Pointer to **NullableInt32** |  | [optional] 
**ReleasesCount** | Pointer to **NullableInt32** |  | [optional] 
**ContributorsCount** | Pointer to **NullableInt32** |  | [optional] 
**ContributorsCountApproximate** | Pointer to **NullableBool** |  | [optional] 
**UsedByCount** | Pointer to **NullableInt32** |  | [optional] 
**UsedByCountApproximate** | Pointer to **NullableBool** |  | [optional] 
**SecurityAdvisoriesCount** | Pointer to **NullableInt32** |  | [optional] 
**FilesCount** | Pointer to **NullableInt32** |  | [optional] 
**FilesTruncated** | Pointer to **NullableBool** |  | [optional] 
**HasIssues** | Pointer to **NullableBool** |  | [optional] 
**HasPullRequests** | Pointer to **NullableBool** |  | [optional] 
**HasDiscussions** | Pointer to **NullableBool** |  | [optional] 
**HasProjects** | Pointer to **NullableBool** |  | [optional] 
**HasWiki** | Pointer to **NullableBool** |  | [optional] 
**HasPages** | Pointer to **NullableBool** |  | [optional] 
**HasDownloads** | Pointer to **NullableBool** |  | [optional] 
**HasCitation** | Pointer to **NullableBool** |  | [optional] 
**HasCodeOfConduct** | Pointer to **NullableBool** |  | [optional] 
**HasContributingGuide** | Pointer to **NullableBool** |  | [optional] 
**HasSecurityPolicy** | Pointer to **NullableBool** |  | [optional] 
**AllowForking** | Pointer to **NullableBool** |  | [optional] 
**WebCommitSignoffRequired** | Pointer to **NullableBool** |  | [optional] 
**PullRequestCreationPolicy** | Pointer to **NullableString** |  | [optional] 
**SizeKb** | Pointer to **NullableInt32** |  | [optional] 
**CloneUrl** | Pointer to **NullableString** |  | [optional] 
**SshUrl** | Pointer to **NullableString** |  | [optional] 
**GitUrl** | Pointer to **NullableString** |  | [optional] 
**SvnUrl** | Pointer to **NullableString** |  | [optional] 
**ArchiveUrl** | Pointer to **NullableString** |  | [optional] 
**MirrorUrl** | Pointer to **NullableString** |  | [optional] 
**CreatedAt** | Pointer to **NullableString** |  | [optional] 
**CreatedUtc** | Pointer to **NullableFloat32** |  | [optional] 
**UpdatedAt** | Pointer to **NullableString** |  | [optional] 
**UpdatedUtc** | Pointer to **NullableFloat32** |  | [optional] 
**PushedAt** | Pointer to **NullableString** |  | [optional] 
**PushedUtc** | Pointer to **NullableFloat32** |  | [optional] 

## Methods

### NewGitHubRepositoryIdentity

`func NewGitHubRepositoryIdentity(name string, fullName string, link string, owner GitHubRepositoryAccount, isEmpty bool, ) *GitHubRepositoryIdentity`

NewGitHubRepositoryIdentity instantiates a new GitHubRepositoryIdentity object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubRepositoryIdentityWithDefaults

`func NewGitHubRepositoryIdentityWithDefaults() *GitHubRepositoryIdentity`

NewGitHubRepositoryIdentityWithDefaults instantiates a new GitHubRepositoryIdentity object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *GitHubRepositoryIdentity) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *GitHubRepositoryIdentity) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *GitHubRepositoryIdentity) SetName(v string)`

SetName sets Name field to given value.


### GetFullName

`func (o *GitHubRepositoryIdentity) GetFullName() string`

GetFullName returns the FullName field if non-nil, zero value otherwise.

### GetFullNameOk

`func (o *GitHubRepositoryIdentity) GetFullNameOk() (*string, bool)`

GetFullNameOk returns a tuple with the FullName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFullName

`func (o *GitHubRepositoryIdentity) SetFullName(v string)`

SetFullName sets FullName field to given value.


### GetLink

`func (o *GitHubRepositoryIdentity) GetLink() string`

GetLink returns the Link field if non-nil, zero value otherwise.

### GetLinkOk

`func (o *GitHubRepositoryIdentity) GetLinkOk() (*string, bool)`

GetLinkOk returns a tuple with the Link field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLink

`func (o *GitHubRepositoryIdentity) SetLink(v string)`

SetLink sets Link field to given value.


### GetOwner

`func (o *GitHubRepositoryIdentity) GetOwner() GitHubRepositoryAccount`

GetOwner returns the Owner field if non-nil, zero value otherwise.

### GetOwnerOk

`func (o *GitHubRepositoryIdentity) GetOwnerOk() (*GitHubRepositoryAccount, bool)`

GetOwnerOk returns a tuple with the Owner field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOwner

`func (o *GitHubRepositoryIdentity) SetOwner(v GitHubRepositoryAccount)`

SetOwner sets Owner field to given value.


### GetIsEmpty

`func (o *GitHubRepositoryIdentity) GetIsEmpty() bool`

GetIsEmpty returns the IsEmpty field if non-nil, zero value otherwise.

### GetIsEmptyOk

`func (o *GitHubRepositoryIdentity) GetIsEmptyOk() (*bool, bool)`

GetIsEmptyOk returns a tuple with the IsEmpty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsEmpty

`func (o *GitHubRepositoryIdentity) SetIsEmpty(v bool)`

SetIsEmpty sets IsEmpty field to given value.


### GetId

`func (o *GitHubRepositoryIdentity) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *GitHubRepositoryIdentity) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *GitHubRepositoryIdentity) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *GitHubRepositoryIdentity) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *GitHubRepositoryIdentity) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *GitHubRepositoryIdentity) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil
### GetNodeId

`func (o *GitHubRepositoryIdentity) GetNodeId() string`

GetNodeId returns the NodeId field if non-nil, zero value otherwise.

### GetNodeIdOk

`func (o *GitHubRepositoryIdentity) GetNodeIdOk() (*string, bool)`

GetNodeIdOk returns a tuple with the NodeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNodeId

`func (o *GitHubRepositoryIdentity) SetNodeId(v string)`

SetNodeId sets NodeId field to given value.

### HasNodeId

`func (o *GitHubRepositoryIdentity) HasNodeId() bool`

HasNodeId returns a boolean if a field has been set.

### SetNodeIdNil

`func (o *GitHubRepositoryIdentity) SetNodeIdNil(b bool)`

 SetNodeIdNil sets the value for NodeId to be an explicit nil

### UnsetNodeId
`func (o *GitHubRepositoryIdentity) UnsetNodeId()`

UnsetNodeId ensures that no value is present for NodeId, not even an explicit nil
### GetDescription

`func (o *GitHubRepositoryIdentity) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *GitHubRepositoryIdentity) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *GitHubRepositoryIdentity) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *GitHubRepositoryIdentity) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *GitHubRepositoryIdentity) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *GitHubRepositoryIdentity) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetWebsite

`func (o *GitHubRepositoryIdentity) GetWebsite() string`

GetWebsite returns the Website field if non-nil, zero value otherwise.

### GetWebsiteOk

`func (o *GitHubRepositoryIdentity) GetWebsiteOk() (*string, bool)`

GetWebsiteOk returns a tuple with the Website field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebsite

`func (o *GitHubRepositoryIdentity) SetWebsite(v string)`

SetWebsite sets Website field to given value.

### HasWebsite

`func (o *GitHubRepositoryIdentity) HasWebsite() bool`

HasWebsite returns a boolean if a field has been set.

### SetWebsiteNil

`func (o *GitHubRepositoryIdentity) SetWebsiteNil(b bool)`

 SetWebsiteNil sets the value for Website to be an explicit nil

### UnsetWebsite
`func (o *GitHubRepositoryIdentity) UnsetWebsite()`

UnsetWebsite ensures that no value is present for Website, not even an explicit nil
### GetSocialImage

`func (o *GitHubRepositoryIdentity) GetSocialImage() string`

GetSocialImage returns the SocialImage field if non-nil, zero value otherwise.

### GetSocialImageOk

`func (o *GitHubRepositoryIdentity) GetSocialImageOk() (*string, bool)`

GetSocialImageOk returns a tuple with the SocialImage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSocialImage

`func (o *GitHubRepositoryIdentity) SetSocialImage(v string)`

SetSocialImage sets SocialImage field to given value.

### HasSocialImage

`func (o *GitHubRepositoryIdentity) HasSocialImage() bool`

HasSocialImage returns a boolean if a field has been set.

### SetSocialImageNil

`func (o *GitHubRepositoryIdentity) SetSocialImageNil(b bool)`

 SetSocialImageNil sets the value for SocialImage to be an explicit nil

### UnsetSocialImage
`func (o *GitHubRepositoryIdentity) UnsetSocialImage()`

UnsetSocialImage ensures that no value is present for SocialImage, not even an explicit nil
### GetDefaultBranch

`func (o *GitHubRepositoryIdentity) GetDefaultBranch() string`

GetDefaultBranch returns the DefaultBranch field if non-nil, zero value otherwise.

### GetDefaultBranchOk

`func (o *GitHubRepositoryIdentity) GetDefaultBranchOk() (*string, bool)`

GetDefaultBranchOk returns a tuple with the DefaultBranch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultBranch

`func (o *GitHubRepositoryIdentity) SetDefaultBranch(v string)`

SetDefaultBranch sets DefaultBranch field to given value.

### HasDefaultBranch

`func (o *GitHubRepositoryIdentity) HasDefaultBranch() bool`

HasDefaultBranch returns a boolean if a field has been set.

### SetDefaultBranchNil

`func (o *GitHubRepositoryIdentity) SetDefaultBranchNil(b bool)`

 SetDefaultBranchNil sets the value for DefaultBranch to be an explicit nil

### UnsetDefaultBranch
`func (o *GitHubRepositoryIdentity) UnsetDefaultBranch()`

UnsetDefaultBranch ensures that no value is present for DefaultBranch, not even an explicit nil
### GetCurrentCommit

`func (o *GitHubRepositoryIdentity) GetCurrentCommit() string`

GetCurrentCommit returns the CurrentCommit field if non-nil, zero value otherwise.

### GetCurrentCommitOk

`func (o *GitHubRepositoryIdentity) GetCurrentCommitOk() (*string, bool)`

GetCurrentCommitOk returns a tuple with the CurrentCommit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrentCommit

`func (o *GitHubRepositoryIdentity) SetCurrentCommit(v string)`

SetCurrentCommit sets CurrentCommit field to given value.

### HasCurrentCommit

`func (o *GitHubRepositoryIdentity) HasCurrentCommit() bool`

HasCurrentCommit returns a boolean if a field has been set.

### SetCurrentCommitNil

`func (o *GitHubRepositoryIdentity) SetCurrentCommitNil(b bool)`

 SetCurrentCommitNil sets the value for CurrentCommit to be an explicit nil

### UnsetCurrentCommit
`func (o *GitHubRepositoryIdentity) UnsetCurrentCommit()`

UnsetCurrentCommit ensures that no value is present for CurrentCommit, not even an explicit nil
### GetVisibility

`func (o *GitHubRepositoryIdentity) GetVisibility() string`

GetVisibility returns the Visibility field if non-nil, zero value otherwise.

### GetVisibilityOk

`func (o *GitHubRepositoryIdentity) GetVisibilityOk() (*string, bool)`

GetVisibilityOk returns a tuple with the Visibility field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVisibility

`func (o *GitHubRepositoryIdentity) SetVisibility(v string)`

SetVisibility sets Visibility field to given value.

### HasVisibility

`func (o *GitHubRepositoryIdentity) HasVisibility() bool`

HasVisibility returns a boolean if a field has been set.

### SetVisibilityNil

`func (o *GitHubRepositoryIdentity) SetVisibilityNil(b bool)`

 SetVisibilityNil sets the value for Visibility to be an explicit nil

### UnsetVisibility
`func (o *GitHubRepositoryIdentity) UnsetVisibility()`

UnsetVisibility ensures that no value is present for Visibility, not even an explicit nil
### GetIsFork

`func (o *GitHubRepositoryIdentity) GetIsFork() bool`

GetIsFork returns the IsFork field if non-nil, zero value otherwise.

### GetIsForkOk

`func (o *GitHubRepositoryIdentity) GetIsForkOk() (*bool, bool)`

GetIsForkOk returns a tuple with the IsFork field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsFork

`func (o *GitHubRepositoryIdentity) SetIsFork(v bool)`

SetIsFork sets IsFork field to given value.

### HasIsFork

`func (o *GitHubRepositoryIdentity) HasIsFork() bool`

HasIsFork returns a boolean if a field has been set.

### SetIsForkNil

`func (o *GitHubRepositoryIdentity) SetIsForkNil(b bool)`

 SetIsForkNil sets the value for IsFork to be an explicit nil

### UnsetIsFork
`func (o *GitHubRepositoryIdentity) UnsetIsFork()`

UnsetIsFork ensures that no value is present for IsFork, not even an explicit nil
### GetForkedFrom

`func (o *GitHubRepositoryIdentity) GetForkedFrom() string`

GetForkedFrom returns the ForkedFrom field if non-nil, zero value otherwise.

### GetForkedFromOk

`func (o *GitHubRepositoryIdentity) GetForkedFromOk() (*string, bool)`

GetForkedFromOk returns a tuple with the ForkedFrom field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetForkedFrom

`func (o *GitHubRepositoryIdentity) SetForkedFrom(v string)`

SetForkedFrom sets ForkedFrom field to given value.

### HasForkedFrom

`func (o *GitHubRepositoryIdentity) HasForkedFrom() bool`

HasForkedFrom returns a boolean if a field has been set.

### SetForkedFromNil

`func (o *GitHubRepositoryIdentity) SetForkedFromNil(b bool)`

 SetForkedFromNil sets the value for ForkedFrom to be an explicit nil

### UnsetForkedFrom
`func (o *GitHubRepositoryIdentity) UnsetForkedFrom()`

UnsetForkedFrom ensures that no value is present for ForkedFrom, not even an explicit nil
### GetParent

`func (o *GitHubRepositoryIdentity) GetParent() GitHubRepositoryReference`

GetParent returns the Parent field if non-nil, zero value otherwise.

### GetParentOk

`func (o *GitHubRepositoryIdentity) GetParentOk() (*GitHubRepositoryReference, bool)`

GetParentOk returns a tuple with the Parent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParent

`func (o *GitHubRepositoryIdentity) SetParent(v GitHubRepositoryReference)`

SetParent sets Parent field to given value.

### HasParent

`func (o *GitHubRepositoryIdentity) HasParent() bool`

HasParent returns a boolean if a field has been set.

### SetParentNil

`func (o *GitHubRepositoryIdentity) SetParentNil(b bool)`

 SetParentNil sets the value for Parent to be an explicit nil

### UnsetParent
`func (o *GitHubRepositoryIdentity) UnsetParent()`

UnsetParent ensures that no value is present for Parent, not even an explicit nil
### GetSource

`func (o *GitHubRepositoryIdentity) GetSource() GitHubRepositoryReference`

GetSource returns the Source field if non-nil, zero value otherwise.

### GetSourceOk

`func (o *GitHubRepositoryIdentity) GetSourceOk() (*GitHubRepositoryReference, bool)`

GetSourceOk returns a tuple with the Source field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSource

`func (o *GitHubRepositoryIdentity) SetSource(v GitHubRepositoryReference)`

SetSource sets Source field to given value.

### HasSource

`func (o *GitHubRepositoryIdentity) HasSource() bool`

HasSource returns a boolean if a field has been set.

### SetSourceNil

`func (o *GitHubRepositoryIdentity) SetSourceNil(b bool)`

 SetSourceNil sets the value for Source to be an explicit nil

### UnsetSource
`func (o *GitHubRepositoryIdentity) UnsetSource()`

UnsetSource ensures that no value is present for Source, not even an explicit nil
### GetForkComparison

`func (o *GitHubRepositoryIdentity) GetForkComparison() GitHubForkComparison`

GetForkComparison returns the ForkComparison field if non-nil, zero value otherwise.

### GetForkComparisonOk

`func (o *GitHubRepositoryIdentity) GetForkComparisonOk() (*GitHubForkComparison, bool)`

GetForkComparisonOk returns a tuple with the ForkComparison field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetForkComparison

`func (o *GitHubRepositoryIdentity) SetForkComparison(v GitHubForkComparison)`

SetForkComparison sets ForkComparison field to given value.

### HasForkComparison

`func (o *GitHubRepositoryIdentity) HasForkComparison() bool`

HasForkComparison returns a boolean if a field has been set.

### SetForkComparisonNil

`func (o *GitHubRepositoryIdentity) SetForkComparisonNil(b bool)`

 SetForkComparisonNil sets the value for ForkComparison to be an explicit nil

### UnsetForkComparison
`func (o *GitHubRepositoryIdentity) UnsetForkComparison()`

UnsetForkComparison ensures that no value is present for ForkComparison, not even an explicit nil
### GetIsArchived

`func (o *GitHubRepositoryIdentity) GetIsArchived() bool`

GetIsArchived returns the IsArchived field if non-nil, zero value otherwise.

### GetIsArchivedOk

`func (o *GitHubRepositoryIdentity) GetIsArchivedOk() (*bool, bool)`

GetIsArchivedOk returns a tuple with the IsArchived field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsArchived

`func (o *GitHubRepositoryIdentity) SetIsArchived(v bool)`

SetIsArchived sets IsArchived field to given value.

### HasIsArchived

`func (o *GitHubRepositoryIdentity) HasIsArchived() bool`

HasIsArchived returns a boolean if a field has been set.

### SetIsArchivedNil

`func (o *GitHubRepositoryIdentity) SetIsArchivedNil(b bool)`

 SetIsArchivedNil sets the value for IsArchived to be an explicit nil

### UnsetIsArchived
`func (o *GitHubRepositoryIdentity) UnsetIsArchived()`

UnsetIsArchived ensures that no value is present for IsArchived, not even an explicit nil
### GetIsTemplate

`func (o *GitHubRepositoryIdentity) GetIsTemplate() bool`

GetIsTemplate returns the IsTemplate field if non-nil, zero value otherwise.

### GetIsTemplateOk

`func (o *GitHubRepositoryIdentity) GetIsTemplateOk() (*bool, bool)`

GetIsTemplateOk returns a tuple with the IsTemplate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsTemplate

`func (o *GitHubRepositoryIdentity) SetIsTemplate(v bool)`

SetIsTemplate sets IsTemplate field to given value.

### HasIsTemplate

`func (o *GitHubRepositoryIdentity) HasIsTemplate() bool`

HasIsTemplate returns a boolean if a field has been set.

### SetIsTemplateNil

`func (o *GitHubRepositoryIdentity) SetIsTemplateNil(b bool)`

 SetIsTemplateNil sets the value for IsTemplate to be an explicit nil

### UnsetIsTemplate
`func (o *GitHubRepositoryIdentity) UnsetIsTemplate()`

UnsetIsTemplate ensures that no value is present for IsTemplate, not even an explicit nil
### GetIsMirror

`func (o *GitHubRepositoryIdentity) GetIsMirror() bool`

GetIsMirror returns the IsMirror field if non-nil, zero value otherwise.

### GetIsMirrorOk

`func (o *GitHubRepositoryIdentity) GetIsMirrorOk() (*bool, bool)`

GetIsMirrorOk returns a tuple with the IsMirror field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsMirror

`func (o *GitHubRepositoryIdentity) SetIsMirror(v bool)`

SetIsMirror sets IsMirror field to given value.

### HasIsMirror

`func (o *GitHubRepositoryIdentity) HasIsMirror() bool`

HasIsMirror returns a boolean if a field has been set.

### SetIsMirrorNil

`func (o *GitHubRepositoryIdentity) SetIsMirrorNil(b bool)`

 SetIsMirrorNil sets the value for IsMirror to be an explicit nil

### UnsetIsMirror
`func (o *GitHubRepositoryIdentity) UnsetIsMirror()`

UnsetIsMirror ensures that no value is present for IsMirror, not even an explicit nil
### GetIsDisabled

`func (o *GitHubRepositoryIdentity) GetIsDisabled() bool`

GetIsDisabled returns the IsDisabled field if non-nil, zero value otherwise.

### GetIsDisabledOk

`func (o *GitHubRepositoryIdentity) GetIsDisabledOk() (*bool, bool)`

GetIsDisabledOk returns a tuple with the IsDisabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDisabled

`func (o *GitHubRepositoryIdentity) SetIsDisabled(v bool)`

SetIsDisabled sets IsDisabled field to given value.

### HasIsDisabled

`func (o *GitHubRepositoryIdentity) HasIsDisabled() bool`

HasIsDisabled returns a boolean if a field has been set.

### SetIsDisabledNil

`func (o *GitHubRepositoryIdentity) SetIsDisabledNil(b bool)`

 SetIsDisabledNil sets the value for IsDisabled to be an explicit nil

### UnsetIsDisabled
`func (o *GitHubRepositoryIdentity) UnsetIsDisabled()`

UnsetIsDisabled ensures that no value is present for IsDisabled, not even an explicit nil
### GetLanguage

`func (o *GitHubRepositoryIdentity) GetLanguage() string`

GetLanguage returns the Language field if non-nil, zero value otherwise.

### GetLanguageOk

`func (o *GitHubRepositoryIdentity) GetLanguageOk() (*string, bool)`

GetLanguageOk returns a tuple with the Language field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLanguage

`func (o *GitHubRepositoryIdentity) SetLanguage(v string)`

SetLanguage sets Language field to given value.

### HasLanguage

`func (o *GitHubRepositoryIdentity) HasLanguage() bool`

HasLanguage returns a boolean if a field has been set.

### SetLanguageNil

`func (o *GitHubRepositoryIdentity) SetLanguageNil(b bool)`

 SetLanguageNil sets the value for Language to be an explicit nil

### UnsetLanguage
`func (o *GitHubRepositoryIdentity) UnsetLanguage()`

UnsetLanguage ensures that no value is present for Language, not even an explicit nil
### GetLanguageColor

`func (o *GitHubRepositoryIdentity) GetLanguageColor() string`

GetLanguageColor returns the LanguageColor field if non-nil, zero value otherwise.

### GetLanguageColorOk

`func (o *GitHubRepositoryIdentity) GetLanguageColorOk() (*string, bool)`

GetLanguageColorOk returns a tuple with the LanguageColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLanguageColor

`func (o *GitHubRepositoryIdentity) SetLanguageColor(v string)`

SetLanguageColor sets LanguageColor field to given value.

### HasLanguageColor

`func (o *GitHubRepositoryIdentity) HasLanguageColor() bool`

HasLanguageColor returns a boolean if a field has been set.

### SetLanguageColorNil

`func (o *GitHubRepositoryIdentity) SetLanguageColorNil(b bool)`

 SetLanguageColorNil sets the value for LanguageColor to be an explicit nil

### UnsetLanguageColor
`func (o *GitHubRepositoryIdentity) UnsetLanguageColor()`

UnsetLanguageColor ensures that no value is present for LanguageColor, not even an explicit nil
### GetLicense

`func (o *GitHubRepositoryIdentity) GetLicense() GitHubRepositoryLicense`

GetLicense returns the License field if non-nil, zero value otherwise.

### GetLicenseOk

`func (o *GitHubRepositoryIdentity) GetLicenseOk() (*GitHubRepositoryLicense, bool)`

GetLicenseOk returns a tuple with the License field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLicense

`func (o *GitHubRepositoryIdentity) SetLicense(v GitHubRepositoryLicense)`

SetLicense sets License field to given value.

### HasLicense

`func (o *GitHubRepositoryIdentity) HasLicense() bool`

HasLicense returns a boolean if a field has been set.

### SetLicenseNil

`func (o *GitHubRepositoryIdentity) SetLicenseNil(b bool)`

 SetLicenseNil sets the value for License to be an explicit nil

### UnsetLicense
`func (o *GitHubRepositoryIdentity) UnsetLicense()`

UnsetLicense ensures that no value is present for License, not even an explicit nil
### GetTopics

`func (o *GitHubRepositoryIdentity) GetTopics() []string`

GetTopics returns the Topics field if non-nil, zero value otherwise.

### GetTopicsOk

`func (o *GitHubRepositoryIdentity) GetTopicsOk() (*[]string, bool)`

GetTopicsOk returns a tuple with the Topics field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTopics

`func (o *GitHubRepositoryIdentity) SetTopics(v []string)`

SetTopics sets Topics field to given value.

### HasTopics

`func (o *GitHubRepositoryIdentity) HasTopics() bool`

HasTopics returns a boolean if a field has been set.

### SetTopicsNil

`func (o *GitHubRepositoryIdentity) SetTopicsNil(b bool)`

 SetTopicsNil sets the value for Topics to be an explicit nil

### UnsetTopics
`func (o *GitHubRepositoryIdentity) UnsetTopics()`

UnsetTopics ensures that no value is present for Topics, not even an explicit nil
### GetStars

`func (o *GitHubRepositoryIdentity) GetStars() int32`

GetStars returns the Stars field if non-nil, zero value otherwise.

### GetStarsOk

`func (o *GitHubRepositoryIdentity) GetStarsOk() (*int32, bool)`

GetStarsOk returns a tuple with the Stars field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStars

`func (o *GitHubRepositoryIdentity) SetStars(v int32)`

SetStars sets Stars field to given value.

### HasStars

`func (o *GitHubRepositoryIdentity) HasStars() bool`

HasStars returns a boolean if a field has been set.

### SetStarsNil

`func (o *GitHubRepositoryIdentity) SetStarsNil(b bool)`

 SetStarsNil sets the value for Stars to be an explicit nil

### UnsetStars
`func (o *GitHubRepositoryIdentity) UnsetStars()`

UnsetStars ensures that no value is present for Stars, not even an explicit nil
### GetWatchers

`func (o *GitHubRepositoryIdentity) GetWatchers() int32`

GetWatchers returns the Watchers field if non-nil, zero value otherwise.

### GetWatchersOk

`func (o *GitHubRepositoryIdentity) GetWatchersOk() (*int32, bool)`

GetWatchersOk returns a tuple with the Watchers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWatchers

`func (o *GitHubRepositoryIdentity) SetWatchers(v int32)`

SetWatchers sets Watchers field to given value.

### HasWatchers

`func (o *GitHubRepositoryIdentity) HasWatchers() bool`

HasWatchers returns a boolean if a field has been set.

### SetWatchersNil

`func (o *GitHubRepositoryIdentity) SetWatchersNil(b bool)`

 SetWatchersNil sets the value for Watchers to be an explicit nil

### UnsetWatchers
`func (o *GitHubRepositoryIdentity) UnsetWatchers()`

UnsetWatchers ensures that no value is present for Watchers, not even an explicit nil
### GetForks

`func (o *GitHubRepositoryIdentity) GetForks() int32`

GetForks returns the Forks field if non-nil, zero value otherwise.

### GetForksOk

`func (o *GitHubRepositoryIdentity) GetForksOk() (*int32, bool)`

GetForksOk returns a tuple with the Forks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetForks

`func (o *GitHubRepositoryIdentity) SetForks(v int32)`

SetForks sets Forks field to given value.

### HasForks

`func (o *GitHubRepositoryIdentity) HasForks() bool`

HasForks returns a boolean if a field has been set.

### SetForksNil

`func (o *GitHubRepositoryIdentity) SetForksNil(b bool)`

 SetForksNil sets the value for Forks to be an explicit nil

### UnsetForks
`func (o *GitHubRepositoryIdentity) UnsetForks()`

UnsetForks ensures that no value is present for Forks, not even an explicit nil
### GetNetworkCount

`func (o *GitHubRepositoryIdentity) GetNetworkCount() int32`

GetNetworkCount returns the NetworkCount field if non-nil, zero value otherwise.

### GetNetworkCountOk

`func (o *GitHubRepositoryIdentity) GetNetworkCountOk() (*int32, bool)`

GetNetworkCountOk returns a tuple with the NetworkCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNetworkCount

`func (o *GitHubRepositoryIdentity) SetNetworkCount(v int32)`

SetNetworkCount sets NetworkCount field to given value.

### HasNetworkCount

`func (o *GitHubRepositoryIdentity) HasNetworkCount() bool`

HasNetworkCount returns a boolean if a field has been set.

### SetNetworkCountNil

`func (o *GitHubRepositoryIdentity) SetNetworkCountNil(b bool)`

 SetNetworkCountNil sets the value for NetworkCount to be an explicit nil

### UnsetNetworkCount
`func (o *GitHubRepositoryIdentity) UnsetNetworkCount()`

UnsetNetworkCount ensures that no value is present for NetworkCount, not even an explicit nil
### GetOpenIssuesCount

`func (o *GitHubRepositoryIdentity) GetOpenIssuesCount() int32`

GetOpenIssuesCount returns the OpenIssuesCount field if non-nil, zero value otherwise.

### GetOpenIssuesCountOk

`func (o *GitHubRepositoryIdentity) GetOpenIssuesCountOk() (*int32, bool)`

GetOpenIssuesCountOk returns a tuple with the OpenIssuesCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOpenIssuesCount

`func (o *GitHubRepositoryIdentity) SetOpenIssuesCount(v int32)`

SetOpenIssuesCount sets OpenIssuesCount field to given value.

### HasOpenIssuesCount

`func (o *GitHubRepositoryIdentity) HasOpenIssuesCount() bool`

HasOpenIssuesCount returns a boolean if a field has been set.

### SetOpenIssuesCountNil

`func (o *GitHubRepositoryIdentity) SetOpenIssuesCountNil(b bool)`

 SetOpenIssuesCountNil sets the value for OpenIssuesCount to be an explicit nil

### UnsetOpenIssuesCount
`func (o *GitHubRepositoryIdentity) UnsetOpenIssuesCount()`

UnsetOpenIssuesCount ensures that no value is present for OpenIssuesCount, not even an explicit nil
### GetOpenPullRequestsCount

`func (o *GitHubRepositoryIdentity) GetOpenPullRequestsCount() int32`

GetOpenPullRequestsCount returns the OpenPullRequestsCount field if non-nil, zero value otherwise.

### GetOpenPullRequestsCountOk

`func (o *GitHubRepositoryIdentity) GetOpenPullRequestsCountOk() (*int32, bool)`

GetOpenPullRequestsCountOk returns a tuple with the OpenPullRequestsCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOpenPullRequestsCount

`func (o *GitHubRepositoryIdentity) SetOpenPullRequestsCount(v int32)`

SetOpenPullRequestsCount sets OpenPullRequestsCount field to given value.

### HasOpenPullRequestsCount

`func (o *GitHubRepositoryIdentity) HasOpenPullRequestsCount() bool`

HasOpenPullRequestsCount returns a boolean if a field has been set.

### SetOpenPullRequestsCountNil

`func (o *GitHubRepositoryIdentity) SetOpenPullRequestsCountNil(b bool)`

 SetOpenPullRequestsCountNil sets the value for OpenPullRequestsCount to be an explicit nil

### UnsetOpenPullRequestsCount
`func (o *GitHubRepositoryIdentity) UnsetOpenPullRequestsCount()`

UnsetOpenPullRequestsCount ensures that no value is present for OpenPullRequestsCount, not even an explicit nil
### GetOpenIssuesCountApproximate

`func (o *GitHubRepositoryIdentity) GetOpenIssuesCountApproximate() bool`

GetOpenIssuesCountApproximate returns the OpenIssuesCountApproximate field if non-nil, zero value otherwise.

### GetOpenIssuesCountApproximateOk

`func (o *GitHubRepositoryIdentity) GetOpenIssuesCountApproximateOk() (*bool, bool)`

GetOpenIssuesCountApproximateOk returns a tuple with the OpenIssuesCountApproximate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOpenIssuesCountApproximate

`func (o *GitHubRepositoryIdentity) SetOpenIssuesCountApproximate(v bool)`

SetOpenIssuesCountApproximate sets OpenIssuesCountApproximate field to given value.

### HasOpenIssuesCountApproximate

`func (o *GitHubRepositoryIdentity) HasOpenIssuesCountApproximate() bool`

HasOpenIssuesCountApproximate returns a boolean if a field has been set.

### SetOpenIssuesCountApproximateNil

`func (o *GitHubRepositoryIdentity) SetOpenIssuesCountApproximateNil(b bool)`

 SetOpenIssuesCountApproximateNil sets the value for OpenIssuesCountApproximate to be an explicit nil

### UnsetOpenIssuesCountApproximate
`func (o *GitHubRepositoryIdentity) UnsetOpenIssuesCountApproximate()`

UnsetOpenIssuesCountApproximate ensures that no value is present for OpenIssuesCountApproximate, not even an explicit nil
### GetOpenPullRequestsCountApproximate

`func (o *GitHubRepositoryIdentity) GetOpenPullRequestsCountApproximate() bool`

GetOpenPullRequestsCountApproximate returns the OpenPullRequestsCountApproximate field if non-nil, zero value otherwise.

### GetOpenPullRequestsCountApproximateOk

`func (o *GitHubRepositoryIdentity) GetOpenPullRequestsCountApproximateOk() (*bool, bool)`

GetOpenPullRequestsCountApproximateOk returns a tuple with the OpenPullRequestsCountApproximate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOpenPullRequestsCountApproximate

`func (o *GitHubRepositoryIdentity) SetOpenPullRequestsCountApproximate(v bool)`

SetOpenPullRequestsCountApproximate sets OpenPullRequestsCountApproximate field to given value.

### HasOpenPullRequestsCountApproximate

`func (o *GitHubRepositoryIdentity) HasOpenPullRequestsCountApproximate() bool`

HasOpenPullRequestsCountApproximate returns a boolean if a field has been set.

### SetOpenPullRequestsCountApproximateNil

`func (o *GitHubRepositoryIdentity) SetOpenPullRequestsCountApproximateNil(b bool)`

 SetOpenPullRequestsCountApproximateNil sets the value for OpenPullRequestsCountApproximate to be an explicit nil

### UnsetOpenPullRequestsCountApproximate
`func (o *GitHubRepositoryIdentity) UnsetOpenPullRequestsCountApproximate()`

UnsetOpenPullRequestsCountApproximate ensures that no value is present for OpenPullRequestsCountApproximate, not even an explicit nil
### GetOpenIssuesDisplay

`func (o *GitHubRepositoryIdentity) GetOpenIssuesDisplay() string`

GetOpenIssuesDisplay returns the OpenIssuesDisplay field if non-nil, zero value otherwise.

### GetOpenIssuesDisplayOk

`func (o *GitHubRepositoryIdentity) GetOpenIssuesDisplayOk() (*string, bool)`

GetOpenIssuesDisplayOk returns a tuple with the OpenIssuesDisplay field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOpenIssuesDisplay

`func (o *GitHubRepositoryIdentity) SetOpenIssuesDisplay(v string)`

SetOpenIssuesDisplay sets OpenIssuesDisplay field to given value.

### HasOpenIssuesDisplay

`func (o *GitHubRepositoryIdentity) HasOpenIssuesDisplay() bool`

HasOpenIssuesDisplay returns a boolean if a field has been set.

### SetOpenIssuesDisplayNil

`func (o *GitHubRepositoryIdentity) SetOpenIssuesDisplayNil(b bool)`

 SetOpenIssuesDisplayNil sets the value for OpenIssuesDisplay to be an explicit nil

### UnsetOpenIssuesDisplay
`func (o *GitHubRepositoryIdentity) UnsetOpenIssuesDisplay()`

UnsetOpenIssuesDisplay ensures that no value is present for OpenIssuesDisplay, not even an explicit nil
### GetOpenPullRequestsDisplay

`func (o *GitHubRepositoryIdentity) GetOpenPullRequestsDisplay() string`

GetOpenPullRequestsDisplay returns the OpenPullRequestsDisplay field if non-nil, zero value otherwise.

### GetOpenPullRequestsDisplayOk

`func (o *GitHubRepositoryIdentity) GetOpenPullRequestsDisplayOk() (*string, bool)`

GetOpenPullRequestsDisplayOk returns a tuple with the OpenPullRequestsDisplay field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOpenPullRequestsDisplay

`func (o *GitHubRepositoryIdentity) SetOpenPullRequestsDisplay(v string)`

SetOpenPullRequestsDisplay sets OpenPullRequestsDisplay field to given value.

### HasOpenPullRequestsDisplay

`func (o *GitHubRepositoryIdentity) HasOpenPullRequestsDisplay() bool`

HasOpenPullRequestsDisplay returns a boolean if a field has been set.

### SetOpenPullRequestsDisplayNil

`func (o *GitHubRepositoryIdentity) SetOpenPullRequestsDisplayNil(b bool)`

 SetOpenPullRequestsDisplayNil sets the value for OpenPullRequestsDisplay to be an explicit nil

### UnsetOpenPullRequestsDisplay
`func (o *GitHubRepositoryIdentity) UnsetOpenPullRequestsDisplay()`

UnsetOpenPullRequestsDisplay ensures that no value is present for OpenPullRequestsDisplay, not even an explicit nil
### GetIsOpenIssuesCountCapped

`func (o *GitHubRepositoryIdentity) GetIsOpenIssuesCountCapped() bool`

GetIsOpenIssuesCountCapped returns the IsOpenIssuesCountCapped field if non-nil, zero value otherwise.

### GetIsOpenIssuesCountCappedOk

`func (o *GitHubRepositoryIdentity) GetIsOpenIssuesCountCappedOk() (*bool, bool)`

GetIsOpenIssuesCountCappedOk returns a tuple with the IsOpenIssuesCountCapped field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsOpenIssuesCountCapped

`func (o *GitHubRepositoryIdentity) SetIsOpenIssuesCountCapped(v bool)`

SetIsOpenIssuesCountCapped sets IsOpenIssuesCountCapped field to given value.

### HasIsOpenIssuesCountCapped

`func (o *GitHubRepositoryIdentity) HasIsOpenIssuesCountCapped() bool`

HasIsOpenIssuesCountCapped returns a boolean if a field has been set.

### SetIsOpenIssuesCountCappedNil

`func (o *GitHubRepositoryIdentity) SetIsOpenIssuesCountCappedNil(b bool)`

 SetIsOpenIssuesCountCappedNil sets the value for IsOpenIssuesCountCapped to be an explicit nil

### UnsetIsOpenIssuesCountCapped
`func (o *GitHubRepositoryIdentity) UnsetIsOpenIssuesCountCapped()`

UnsetIsOpenIssuesCountCapped ensures that no value is present for IsOpenIssuesCountCapped, not even an explicit nil
### GetIsOpenPullRequestsCountCapped

`func (o *GitHubRepositoryIdentity) GetIsOpenPullRequestsCountCapped() bool`

GetIsOpenPullRequestsCountCapped returns the IsOpenPullRequestsCountCapped field if non-nil, zero value otherwise.

### GetIsOpenPullRequestsCountCappedOk

`func (o *GitHubRepositoryIdentity) GetIsOpenPullRequestsCountCappedOk() (*bool, bool)`

GetIsOpenPullRequestsCountCappedOk returns a tuple with the IsOpenPullRequestsCountCapped field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsOpenPullRequestsCountCapped

`func (o *GitHubRepositoryIdentity) SetIsOpenPullRequestsCountCapped(v bool)`

SetIsOpenPullRequestsCountCapped sets IsOpenPullRequestsCountCapped field to given value.

### HasIsOpenPullRequestsCountCapped

`func (o *GitHubRepositoryIdentity) HasIsOpenPullRequestsCountCapped() bool`

HasIsOpenPullRequestsCountCapped returns a boolean if a field has been set.

### SetIsOpenPullRequestsCountCappedNil

`func (o *GitHubRepositoryIdentity) SetIsOpenPullRequestsCountCappedNil(b bool)`

 SetIsOpenPullRequestsCountCappedNil sets the value for IsOpenPullRequestsCountCapped to be an explicit nil

### UnsetIsOpenPullRequestsCountCapped
`func (o *GitHubRepositoryIdentity) UnsetIsOpenPullRequestsCountCapped()`

UnsetIsOpenPullRequestsCountCapped ensures that no value is present for IsOpenPullRequestsCountCapped, not even an explicit nil
### GetOpenIssuesAndPullRequestsCount

`func (o *GitHubRepositoryIdentity) GetOpenIssuesAndPullRequestsCount() int32`

GetOpenIssuesAndPullRequestsCount returns the OpenIssuesAndPullRequestsCount field if non-nil, zero value otherwise.

### GetOpenIssuesAndPullRequestsCountOk

`func (o *GitHubRepositoryIdentity) GetOpenIssuesAndPullRequestsCountOk() (*int32, bool)`

GetOpenIssuesAndPullRequestsCountOk returns a tuple with the OpenIssuesAndPullRequestsCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOpenIssuesAndPullRequestsCount

`func (o *GitHubRepositoryIdentity) SetOpenIssuesAndPullRequestsCount(v int32)`

SetOpenIssuesAndPullRequestsCount sets OpenIssuesAndPullRequestsCount field to given value.

### HasOpenIssuesAndPullRequestsCount

`func (o *GitHubRepositoryIdentity) HasOpenIssuesAndPullRequestsCount() bool`

HasOpenIssuesAndPullRequestsCount returns a boolean if a field has been set.

### SetOpenIssuesAndPullRequestsCountNil

`func (o *GitHubRepositoryIdentity) SetOpenIssuesAndPullRequestsCountNil(b bool)`

 SetOpenIssuesAndPullRequestsCountNil sets the value for OpenIssuesAndPullRequestsCount to be an explicit nil

### UnsetOpenIssuesAndPullRequestsCount
`func (o *GitHubRepositoryIdentity) UnsetOpenIssuesAndPullRequestsCount()`

UnsetOpenIssuesAndPullRequestsCount ensures that no value is present for OpenIssuesAndPullRequestsCount, not even an explicit nil
### GetCommitsCount

`func (o *GitHubRepositoryIdentity) GetCommitsCount() int32`

GetCommitsCount returns the CommitsCount field if non-nil, zero value otherwise.

### GetCommitsCountOk

`func (o *GitHubRepositoryIdentity) GetCommitsCountOk() (*int32, bool)`

GetCommitsCountOk returns a tuple with the CommitsCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommitsCount

`func (o *GitHubRepositoryIdentity) SetCommitsCount(v int32)`

SetCommitsCount sets CommitsCount field to given value.

### HasCommitsCount

`func (o *GitHubRepositoryIdentity) HasCommitsCount() bool`

HasCommitsCount returns a boolean if a field has been set.

### SetCommitsCountNil

`func (o *GitHubRepositoryIdentity) SetCommitsCountNil(b bool)`

 SetCommitsCountNil sets the value for CommitsCount to be an explicit nil

### UnsetCommitsCount
`func (o *GitHubRepositoryIdentity) UnsetCommitsCount()`

UnsetCommitsCount ensures that no value is present for CommitsCount, not even an explicit nil
### GetCommitsDisplay

`func (o *GitHubRepositoryIdentity) GetCommitsDisplay() string`

GetCommitsDisplay returns the CommitsDisplay field if non-nil, zero value otherwise.

### GetCommitsDisplayOk

`func (o *GitHubRepositoryIdentity) GetCommitsDisplayOk() (*string, bool)`

GetCommitsDisplayOk returns a tuple with the CommitsDisplay field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommitsDisplay

`func (o *GitHubRepositoryIdentity) SetCommitsDisplay(v string)`

SetCommitsDisplay sets CommitsDisplay field to given value.

### HasCommitsDisplay

`func (o *GitHubRepositoryIdentity) HasCommitsDisplay() bool`

HasCommitsDisplay returns a boolean if a field has been set.

### SetCommitsDisplayNil

`func (o *GitHubRepositoryIdentity) SetCommitsDisplayNil(b bool)`

 SetCommitsDisplayNil sets the value for CommitsDisplay to be an explicit nil

### UnsetCommitsDisplay
`func (o *GitHubRepositoryIdentity) UnsetCommitsDisplay()`

UnsetCommitsDisplay ensures that no value is present for CommitsDisplay, not even an explicit nil
### GetCommitsCountApproximate

`func (o *GitHubRepositoryIdentity) GetCommitsCountApproximate() bool`

GetCommitsCountApproximate returns the CommitsCountApproximate field if non-nil, zero value otherwise.

### GetCommitsCountApproximateOk

`func (o *GitHubRepositoryIdentity) GetCommitsCountApproximateOk() (*bool, bool)`

GetCommitsCountApproximateOk returns a tuple with the CommitsCountApproximate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommitsCountApproximate

`func (o *GitHubRepositoryIdentity) SetCommitsCountApproximate(v bool)`

SetCommitsCountApproximate sets CommitsCountApproximate field to given value.

### HasCommitsCountApproximate

`func (o *GitHubRepositoryIdentity) HasCommitsCountApproximate() bool`

HasCommitsCountApproximate returns a boolean if a field has been set.

### SetCommitsCountApproximateNil

`func (o *GitHubRepositoryIdentity) SetCommitsCountApproximateNil(b bool)`

 SetCommitsCountApproximateNil sets the value for CommitsCountApproximate to be an explicit nil

### UnsetCommitsCountApproximate
`func (o *GitHubRepositoryIdentity) UnsetCommitsCountApproximate()`

UnsetCommitsCountApproximate ensures that no value is present for CommitsCountApproximate, not even an explicit nil
### GetBranchesCount

`func (o *GitHubRepositoryIdentity) GetBranchesCount() int32`

GetBranchesCount returns the BranchesCount field if non-nil, zero value otherwise.

### GetBranchesCountOk

`func (o *GitHubRepositoryIdentity) GetBranchesCountOk() (*int32, bool)`

GetBranchesCountOk returns a tuple with the BranchesCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBranchesCount

`func (o *GitHubRepositoryIdentity) SetBranchesCount(v int32)`

SetBranchesCount sets BranchesCount field to given value.

### HasBranchesCount

`func (o *GitHubRepositoryIdentity) HasBranchesCount() bool`

HasBranchesCount returns a boolean if a field has been set.

### SetBranchesCountNil

`func (o *GitHubRepositoryIdentity) SetBranchesCountNil(b bool)`

 SetBranchesCountNil sets the value for BranchesCount to be an explicit nil

### UnsetBranchesCount
`func (o *GitHubRepositoryIdentity) UnsetBranchesCount()`

UnsetBranchesCount ensures that no value is present for BranchesCount, not even an explicit nil
### GetBranchesCountApproximate

`func (o *GitHubRepositoryIdentity) GetBranchesCountApproximate() bool`

GetBranchesCountApproximate returns the BranchesCountApproximate field if non-nil, zero value otherwise.

### GetBranchesCountApproximateOk

`func (o *GitHubRepositoryIdentity) GetBranchesCountApproximateOk() (*bool, bool)`

GetBranchesCountApproximateOk returns a tuple with the BranchesCountApproximate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBranchesCountApproximate

`func (o *GitHubRepositoryIdentity) SetBranchesCountApproximate(v bool)`

SetBranchesCountApproximate sets BranchesCountApproximate field to given value.

### HasBranchesCountApproximate

`func (o *GitHubRepositoryIdentity) HasBranchesCountApproximate() bool`

HasBranchesCountApproximate returns a boolean if a field has been set.

### SetBranchesCountApproximateNil

`func (o *GitHubRepositoryIdentity) SetBranchesCountApproximateNil(b bool)`

 SetBranchesCountApproximateNil sets the value for BranchesCountApproximate to be an explicit nil

### UnsetBranchesCountApproximate
`func (o *GitHubRepositoryIdentity) UnsetBranchesCountApproximate()`

UnsetBranchesCountApproximate ensures that no value is present for BranchesCountApproximate, not even an explicit nil
### GetTagsCount

`func (o *GitHubRepositoryIdentity) GetTagsCount() int32`

GetTagsCount returns the TagsCount field if non-nil, zero value otherwise.

### GetTagsCountOk

`func (o *GitHubRepositoryIdentity) GetTagsCountOk() (*int32, bool)`

GetTagsCountOk returns a tuple with the TagsCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagsCount

`func (o *GitHubRepositoryIdentity) SetTagsCount(v int32)`

SetTagsCount sets TagsCount field to given value.

### HasTagsCount

`func (o *GitHubRepositoryIdentity) HasTagsCount() bool`

HasTagsCount returns a boolean if a field has been set.

### SetTagsCountNil

`func (o *GitHubRepositoryIdentity) SetTagsCountNil(b bool)`

 SetTagsCountNil sets the value for TagsCount to be an explicit nil

### UnsetTagsCount
`func (o *GitHubRepositoryIdentity) UnsetTagsCount()`

UnsetTagsCount ensures that no value is present for TagsCount, not even an explicit nil
### GetReleasesCount

`func (o *GitHubRepositoryIdentity) GetReleasesCount() int32`

GetReleasesCount returns the ReleasesCount field if non-nil, zero value otherwise.

### GetReleasesCountOk

`func (o *GitHubRepositoryIdentity) GetReleasesCountOk() (*int32, bool)`

GetReleasesCountOk returns a tuple with the ReleasesCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReleasesCount

`func (o *GitHubRepositoryIdentity) SetReleasesCount(v int32)`

SetReleasesCount sets ReleasesCount field to given value.

### HasReleasesCount

`func (o *GitHubRepositoryIdentity) HasReleasesCount() bool`

HasReleasesCount returns a boolean if a field has been set.

### SetReleasesCountNil

`func (o *GitHubRepositoryIdentity) SetReleasesCountNil(b bool)`

 SetReleasesCountNil sets the value for ReleasesCount to be an explicit nil

### UnsetReleasesCount
`func (o *GitHubRepositoryIdentity) UnsetReleasesCount()`

UnsetReleasesCount ensures that no value is present for ReleasesCount, not even an explicit nil
### GetContributorsCount

`func (o *GitHubRepositoryIdentity) GetContributorsCount() int32`

GetContributorsCount returns the ContributorsCount field if non-nil, zero value otherwise.

### GetContributorsCountOk

`func (o *GitHubRepositoryIdentity) GetContributorsCountOk() (*int32, bool)`

GetContributorsCountOk returns a tuple with the ContributorsCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContributorsCount

`func (o *GitHubRepositoryIdentity) SetContributorsCount(v int32)`

SetContributorsCount sets ContributorsCount field to given value.

### HasContributorsCount

`func (o *GitHubRepositoryIdentity) HasContributorsCount() bool`

HasContributorsCount returns a boolean if a field has been set.

### SetContributorsCountNil

`func (o *GitHubRepositoryIdentity) SetContributorsCountNil(b bool)`

 SetContributorsCountNil sets the value for ContributorsCount to be an explicit nil

### UnsetContributorsCount
`func (o *GitHubRepositoryIdentity) UnsetContributorsCount()`

UnsetContributorsCount ensures that no value is present for ContributorsCount, not even an explicit nil
### GetContributorsCountApproximate

`func (o *GitHubRepositoryIdentity) GetContributorsCountApproximate() bool`

GetContributorsCountApproximate returns the ContributorsCountApproximate field if non-nil, zero value otherwise.

### GetContributorsCountApproximateOk

`func (o *GitHubRepositoryIdentity) GetContributorsCountApproximateOk() (*bool, bool)`

GetContributorsCountApproximateOk returns a tuple with the ContributorsCountApproximate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContributorsCountApproximate

`func (o *GitHubRepositoryIdentity) SetContributorsCountApproximate(v bool)`

SetContributorsCountApproximate sets ContributorsCountApproximate field to given value.

### HasContributorsCountApproximate

`func (o *GitHubRepositoryIdentity) HasContributorsCountApproximate() bool`

HasContributorsCountApproximate returns a boolean if a field has been set.

### SetContributorsCountApproximateNil

`func (o *GitHubRepositoryIdentity) SetContributorsCountApproximateNil(b bool)`

 SetContributorsCountApproximateNil sets the value for ContributorsCountApproximate to be an explicit nil

### UnsetContributorsCountApproximate
`func (o *GitHubRepositoryIdentity) UnsetContributorsCountApproximate()`

UnsetContributorsCountApproximate ensures that no value is present for ContributorsCountApproximate, not even an explicit nil
### GetUsedByCount

`func (o *GitHubRepositoryIdentity) GetUsedByCount() int32`

GetUsedByCount returns the UsedByCount field if non-nil, zero value otherwise.

### GetUsedByCountOk

`func (o *GitHubRepositoryIdentity) GetUsedByCountOk() (*int32, bool)`

GetUsedByCountOk returns a tuple with the UsedByCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsedByCount

`func (o *GitHubRepositoryIdentity) SetUsedByCount(v int32)`

SetUsedByCount sets UsedByCount field to given value.

### HasUsedByCount

`func (o *GitHubRepositoryIdentity) HasUsedByCount() bool`

HasUsedByCount returns a boolean if a field has been set.

### SetUsedByCountNil

`func (o *GitHubRepositoryIdentity) SetUsedByCountNil(b bool)`

 SetUsedByCountNil sets the value for UsedByCount to be an explicit nil

### UnsetUsedByCount
`func (o *GitHubRepositoryIdentity) UnsetUsedByCount()`

UnsetUsedByCount ensures that no value is present for UsedByCount, not even an explicit nil
### GetUsedByCountApproximate

`func (o *GitHubRepositoryIdentity) GetUsedByCountApproximate() bool`

GetUsedByCountApproximate returns the UsedByCountApproximate field if non-nil, zero value otherwise.

### GetUsedByCountApproximateOk

`func (o *GitHubRepositoryIdentity) GetUsedByCountApproximateOk() (*bool, bool)`

GetUsedByCountApproximateOk returns a tuple with the UsedByCountApproximate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsedByCountApproximate

`func (o *GitHubRepositoryIdentity) SetUsedByCountApproximate(v bool)`

SetUsedByCountApproximate sets UsedByCountApproximate field to given value.

### HasUsedByCountApproximate

`func (o *GitHubRepositoryIdentity) HasUsedByCountApproximate() bool`

HasUsedByCountApproximate returns a boolean if a field has been set.

### SetUsedByCountApproximateNil

`func (o *GitHubRepositoryIdentity) SetUsedByCountApproximateNil(b bool)`

 SetUsedByCountApproximateNil sets the value for UsedByCountApproximate to be an explicit nil

### UnsetUsedByCountApproximate
`func (o *GitHubRepositoryIdentity) UnsetUsedByCountApproximate()`

UnsetUsedByCountApproximate ensures that no value is present for UsedByCountApproximate, not even an explicit nil
### GetSecurityAdvisoriesCount

`func (o *GitHubRepositoryIdentity) GetSecurityAdvisoriesCount() int32`

GetSecurityAdvisoriesCount returns the SecurityAdvisoriesCount field if non-nil, zero value otherwise.

### GetSecurityAdvisoriesCountOk

`func (o *GitHubRepositoryIdentity) GetSecurityAdvisoriesCountOk() (*int32, bool)`

GetSecurityAdvisoriesCountOk returns a tuple with the SecurityAdvisoriesCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecurityAdvisoriesCount

`func (o *GitHubRepositoryIdentity) SetSecurityAdvisoriesCount(v int32)`

SetSecurityAdvisoriesCount sets SecurityAdvisoriesCount field to given value.

### HasSecurityAdvisoriesCount

`func (o *GitHubRepositoryIdentity) HasSecurityAdvisoriesCount() bool`

HasSecurityAdvisoriesCount returns a boolean if a field has been set.

### SetSecurityAdvisoriesCountNil

`func (o *GitHubRepositoryIdentity) SetSecurityAdvisoriesCountNil(b bool)`

 SetSecurityAdvisoriesCountNil sets the value for SecurityAdvisoriesCount to be an explicit nil

### UnsetSecurityAdvisoriesCount
`func (o *GitHubRepositoryIdentity) UnsetSecurityAdvisoriesCount()`

UnsetSecurityAdvisoriesCount ensures that no value is present for SecurityAdvisoriesCount, not even an explicit nil
### GetFilesCount

`func (o *GitHubRepositoryIdentity) GetFilesCount() int32`

GetFilesCount returns the FilesCount field if non-nil, zero value otherwise.

### GetFilesCountOk

`func (o *GitHubRepositoryIdentity) GetFilesCountOk() (*int32, bool)`

GetFilesCountOk returns a tuple with the FilesCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilesCount

`func (o *GitHubRepositoryIdentity) SetFilesCount(v int32)`

SetFilesCount sets FilesCount field to given value.

### HasFilesCount

`func (o *GitHubRepositoryIdentity) HasFilesCount() bool`

HasFilesCount returns a boolean if a field has been set.

### SetFilesCountNil

`func (o *GitHubRepositoryIdentity) SetFilesCountNil(b bool)`

 SetFilesCountNil sets the value for FilesCount to be an explicit nil

### UnsetFilesCount
`func (o *GitHubRepositoryIdentity) UnsetFilesCount()`

UnsetFilesCount ensures that no value is present for FilesCount, not even an explicit nil
### GetFilesTruncated

`func (o *GitHubRepositoryIdentity) GetFilesTruncated() bool`

GetFilesTruncated returns the FilesTruncated field if non-nil, zero value otherwise.

### GetFilesTruncatedOk

`func (o *GitHubRepositoryIdentity) GetFilesTruncatedOk() (*bool, bool)`

GetFilesTruncatedOk returns a tuple with the FilesTruncated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilesTruncated

`func (o *GitHubRepositoryIdentity) SetFilesTruncated(v bool)`

SetFilesTruncated sets FilesTruncated field to given value.

### HasFilesTruncated

`func (o *GitHubRepositoryIdentity) HasFilesTruncated() bool`

HasFilesTruncated returns a boolean if a field has been set.

### SetFilesTruncatedNil

`func (o *GitHubRepositoryIdentity) SetFilesTruncatedNil(b bool)`

 SetFilesTruncatedNil sets the value for FilesTruncated to be an explicit nil

### UnsetFilesTruncated
`func (o *GitHubRepositoryIdentity) UnsetFilesTruncated()`

UnsetFilesTruncated ensures that no value is present for FilesTruncated, not even an explicit nil
### GetHasIssues

`func (o *GitHubRepositoryIdentity) GetHasIssues() bool`

GetHasIssues returns the HasIssues field if non-nil, zero value otherwise.

### GetHasIssuesOk

`func (o *GitHubRepositoryIdentity) GetHasIssuesOk() (*bool, bool)`

GetHasIssuesOk returns a tuple with the HasIssues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasIssues

`func (o *GitHubRepositoryIdentity) SetHasIssues(v bool)`

SetHasIssues sets HasIssues field to given value.

### HasHasIssues

`func (o *GitHubRepositoryIdentity) HasHasIssues() bool`

HasHasIssues returns a boolean if a field has been set.

### SetHasIssuesNil

`func (o *GitHubRepositoryIdentity) SetHasIssuesNil(b bool)`

 SetHasIssuesNil sets the value for HasIssues to be an explicit nil

### UnsetHasIssues
`func (o *GitHubRepositoryIdentity) UnsetHasIssues()`

UnsetHasIssues ensures that no value is present for HasIssues, not even an explicit nil
### GetHasPullRequests

`func (o *GitHubRepositoryIdentity) GetHasPullRequests() bool`

GetHasPullRequests returns the HasPullRequests field if non-nil, zero value otherwise.

### GetHasPullRequestsOk

`func (o *GitHubRepositoryIdentity) GetHasPullRequestsOk() (*bool, bool)`

GetHasPullRequestsOk returns a tuple with the HasPullRequests field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasPullRequests

`func (o *GitHubRepositoryIdentity) SetHasPullRequests(v bool)`

SetHasPullRequests sets HasPullRequests field to given value.

### HasHasPullRequests

`func (o *GitHubRepositoryIdentity) HasHasPullRequests() bool`

HasHasPullRequests returns a boolean if a field has been set.

### SetHasPullRequestsNil

`func (o *GitHubRepositoryIdentity) SetHasPullRequestsNil(b bool)`

 SetHasPullRequestsNil sets the value for HasPullRequests to be an explicit nil

### UnsetHasPullRequests
`func (o *GitHubRepositoryIdentity) UnsetHasPullRequests()`

UnsetHasPullRequests ensures that no value is present for HasPullRequests, not even an explicit nil
### GetHasDiscussions

`func (o *GitHubRepositoryIdentity) GetHasDiscussions() bool`

GetHasDiscussions returns the HasDiscussions field if non-nil, zero value otherwise.

### GetHasDiscussionsOk

`func (o *GitHubRepositoryIdentity) GetHasDiscussionsOk() (*bool, bool)`

GetHasDiscussionsOk returns a tuple with the HasDiscussions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasDiscussions

`func (o *GitHubRepositoryIdentity) SetHasDiscussions(v bool)`

SetHasDiscussions sets HasDiscussions field to given value.

### HasHasDiscussions

`func (o *GitHubRepositoryIdentity) HasHasDiscussions() bool`

HasHasDiscussions returns a boolean if a field has been set.

### SetHasDiscussionsNil

`func (o *GitHubRepositoryIdentity) SetHasDiscussionsNil(b bool)`

 SetHasDiscussionsNil sets the value for HasDiscussions to be an explicit nil

### UnsetHasDiscussions
`func (o *GitHubRepositoryIdentity) UnsetHasDiscussions()`

UnsetHasDiscussions ensures that no value is present for HasDiscussions, not even an explicit nil
### GetHasProjects

`func (o *GitHubRepositoryIdentity) GetHasProjects() bool`

GetHasProjects returns the HasProjects field if non-nil, zero value otherwise.

### GetHasProjectsOk

`func (o *GitHubRepositoryIdentity) GetHasProjectsOk() (*bool, bool)`

GetHasProjectsOk returns a tuple with the HasProjects field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasProjects

`func (o *GitHubRepositoryIdentity) SetHasProjects(v bool)`

SetHasProjects sets HasProjects field to given value.

### HasHasProjects

`func (o *GitHubRepositoryIdentity) HasHasProjects() bool`

HasHasProjects returns a boolean if a field has been set.

### SetHasProjectsNil

`func (o *GitHubRepositoryIdentity) SetHasProjectsNil(b bool)`

 SetHasProjectsNil sets the value for HasProjects to be an explicit nil

### UnsetHasProjects
`func (o *GitHubRepositoryIdentity) UnsetHasProjects()`

UnsetHasProjects ensures that no value is present for HasProjects, not even an explicit nil
### GetHasWiki

`func (o *GitHubRepositoryIdentity) GetHasWiki() bool`

GetHasWiki returns the HasWiki field if non-nil, zero value otherwise.

### GetHasWikiOk

`func (o *GitHubRepositoryIdentity) GetHasWikiOk() (*bool, bool)`

GetHasWikiOk returns a tuple with the HasWiki field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasWiki

`func (o *GitHubRepositoryIdentity) SetHasWiki(v bool)`

SetHasWiki sets HasWiki field to given value.

### HasHasWiki

`func (o *GitHubRepositoryIdentity) HasHasWiki() bool`

HasHasWiki returns a boolean if a field has been set.

### SetHasWikiNil

`func (o *GitHubRepositoryIdentity) SetHasWikiNil(b bool)`

 SetHasWikiNil sets the value for HasWiki to be an explicit nil

### UnsetHasWiki
`func (o *GitHubRepositoryIdentity) UnsetHasWiki()`

UnsetHasWiki ensures that no value is present for HasWiki, not even an explicit nil
### GetHasPages

`func (o *GitHubRepositoryIdentity) GetHasPages() bool`

GetHasPages returns the HasPages field if non-nil, zero value otherwise.

### GetHasPagesOk

`func (o *GitHubRepositoryIdentity) GetHasPagesOk() (*bool, bool)`

GetHasPagesOk returns a tuple with the HasPages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasPages

`func (o *GitHubRepositoryIdentity) SetHasPages(v bool)`

SetHasPages sets HasPages field to given value.

### HasHasPages

`func (o *GitHubRepositoryIdentity) HasHasPages() bool`

HasHasPages returns a boolean if a field has been set.

### SetHasPagesNil

`func (o *GitHubRepositoryIdentity) SetHasPagesNil(b bool)`

 SetHasPagesNil sets the value for HasPages to be an explicit nil

### UnsetHasPages
`func (o *GitHubRepositoryIdentity) UnsetHasPages()`

UnsetHasPages ensures that no value is present for HasPages, not even an explicit nil
### GetHasDownloads

`func (o *GitHubRepositoryIdentity) GetHasDownloads() bool`

GetHasDownloads returns the HasDownloads field if non-nil, zero value otherwise.

### GetHasDownloadsOk

`func (o *GitHubRepositoryIdentity) GetHasDownloadsOk() (*bool, bool)`

GetHasDownloadsOk returns a tuple with the HasDownloads field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasDownloads

`func (o *GitHubRepositoryIdentity) SetHasDownloads(v bool)`

SetHasDownloads sets HasDownloads field to given value.

### HasHasDownloads

`func (o *GitHubRepositoryIdentity) HasHasDownloads() bool`

HasHasDownloads returns a boolean if a field has been set.

### SetHasDownloadsNil

`func (o *GitHubRepositoryIdentity) SetHasDownloadsNil(b bool)`

 SetHasDownloadsNil sets the value for HasDownloads to be an explicit nil

### UnsetHasDownloads
`func (o *GitHubRepositoryIdentity) UnsetHasDownloads()`

UnsetHasDownloads ensures that no value is present for HasDownloads, not even an explicit nil
### GetHasCitation

`func (o *GitHubRepositoryIdentity) GetHasCitation() bool`

GetHasCitation returns the HasCitation field if non-nil, zero value otherwise.

### GetHasCitationOk

`func (o *GitHubRepositoryIdentity) GetHasCitationOk() (*bool, bool)`

GetHasCitationOk returns a tuple with the HasCitation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasCitation

`func (o *GitHubRepositoryIdentity) SetHasCitation(v bool)`

SetHasCitation sets HasCitation field to given value.

### HasHasCitation

`func (o *GitHubRepositoryIdentity) HasHasCitation() bool`

HasHasCitation returns a boolean if a field has been set.

### SetHasCitationNil

`func (o *GitHubRepositoryIdentity) SetHasCitationNil(b bool)`

 SetHasCitationNil sets the value for HasCitation to be an explicit nil

### UnsetHasCitation
`func (o *GitHubRepositoryIdentity) UnsetHasCitation()`

UnsetHasCitation ensures that no value is present for HasCitation, not even an explicit nil
### GetHasCodeOfConduct

`func (o *GitHubRepositoryIdentity) GetHasCodeOfConduct() bool`

GetHasCodeOfConduct returns the HasCodeOfConduct field if non-nil, zero value otherwise.

### GetHasCodeOfConductOk

`func (o *GitHubRepositoryIdentity) GetHasCodeOfConductOk() (*bool, bool)`

GetHasCodeOfConductOk returns a tuple with the HasCodeOfConduct field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasCodeOfConduct

`func (o *GitHubRepositoryIdentity) SetHasCodeOfConduct(v bool)`

SetHasCodeOfConduct sets HasCodeOfConduct field to given value.

### HasHasCodeOfConduct

`func (o *GitHubRepositoryIdentity) HasHasCodeOfConduct() bool`

HasHasCodeOfConduct returns a boolean if a field has been set.

### SetHasCodeOfConductNil

`func (o *GitHubRepositoryIdentity) SetHasCodeOfConductNil(b bool)`

 SetHasCodeOfConductNil sets the value for HasCodeOfConduct to be an explicit nil

### UnsetHasCodeOfConduct
`func (o *GitHubRepositoryIdentity) UnsetHasCodeOfConduct()`

UnsetHasCodeOfConduct ensures that no value is present for HasCodeOfConduct, not even an explicit nil
### GetHasContributingGuide

`func (o *GitHubRepositoryIdentity) GetHasContributingGuide() bool`

GetHasContributingGuide returns the HasContributingGuide field if non-nil, zero value otherwise.

### GetHasContributingGuideOk

`func (o *GitHubRepositoryIdentity) GetHasContributingGuideOk() (*bool, bool)`

GetHasContributingGuideOk returns a tuple with the HasContributingGuide field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasContributingGuide

`func (o *GitHubRepositoryIdentity) SetHasContributingGuide(v bool)`

SetHasContributingGuide sets HasContributingGuide field to given value.

### HasHasContributingGuide

`func (o *GitHubRepositoryIdentity) HasHasContributingGuide() bool`

HasHasContributingGuide returns a boolean if a field has been set.

### SetHasContributingGuideNil

`func (o *GitHubRepositoryIdentity) SetHasContributingGuideNil(b bool)`

 SetHasContributingGuideNil sets the value for HasContributingGuide to be an explicit nil

### UnsetHasContributingGuide
`func (o *GitHubRepositoryIdentity) UnsetHasContributingGuide()`

UnsetHasContributingGuide ensures that no value is present for HasContributingGuide, not even an explicit nil
### GetHasSecurityPolicy

`func (o *GitHubRepositoryIdentity) GetHasSecurityPolicy() bool`

GetHasSecurityPolicy returns the HasSecurityPolicy field if non-nil, zero value otherwise.

### GetHasSecurityPolicyOk

`func (o *GitHubRepositoryIdentity) GetHasSecurityPolicyOk() (*bool, bool)`

GetHasSecurityPolicyOk returns a tuple with the HasSecurityPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasSecurityPolicy

`func (o *GitHubRepositoryIdentity) SetHasSecurityPolicy(v bool)`

SetHasSecurityPolicy sets HasSecurityPolicy field to given value.

### HasHasSecurityPolicy

`func (o *GitHubRepositoryIdentity) HasHasSecurityPolicy() bool`

HasHasSecurityPolicy returns a boolean if a field has been set.

### SetHasSecurityPolicyNil

`func (o *GitHubRepositoryIdentity) SetHasSecurityPolicyNil(b bool)`

 SetHasSecurityPolicyNil sets the value for HasSecurityPolicy to be an explicit nil

### UnsetHasSecurityPolicy
`func (o *GitHubRepositoryIdentity) UnsetHasSecurityPolicy()`

UnsetHasSecurityPolicy ensures that no value is present for HasSecurityPolicy, not even an explicit nil
### GetAllowForking

`func (o *GitHubRepositoryIdentity) GetAllowForking() bool`

GetAllowForking returns the AllowForking field if non-nil, zero value otherwise.

### GetAllowForkingOk

`func (o *GitHubRepositoryIdentity) GetAllowForkingOk() (*bool, bool)`

GetAllowForkingOk returns a tuple with the AllowForking field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllowForking

`func (o *GitHubRepositoryIdentity) SetAllowForking(v bool)`

SetAllowForking sets AllowForking field to given value.

### HasAllowForking

`func (o *GitHubRepositoryIdentity) HasAllowForking() bool`

HasAllowForking returns a boolean if a field has been set.

### SetAllowForkingNil

`func (o *GitHubRepositoryIdentity) SetAllowForkingNil(b bool)`

 SetAllowForkingNil sets the value for AllowForking to be an explicit nil

### UnsetAllowForking
`func (o *GitHubRepositoryIdentity) UnsetAllowForking()`

UnsetAllowForking ensures that no value is present for AllowForking, not even an explicit nil
### GetWebCommitSignoffRequired

`func (o *GitHubRepositoryIdentity) GetWebCommitSignoffRequired() bool`

GetWebCommitSignoffRequired returns the WebCommitSignoffRequired field if non-nil, zero value otherwise.

### GetWebCommitSignoffRequiredOk

`func (o *GitHubRepositoryIdentity) GetWebCommitSignoffRequiredOk() (*bool, bool)`

GetWebCommitSignoffRequiredOk returns a tuple with the WebCommitSignoffRequired field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebCommitSignoffRequired

`func (o *GitHubRepositoryIdentity) SetWebCommitSignoffRequired(v bool)`

SetWebCommitSignoffRequired sets WebCommitSignoffRequired field to given value.

### HasWebCommitSignoffRequired

`func (o *GitHubRepositoryIdentity) HasWebCommitSignoffRequired() bool`

HasWebCommitSignoffRequired returns a boolean if a field has been set.

### SetWebCommitSignoffRequiredNil

`func (o *GitHubRepositoryIdentity) SetWebCommitSignoffRequiredNil(b bool)`

 SetWebCommitSignoffRequiredNil sets the value for WebCommitSignoffRequired to be an explicit nil

### UnsetWebCommitSignoffRequired
`func (o *GitHubRepositoryIdentity) UnsetWebCommitSignoffRequired()`

UnsetWebCommitSignoffRequired ensures that no value is present for WebCommitSignoffRequired, not even an explicit nil
### GetPullRequestCreationPolicy

`func (o *GitHubRepositoryIdentity) GetPullRequestCreationPolicy() string`

GetPullRequestCreationPolicy returns the PullRequestCreationPolicy field if non-nil, zero value otherwise.

### GetPullRequestCreationPolicyOk

`func (o *GitHubRepositoryIdentity) GetPullRequestCreationPolicyOk() (*string, bool)`

GetPullRequestCreationPolicyOk returns a tuple with the PullRequestCreationPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPullRequestCreationPolicy

`func (o *GitHubRepositoryIdentity) SetPullRequestCreationPolicy(v string)`

SetPullRequestCreationPolicy sets PullRequestCreationPolicy field to given value.

### HasPullRequestCreationPolicy

`func (o *GitHubRepositoryIdentity) HasPullRequestCreationPolicy() bool`

HasPullRequestCreationPolicy returns a boolean if a field has been set.

### SetPullRequestCreationPolicyNil

`func (o *GitHubRepositoryIdentity) SetPullRequestCreationPolicyNil(b bool)`

 SetPullRequestCreationPolicyNil sets the value for PullRequestCreationPolicy to be an explicit nil

### UnsetPullRequestCreationPolicy
`func (o *GitHubRepositoryIdentity) UnsetPullRequestCreationPolicy()`

UnsetPullRequestCreationPolicy ensures that no value is present for PullRequestCreationPolicy, not even an explicit nil
### GetSizeKb

`func (o *GitHubRepositoryIdentity) GetSizeKb() int32`

GetSizeKb returns the SizeKb field if non-nil, zero value otherwise.

### GetSizeKbOk

`func (o *GitHubRepositoryIdentity) GetSizeKbOk() (*int32, bool)`

GetSizeKbOk returns a tuple with the SizeKb field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSizeKb

`func (o *GitHubRepositoryIdentity) SetSizeKb(v int32)`

SetSizeKb sets SizeKb field to given value.

### HasSizeKb

`func (o *GitHubRepositoryIdentity) HasSizeKb() bool`

HasSizeKb returns a boolean if a field has been set.

### SetSizeKbNil

`func (o *GitHubRepositoryIdentity) SetSizeKbNil(b bool)`

 SetSizeKbNil sets the value for SizeKb to be an explicit nil

### UnsetSizeKb
`func (o *GitHubRepositoryIdentity) UnsetSizeKb()`

UnsetSizeKb ensures that no value is present for SizeKb, not even an explicit nil
### GetCloneUrl

`func (o *GitHubRepositoryIdentity) GetCloneUrl() string`

GetCloneUrl returns the CloneUrl field if non-nil, zero value otherwise.

### GetCloneUrlOk

`func (o *GitHubRepositoryIdentity) GetCloneUrlOk() (*string, bool)`

GetCloneUrlOk returns a tuple with the CloneUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCloneUrl

`func (o *GitHubRepositoryIdentity) SetCloneUrl(v string)`

SetCloneUrl sets CloneUrl field to given value.

### HasCloneUrl

`func (o *GitHubRepositoryIdentity) HasCloneUrl() bool`

HasCloneUrl returns a boolean if a field has been set.

### SetCloneUrlNil

`func (o *GitHubRepositoryIdentity) SetCloneUrlNil(b bool)`

 SetCloneUrlNil sets the value for CloneUrl to be an explicit nil

### UnsetCloneUrl
`func (o *GitHubRepositoryIdentity) UnsetCloneUrl()`

UnsetCloneUrl ensures that no value is present for CloneUrl, not even an explicit nil
### GetSshUrl

`func (o *GitHubRepositoryIdentity) GetSshUrl() string`

GetSshUrl returns the SshUrl field if non-nil, zero value otherwise.

### GetSshUrlOk

`func (o *GitHubRepositoryIdentity) GetSshUrlOk() (*string, bool)`

GetSshUrlOk returns a tuple with the SshUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSshUrl

`func (o *GitHubRepositoryIdentity) SetSshUrl(v string)`

SetSshUrl sets SshUrl field to given value.

### HasSshUrl

`func (o *GitHubRepositoryIdentity) HasSshUrl() bool`

HasSshUrl returns a boolean if a field has been set.

### SetSshUrlNil

`func (o *GitHubRepositoryIdentity) SetSshUrlNil(b bool)`

 SetSshUrlNil sets the value for SshUrl to be an explicit nil

### UnsetSshUrl
`func (o *GitHubRepositoryIdentity) UnsetSshUrl()`

UnsetSshUrl ensures that no value is present for SshUrl, not even an explicit nil
### GetGitUrl

`func (o *GitHubRepositoryIdentity) GetGitUrl() string`

GetGitUrl returns the GitUrl field if non-nil, zero value otherwise.

### GetGitUrlOk

`func (o *GitHubRepositoryIdentity) GetGitUrlOk() (*string, bool)`

GetGitUrlOk returns a tuple with the GitUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGitUrl

`func (o *GitHubRepositoryIdentity) SetGitUrl(v string)`

SetGitUrl sets GitUrl field to given value.

### HasGitUrl

`func (o *GitHubRepositoryIdentity) HasGitUrl() bool`

HasGitUrl returns a boolean if a field has been set.

### SetGitUrlNil

`func (o *GitHubRepositoryIdentity) SetGitUrlNil(b bool)`

 SetGitUrlNil sets the value for GitUrl to be an explicit nil

### UnsetGitUrl
`func (o *GitHubRepositoryIdentity) UnsetGitUrl()`

UnsetGitUrl ensures that no value is present for GitUrl, not even an explicit nil
### GetSvnUrl

`func (o *GitHubRepositoryIdentity) GetSvnUrl() string`

GetSvnUrl returns the SvnUrl field if non-nil, zero value otherwise.

### GetSvnUrlOk

`func (o *GitHubRepositoryIdentity) GetSvnUrlOk() (*string, bool)`

GetSvnUrlOk returns a tuple with the SvnUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSvnUrl

`func (o *GitHubRepositoryIdentity) SetSvnUrl(v string)`

SetSvnUrl sets SvnUrl field to given value.

### HasSvnUrl

`func (o *GitHubRepositoryIdentity) HasSvnUrl() bool`

HasSvnUrl returns a boolean if a field has been set.

### SetSvnUrlNil

`func (o *GitHubRepositoryIdentity) SetSvnUrlNil(b bool)`

 SetSvnUrlNil sets the value for SvnUrl to be an explicit nil

### UnsetSvnUrl
`func (o *GitHubRepositoryIdentity) UnsetSvnUrl()`

UnsetSvnUrl ensures that no value is present for SvnUrl, not even an explicit nil
### GetArchiveUrl

`func (o *GitHubRepositoryIdentity) GetArchiveUrl() string`

GetArchiveUrl returns the ArchiveUrl field if non-nil, zero value otherwise.

### GetArchiveUrlOk

`func (o *GitHubRepositoryIdentity) GetArchiveUrlOk() (*string, bool)`

GetArchiveUrlOk returns a tuple with the ArchiveUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchiveUrl

`func (o *GitHubRepositoryIdentity) SetArchiveUrl(v string)`

SetArchiveUrl sets ArchiveUrl field to given value.

### HasArchiveUrl

`func (o *GitHubRepositoryIdentity) HasArchiveUrl() bool`

HasArchiveUrl returns a boolean if a field has been set.

### SetArchiveUrlNil

`func (o *GitHubRepositoryIdentity) SetArchiveUrlNil(b bool)`

 SetArchiveUrlNil sets the value for ArchiveUrl to be an explicit nil

### UnsetArchiveUrl
`func (o *GitHubRepositoryIdentity) UnsetArchiveUrl()`

UnsetArchiveUrl ensures that no value is present for ArchiveUrl, not even an explicit nil
### GetMirrorUrl

`func (o *GitHubRepositoryIdentity) GetMirrorUrl() string`

GetMirrorUrl returns the MirrorUrl field if non-nil, zero value otherwise.

### GetMirrorUrlOk

`func (o *GitHubRepositoryIdentity) GetMirrorUrlOk() (*string, bool)`

GetMirrorUrlOk returns a tuple with the MirrorUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMirrorUrl

`func (o *GitHubRepositoryIdentity) SetMirrorUrl(v string)`

SetMirrorUrl sets MirrorUrl field to given value.

### HasMirrorUrl

`func (o *GitHubRepositoryIdentity) HasMirrorUrl() bool`

HasMirrorUrl returns a boolean if a field has been set.

### SetMirrorUrlNil

`func (o *GitHubRepositoryIdentity) SetMirrorUrlNil(b bool)`

 SetMirrorUrlNil sets the value for MirrorUrl to be an explicit nil

### UnsetMirrorUrl
`func (o *GitHubRepositoryIdentity) UnsetMirrorUrl()`

UnsetMirrorUrl ensures that no value is present for MirrorUrl, not even an explicit nil
### GetCreatedAt

`func (o *GitHubRepositoryIdentity) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *GitHubRepositoryIdentity) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *GitHubRepositoryIdentity) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *GitHubRepositoryIdentity) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### SetCreatedAtNil

`func (o *GitHubRepositoryIdentity) SetCreatedAtNil(b bool)`

 SetCreatedAtNil sets the value for CreatedAt to be an explicit nil

### UnsetCreatedAt
`func (o *GitHubRepositoryIdentity) UnsetCreatedAt()`

UnsetCreatedAt ensures that no value is present for CreatedAt, not even an explicit nil
### GetCreatedUtc

`func (o *GitHubRepositoryIdentity) GetCreatedUtc() float32`

GetCreatedUtc returns the CreatedUtc field if non-nil, zero value otherwise.

### GetCreatedUtcOk

`func (o *GitHubRepositoryIdentity) GetCreatedUtcOk() (*float32, bool)`

GetCreatedUtcOk returns a tuple with the CreatedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedUtc

`func (o *GitHubRepositoryIdentity) SetCreatedUtc(v float32)`

SetCreatedUtc sets CreatedUtc field to given value.

### HasCreatedUtc

`func (o *GitHubRepositoryIdentity) HasCreatedUtc() bool`

HasCreatedUtc returns a boolean if a field has been set.

### SetCreatedUtcNil

`func (o *GitHubRepositoryIdentity) SetCreatedUtcNil(b bool)`

 SetCreatedUtcNil sets the value for CreatedUtc to be an explicit nil

### UnsetCreatedUtc
`func (o *GitHubRepositoryIdentity) UnsetCreatedUtc()`

UnsetCreatedUtc ensures that no value is present for CreatedUtc, not even an explicit nil
### GetUpdatedAt

`func (o *GitHubRepositoryIdentity) GetUpdatedAt() string`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *GitHubRepositoryIdentity) GetUpdatedAtOk() (*string, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *GitHubRepositoryIdentity) SetUpdatedAt(v string)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *GitHubRepositoryIdentity) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.

### SetUpdatedAtNil

`func (o *GitHubRepositoryIdentity) SetUpdatedAtNil(b bool)`

 SetUpdatedAtNil sets the value for UpdatedAt to be an explicit nil

### UnsetUpdatedAt
`func (o *GitHubRepositoryIdentity) UnsetUpdatedAt()`

UnsetUpdatedAt ensures that no value is present for UpdatedAt, not even an explicit nil
### GetUpdatedUtc

`func (o *GitHubRepositoryIdentity) GetUpdatedUtc() float32`

GetUpdatedUtc returns the UpdatedUtc field if non-nil, zero value otherwise.

### GetUpdatedUtcOk

`func (o *GitHubRepositoryIdentity) GetUpdatedUtcOk() (*float32, bool)`

GetUpdatedUtcOk returns a tuple with the UpdatedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedUtc

`func (o *GitHubRepositoryIdentity) SetUpdatedUtc(v float32)`

SetUpdatedUtc sets UpdatedUtc field to given value.

### HasUpdatedUtc

`func (o *GitHubRepositoryIdentity) HasUpdatedUtc() bool`

HasUpdatedUtc returns a boolean if a field has been set.

### SetUpdatedUtcNil

`func (o *GitHubRepositoryIdentity) SetUpdatedUtcNil(b bool)`

 SetUpdatedUtcNil sets the value for UpdatedUtc to be an explicit nil

### UnsetUpdatedUtc
`func (o *GitHubRepositoryIdentity) UnsetUpdatedUtc()`

UnsetUpdatedUtc ensures that no value is present for UpdatedUtc, not even an explicit nil
### GetPushedAt

`func (o *GitHubRepositoryIdentity) GetPushedAt() string`

GetPushedAt returns the PushedAt field if non-nil, zero value otherwise.

### GetPushedAtOk

`func (o *GitHubRepositoryIdentity) GetPushedAtOk() (*string, bool)`

GetPushedAtOk returns a tuple with the PushedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPushedAt

`func (o *GitHubRepositoryIdentity) SetPushedAt(v string)`

SetPushedAt sets PushedAt field to given value.

### HasPushedAt

`func (o *GitHubRepositoryIdentity) HasPushedAt() bool`

HasPushedAt returns a boolean if a field has been set.

### SetPushedAtNil

`func (o *GitHubRepositoryIdentity) SetPushedAtNil(b bool)`

 SetPushedAtNil sets the value for PushedAt to be an explicit nil

### UnsetPushedAt
`func (o *GitHubRepositoryIdentity) UnsetPushedAt()`

UnsetPushedAt ensures that no value is present for PushedAt, not even an explicit nil
### GetPushedUtc

`func (o *GitHubRepositoryIdentity) GetPushedUtc() float32`

GetPushedUtc returns the PushedUtc field if non-nil, zero value otherwise.

### GetPushedUtcOk

`func (o *GitHubRepositoryIdentity) GetPushedUtcOk() (*float32, bool)`

GetPushedUtcOk returns a tuple with the PushedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPushedUtc

`func (o *GitHubRepositoryIdentity) SetPushedUtc(v float32)`

SetPushedUtc sets PushedUtc field to given value.

### HasPushedUtc

`func (o *GitHubRepositoryIdentity) HasPushedUtc() bool`

HasPushedUtc returns a boolean if a field has been set.

### SetPushedUtcNil

`func (o *GitHubRepositoryIdentity) SetPushedUtcNil(b bool)`

 SetPushedUtcNil sets the value for PushedUtc to be an explicit nil

### UnsetPushedUtc
`func (o *GitHubRepositoryIdentity) UnsetPushedUtc()`

UnsetPushedUtc ensures that no value is present for PushedUtc, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



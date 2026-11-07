# GitHubRepository

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Position** | **int32** |  | 
**Name** | **string** |  | 
**FullName** | **string** |  | 
**Owner** | [**GitHubAccountPreview**](GitHubAccountPreview.md) |  | 
**Link** | **string** |  | 
**Id** | Pointer to **NullableInt32** |  | [optional] 
**Description** | Pointer to **NullableString** |  | [optional] 
**Language** | Pointer to **NullableString** |  | [optional] 
**LanguageColor** | Pointer to **NullableString** |  | [optional] 
**Stars** | Pointer to **NullableInt32** |  | [optional] 
**Forks** | Pointer to **NullableInt32** |  | [optional] 
**Issues** | Pointer to **NullableInt32** |  | [optional] 
**PullRequests** | Pointer to **NullableInt32** |  | [optional] 
**StarsApproximate** | Pointer to **NullableBool** |  | [optional] 
**ForksApproximate** | Pointer to **NullableBool** |  | [optional] 
**IssuesApproximate** | Pointer to **NullableBool** |  | [optional] 
**PullRequestsApproximate** | Pointer to **NullableBool** |  | [optional] 
**Visibility** | Pointer to **NullableString** |  | [optional] 
**IsFork** | Pointer to **NullableBool** |  | [optional] 
**License** | Pointer to **NullableString** |  | [optional] 
**Topics** | Pointer to **[]string** |  | [optional] 
**Participation** | Pointer to **[]int32** |  | [optional] 
**UpdatedAt** | Pointer to **NullableString** |  | [optional] 
**UpdatedUtc** | Pointer to **NullableFloat32** |  | [optional] 

## Methods

### NewGitHubRepository

`func NewGitHubRepository(position int32, name string, fullName string, owner GitHubAccountPreview, link string, ) *GitHubRepository`

NewGitHubRepository instantiates a new GitHubRepository object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubRepositoryWithDefaults

`func NewGitHubRepositoryWithDefaults() *GitHubRepository`

NewGitHubRepositoryWithDefaults instantiates a new GitHubRepository object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPosition

`func (o *GitHubRepository) GetPosition() int32`

GetPosition returns the Position field if non-nil, zero value otherwise.

### GetPositionOk

`func (o *GitHubRepository) GetPositionOk() (*int32, bool)`

GetPositionOk returns a tuple with the Position field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPosition

`func (o *GitHubRepository) SetPosition(v int32)`

SetPosition sets Position field to given value.


### GetName

`func (o *GitHubRepository) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *GitHubRepository) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *GitHubRepository) SetName(v string)`

SetName sets Name field to given value.


### GetFullName

`func (o *GitHubRepository) GetFullName() string`

GetFullName returns the FullName field if non-nil, zero value otherwise.

### GetFullNameOk

`func (o *GitHubRepository) GetFullNameOk() (*string, bool)`

GetFullNameOk returns a tuple with the FullName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFullName

`func (o *GitHubRepository) SetFullName(v string)`

SetFullName sets FullName field to given value.


### GetOwner

`func (o *GitHubRepository) GetOwner() GitHubAccountPreview`

GetOwner returns the Owner field if non-nil, zero value otherwise.

### GetOwnerOk

`func (o *GitHubRepository) GetOwnerOk() (*GitHubAccountPreview, bool)`

GetOwnerOk returns a tuple with the Owner field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOwner

`func (o *GitHubRepository) SetOwner(v GitHubAccountPreview)`

SetOwner sets Owner field to given value.


### GetLink

`func (o *GitHubRepository) GetLink() string`

GetLink returns the Link field if non-nil, zero value otherwise.

### GetLinkOk

`func (o *GitHubRepository) GetLinkOk() (*string, bool)`

GetLinkOk returns a tuple with the Link field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLink

`func (o *GitHubRepository) SetLink(v string)`

SetLink sets Link field to given value.


### GetId

`func (o *GitHubRepository) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *GitHubRepository) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *GitHubRepository) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *GitHubRepository) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *GitHubRepository) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *GitHubRepository) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil
### GetDescription

`func (o *GitHubRepository) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *GitHubRepository) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *GitHubRepository) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *GitHubRepository) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *GitHubRepository) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *GitHubRepository) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetLanguage

`func (o *GitHubRepository) GetLanguage() string`

GetLanguage returns the Language field if non-nil, zero value otherwise.

### GetLanguageOk

`func (o *GitHubRepository) GetLanguageOk() (*string, bool)`

GetLanguageOk returns a tuple with the Language field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLanguage

`func (o *GitHubRepository) SetLanguage(v string)`

SetLanguage sets Language field to given value.

### HasLanguage

`func (o *GitHubRepository) HasLanguage() bool`

HasLanguage returns a boolean if a field has been set.

### SetLanguageNil

`func (o *GitHubRepository) SetLanguageNil(b bool)`

 SetLanguageNil sets the value for Language to be an explicit nil

### UnsetLanguage
`func (o *GitHubRepository) UnsetLanguage()`

UnsetLanguage ensures that no value is present for Language, not even an explicit nil
### GetLanguageColor

`func (o *GitHubRepository) GetLanguageColor() string`

GetLanguageColor returns the LanguageColor field if non-nil, zero value otherwise.

### GetLanguageColorOk

`func (o *GitHubRepository) GetLanguageColorOk() (*string, bool)`

GetLanguageColorOk returns a tuple with the LanguageColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLanguageColor

`func (o *GitHubRepository) SetLanguageColor(v string)`

SetLanguageColor sets LanguageColor field to given value.

### HasLanguageColor

`func (o *GitHubRepository) HasLanguageColor() bool`

HasLanguageColor returns a boolean if a field has been set.

### SetLanguageColorNil

`func (o *GitHubRepository) SetLanguageColorNil(b bool)`

 SetLanguageColorNil sets the value for LanguageColor to be an explicit nil

### UnsetLanguageColor
`func (o *GitHubRepository) UnsetLanguageColor()`

UnsetLanguageColor ensures that no value is present for LanguageColor, not even an explicit nil
### GetStars

`func (o *GitHubRepository) GetStars() int32`

GetStars returns the Stars field if non-nil, zero value otherwise.

### GetStarsOk

`func (o *GitHubRepository) GetStarsOk() (*int32, bool)`

GetStarsOk returns a tuple with the Stars field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStars

`func (o *GitHubRepository) SetStars(v int32)`

SetStars sets Stars field to given value.

### HasStars

`func (o *GitHubRepository) HasStars() bool`

HasStars returns a boolean if a field has been set.

### SetStarsNil

`func (o *GitHubRepository) SetStarsNil(b bool)`

 SetStarsNil sets the value for Stars to be an explicit nil

### UnsetStars
`func (o *GitHubRepository) UnsetStars()`

UnsetStars ensures that no value is present for Stars, not even an explicit nil
### GetForks

`func (o *GitHubRepository) GetForks() int32`

GetForks returns the Forks field if non-nil, zero value otherwise.

### GetForksOk

`func (o *GitHubRepository) GetForksOk() (*int32, bool)`

GetForksOk returns a tuple with the Forks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetForks

`func (o *GitHubRepository) SetForks(v int32)`

SetForks sets Forks field to given value.

### HasForks

`func (o *GitHubRepository) HasForks() bool`

HasForks returns a boolean if a field has been set.

### SetForksNil

`func (o *GitHubRepository) SetForksNil(b bool)`

 SetForksNil sets the value for Forks to be an explicit nil

### UnsetForks
`func (o *GitHubRepository) UnsetForks()`

UnsetForks ensures that no value is present for Forks, not even an explicit nil
### GetIssues

`func (o *GitHubRepository) GetIssues() int32`

GetIssues returns the Issues field if non-nil, zero value otherwise.

### GetIssuesOk

`func (o *GitHubRepository) GetIssuesOk() (*int32, bool)`

GetIssuesOk returns a tuple with the Issues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssues

`func (o *GitHubRepository) SetIssues(v int32)`

SetIssues sets Issues field to given value.

### HasIssues

`func (o *GitHubRepository) HasIssues() bool`

HasIssues returns a boolean if a field has been set.

### SetIssuesNil

`func (o *GitHubRepository) SetIssuesNil(b bool)`

 SetIssuesNil sets the value for Issues to be an explicit nil

### UnsetIssues
`func (o *GitHubRepository) UnsetIssues()`

UnsetIssues ensures that no value is present for Issues, not even an explicit nil
### GetPullRequests

`func (o *GitHubRepository) GetPullRequests() int32`

GetPullRequests returns the PullRequests field if non-nil, zero value otherwise.

### GetPullRequestsOk

`func (o *GitHubRepository) GetPullRequestsOk() (*int32, bool)`

GetPullRequestsOk returns a tuple with the PullRequests field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPullRequests

`func (o *GitHubRepository) SetPullRequests(v int32)`

SetPullRequests sets PullRequests field to given value.

### HasPullRequests

`func (o *GitHubRepository) HasPullRequests() bool`

HasPullRequests returns a boolean if a field has been set.

### SetPullRequestsNil

`func (o *GitHubRepository) SetPullRequestsNil(b bool)`

 SetPullRequestsNil sets the value for PullRequests to be an explicit nil

### UnsetPullRequests
`func (o *GitHubRepository) UnsetPullRequests()`

UnsetPullRequests ensures that no value is present for PullRequests, not even an explicit nil
### GetStarsApproximate

`func (o *GitHubRepository) GetStarsApproximate() bool`

GetStarsApproximate returns the StarsApproximate field if non-nil, zero value otherwise.

### GetStarsApproximateOk

`func (o *GitHubRepository) GetStarsApproximateOk() (*bool, bool)`

GetStarsApproximateOk returns a tuple with the StarsApproximate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStarsApproximate

`func (o *GitHubRepository) SetStarsApproximate(v bool)`

SetStarsApproximate sets StarsApproximate field to given value.

### HasStarsApproximate

`func (o *GitHubRepository) HasStarsApproximate() bool`

HasStarsApproximate returns a boolean if a field has been set.

### SetStarsApproximateNil

`func (o *GitHubRepository) SetStarsApproximateNil(b bool)`

 SetStarsApproximateNil sets the value for StarsApproximate to be an explicit nil

### UnsetStarsApproximate
`func (o *GitHubRepository) UnsetStarsApproximate()`

UnsetStarsApproximate ensures that no value is present for StarsApproximate, not even an explicit nil
### GetForksApproximate

`func (o *GitHubRepository) GetForksApproximate() bool`

GetForksApproximate returns the ForksApproximate field if non-nil, zero value otherwise.

### GetForksApproximateOk

`func (o *GitHubRepository) GetForksApproximateOk() (*bool, bool)`

GetForksApproximateOk returns a tuple with the ForksApproximate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetForksApproximate

`func (o *GitHubRepository) SetForksApproximate(v bool)`

SetForksApproximate sets ForksApproximate field to given value.

### HasForksApproximate

`func (o *GitHubRepository) HasForksApproximate() bool`

HasForksApproximate returns a boolean if a field has been set.

### SetForksApproximateNil

`func (o *GitHubRepository) SetForksApproximateNil(b bool)`

 SetForksApproximateNil sets the value for ForksApproximate to be an explicit nil

### UnsetForksApproximate
`func (o *GitHubRepository) UnsetForksApproximate()`

UnsetForksApproximate ensures that no value is present for ForksApproximate, not even an explicit nil
### GetIssuesApproximate

`func (o *GitHubRepository) GetIssuesApproximate() bool`

GetIssuesApproximate returns the IssuesApproximate field if non-nil, zero value otherwise.

### GetIssuesApproximateOk

`func (o *GitHubRepository) GetIssuesApproximateOk() (*bool, bool)`

GetIssuesApproximateOk returns a tuple with the IssuesApproximate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssuesApproximate

`func (o *GitHubRepository) SetIssuesApproximate(v bool)`

SetIssuesApproximate sets IssuesApproximate field to given value.

### HasIssuesApproximate

`func (o *GitHubRepository) HasIssuesApproximate() bool`

HasIssuesApproximate returns a boolean if a field has been set.

### SetIssuesApproximateNil

`func (o *GitHubRepository) SetIssuesApproximateNil(b bool)`

 SetIssuesApproximateNil sets the value for IssuesApproximate to be an explicit nil

### UnsetIssuesApproximate
`func (o *GitHubRepository) UnsetIssuesApproximate()`

UnsetIssuesApproximate ensures that no value is present for IssuesApproximate, not even an explicit nil
### GetPullRequestsApproximate

`func (o *GitHubRepository) GetPullRequestsApproximate() bool`

GetPullRequestsApproximate returns the PullRequestsApproximate field if non-nil, zero value otherwise.

### GetPullRequestsApproximateOk

`func (o *GitHubRepository) GetPullRequestsApproximateOk() (*bool, bool)`

GetPullRequestsApproximateOk returns a tuple with the PullRequestsApproximate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPullRequestsApproximate

`func (o *GitHubRepository) SetPullRequestsApproximate(v bool)`

SetPullRequestsApproximate sets PullRequestsApproximate field to given value.

### HasPullRequestsApproximate

`func (o *GitHubRepository) HasPullRequestsApproximate() bool`

HasPullRequestsApproximate returns a boolean if a field has been set.

### SetPullRequestsApproximateNil

`func (o *GitHubRepository) SetPullRequestsApproximateNil(b bool)`

 SetPullRequestsApproximateNil sets the value for PullRequestsApproximate to be an explicit nil

### UnsetPullRequestsApproximate
`func (o *GitHubRepository) UnsetPullRequestsApproximate()`

UnsetPullRequestsApproximate ensures that no value is present for PullRequestsApproximate, not even an explicit nil
### GetVisibility

`func (o *GitHubRepository) GetVisibility() string`

GetVisibility returns the Visibility field if non-nil, zero value otherwise.

### GetVisibilityOk

`func (o *GitHubRepository) GetVisibilityOk() (*string, bool)`

GetVisibilityOk returns a tuple with the Visibility field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVisibility

`func (o *GitHubRepository) SetVisibility(v string)`

SetVisibility sets Visibility field to given value.

### HasVisibility

`func (o *GitHubRepository) HasVisibility() bool`

HasVisibility returns a boolean if a field has been set.

### SetVisibilityNil

`func (o *GitHubRepository) SetVisibilityNil(b bool)`

 SetVisibilityNil sets the value for Visibility to be an explicit nil

### UnsetVisibility
`func (o *GitHubRepository) UnsetVisibility()`

UnsetVisibility ensures that no value is present for Visibility, not even an explicit nil
### GetIsFork

`func (o *GitHubRepository) GetIsFork() bool`

GetIsFork returns the IsFork field if non-nil, zero value otherwise.

### GetIsForkOk

`func (o *GitHubRepository) GetIsForkOk() (*bool, bool)`

GetIsForkOk returns a tuple with the IsFork field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsFork

`func (o *GitHubRepository) SetIsFork(v bool)`

SetIsFork sets IsFork field to given value.

### HasIsFork

`func (o *GitHubRepository) HasIsFork() bool`

HasIsFork returns a boolean if a field has been set.

### SetIsForkNil

`func (o *GitHubRepository) SetIsForkNil(b bool)`

 SetIsForkNil sets the value for IsFork to be an explicit nil

### UnsetIsFork
`func (o *GitHubRepository) UnsetIsFork()`

UnsetIsFork ensures that no value is present for IsFork, not even an explicit nil
### GetLicense

`func (o *GitHubRepository) GetLicense() string`

GetLicense returns the License field if non-nil, zero value otherwise.

### GetLicenseOk

`func (o *GitHubRepository) GetLicenseOk() (*string, bool)`

GetLicenseOk returns a tuple with the License field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLicense

`func (o *GitHubRepository) SetLicense(v string)`

SetLicense sets License field to given value.

### HasLicense

`func (o *GitHubRepository) HasLicense() bool`

HasLicense returns a boolean if a field has been set.

### SetLicenseNil

`func (o *GitHubRepository) SetLicenseNil(b bool)`

 SetLicenseNil sets the value for License to be an explicit nil

### UnsetLicense
`func (o *GitHubRepository) UnsetLicense()`

UnsetLicense ensures that no value is present for License, not even an explicit nil
### GetTopics

`func (o *GitHubRepository) GetTopics() []string`

GetTopics returns the Topics field if non-nil, zero value otherwise.

### GetTopicsOk

`func (o *GitHubRepository) GetTopicsOk() (*[]string, bool)`

GetTopicsOk returns a tuple with the Topics field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTopics

`func (o *GitHubRepository) SetTopics(v []string)`

SetTopics sets Topics field to given value.

### HasTopics

`func (o *GitHubRepository) HasTopics() bool`

HasTopics returns a boolean if a field has been set.

### SetTopicsNil

`func (o *GitHubRepository) SetTopicsNil(b bool)`

 SetTopicsNil sets the value for Topics to be an explicit nil

### UnsetTopics
`func (o *GitHubRepository) UnsetTopics()`

UnsetTopics ensures that no value is present for Topics, not even an explicit nil
### GetParticipation

`func (o *GitHubRepository) GetParticipation() []int32`

GetParticipation returns the Participation field if non-nil, zero value otherwise.

### GetParticipationOk

`func (o *GitHubRepository) GetParticipationOk() (*[]int32, bool)`

GetParticipationOk returns a tuple with the Participation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParticipation

`func (o *GitHubRepository) SetParticipation(v []int32)`

SetParticipation sets Participation field to given value.

### HasParticipation

`func (o *GitHubRepository) HasParticipation() bool`

HasParticipation returns a boolean if a field has been set.

### SetParticipationNil

`func (o *GitHubRepository) SetParticipationNil(b bool)`

 SetParticipationNil sets the value for Participation to be an explicit nil

### UnsetParticipation
`func (o *GitHubRepository) UnsetParticipation()`

UnsetParticipation ensures that no value is present for Participation, not even an explicit nil
### GetUpdatedAt

`func (o *GitHubRepository) GetUpdatedAt() string`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *GitHubRepository) GetUpdatedAtOk() (*string, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *GitHubRepository) SetUpdatedAt(v string)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *GitHubRepository) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.

### SetUpdatedAtNil

`func (o *GitHubRepository) SetUpdatedAtNil(b bool)`

 SetUpdatedAtNil sets the value for UpdatedAt to be an explicit nil

### UnsetUpdatedAt
`func (o *GitHubRepository) UnsetUpdatedAt()`

UnsetUpdatedAt ensures that no value is present for UpdatedAt, not even an explicit nil
### GetUpdatedUtc

`func (o *GitHubRepository) GetUpdatedUtc() float32`

GetUpdatedUtc returns the UpdatedUtc field if non-nil, zero value otherwise.

### GetUpdatedUtcOk

`func (o *GitHubRepository) GetUpdatedUtcOk() (*float32, bool)`

GetUpdatedUtcOk returns a tuple with the UpdatedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedUtc

`func (o *GitHubRepository) SetUpdatedUtc(v float32)`

SetUpdatedUtc sets UpdatedUtc field to given value.

### HasUpdatedUtc

`func (o *GitHubRepository) HasUpdatedUtc() bool`

HasUpdatedUtc returns a boolean if a field has been set.

### SetUpdatedUtcNil

`func (o *GitHubRepository) SetUpdatedUtcNil(b bool)`

 SetUpdatedUtcNil sets the value for UpdatedUtc to be an explicit nil

### UnsetUpdatedUtc
`func (o *GitHubRepository) UnsetUpdatedUtc()`

UnsetUpdatedUtc ensures that no value is present for UpdatedUtc, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



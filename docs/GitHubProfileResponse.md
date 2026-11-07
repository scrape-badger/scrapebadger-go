# GitHubProfileResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Profile** | [**GitHubProfile**](GitHubProfile.md) |  | 
**PinnedRepositories** | Pointer to [**[]GitHubRepository**](GitHubRepository.md) |  | [optional] 
**PopularRepositories** | Pointer to [**[]GitHubRepository**](GitHubRepository.md) |  | [optional] 
**Readme** | Pointer to [**NullableGitHubReadme**](GitHubReadme.md) |  | [optional] 
**Organizations** | Pointer to [**[]GitHubAccountPreview**](GitHubAccountPreview.md) |  | [optional] 
**Sponsors** | Pointer to [**[]GitHubAccountPreview**](GitHubAccountPreview.md) |  | [optional] 
**Sponsoring** | Pointer to [**[]GitHubAccountPreview**](GitHubAccountPreview.md) |  | [optional] 
**AdditionalSponsorsCount** | Pointer to **NullableInt32** |  | [optional] 
**AdditionalSponsoringCount** | Pointer to **NullableInt32** |  | [optional] 
**Achievements** | Pointer to [**[]GitHubAchievement**](GitHubAchievement.md) |  | [optional] 
**Highlights** | Pointer to [**[]GitHubTextLink**](GitHubTextLink.md) |  | [optional] 
**Contributions** | Pointer to [**NullableGitHubContributions**](GitHubContributions.md) |  | [optional] 
**Repositories** | Pointer to [**[]GitHubRepository**](GitHubRepository.md) |  | [optional] 
**StarredRepositories** | Pointer to [**[]GitHubRepository**](GitHubRepository.md) |  | [optional] 
**StarLists** | Pointer to [**[]GitHubNamedLink**](GitHubNamedLink.md) |  | [optional] 
**Pagination** | Pointer to [**NullableGitHubPagination**](GitHubPagination.md) |  | [optional] 
**TopLanguages** | Pointer to [**[]GitHubLanguage**](GitHubLanguage.md) |  | [optional] 
**Topics** | Pointer to **[]string** |  | [optional] 
**People** | Pointer to [**[]GitHubAccountPreview**](GitHubAccountPreview.md) |  | [optional] 
**VerifiedDomains** | Pointer to **[]string** |  | [optional] 

## Methods

### NewGitHubProfileResponse

`func NewGitHubProfileResponse(profile GitHubProfile, ) *GitHubProfileResponse`

NewGitHubProfileResponse instantiates a new GitHubProfileResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubProfileResponseWithDefaults

`func NewGitHubProfileResponseWithDefaults() *GitHubProfileResponse`

NewGitHubProfileResponseWithDefaults instantiates a new GitHubProfileResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProfile

`func (o *GitHubProfileResponse) GetProfile() GitHubProfile`

GetProfile returns the Profile field if non-nil, zero value otherwise.

### GetProfileOk

`func (o *GitHubProfileResponse) GetProfileOk() (*GitHubProfile, bool)`

GetProfileOk returns a tuple with the Profile field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProfile

`func (o *GitHubProfileResponse) SetProfile(v GitHubProfile)`

SetProfile sets Profile field to given value.


### GetPinnedRepositories

`func (o *GitHubProfileResponse) GetPinnedRepositories() []GitHubRepository`

GetPinnedRepositories returns the PinnedRepositories field if non-nil, zero value otherwise.

### GetPinnedRepositoriesOk

`func (o *GitHubProfileResponse) GetPinnedRepositoriesOk() (*[]GitHubRepository, bool)`

GetPinnedRepositoriesOk returns a tuple with the PinnedRepositories field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPinnedRepositories

`func (o *GitHubProfileResponse) SetPinnedRepositories(v []GitHubRepository)`

SetPinnedRepositories sets PinnedRepositories field to given value.

### HasPinnedRepositories

`func (o *GitHubProfileResponse) HasPinnedRepositories() bool`

HasPinnedRepositories returns a boolean if a field has been set.

### SetPinnedRepositoriesNil

`func (o *GitHubProfileResponse) SetPinnedRepositoriesNil(b bool)`

 SetPinnedRepositoriesNil sets the value for PinnedRepositories to be an explicit nil

### UnsetPinnedRepositories
`func (o *GitHubProfileResponse) UnsetPinnedRepositories()`

UnsetPinnedRepositories ensures that no value is present for PinnedRepositories, not even an explicit nil
### GetPopularRepositories

`func (o *GitHubProfileResponse) GetPopularRepositories() []GitHubRepository`

GetPopularRepositories returns the PopularRepositories field if non-nil, zero value otherwise.

### GetPopularRepositoriesOk

`func (o *GitHubProfileResponse) GetPopularRepositoriesOk() (*[]GitHubRepository, bool)`

GetPopularRepositoriesOk returns a tuple with the PopularRepositories field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPopularRepositories

`func (o *GitHubProfileResponse) SetPopularRepositories(v []GitHubRepository)`

SetPopularRepositories sets PopularRepositories field to given value.

### HasPopularRepositories

`func (o *GitHubProfileResponse) HasPopularRepositories() bool`

HasPopularRepositories returns a boolean if a field has been set.

### SetPopularRepositoriesNil

`func (o *GitHubProfileResponse) SetPopularRepositoriesNil(b bool)`

 SetPopularRepositoriesNil sets the value for PopularRepositories to be an explicit nil

### UnsetPopularRepositories
`func (o *GitHubProfileResponse) UnsetPopularRepositories()`

UnsetPopularRepositories ensures that no value is present for PopularRepositories, not even an explicit nil
### GetReadme

`func (o *GitHubProfileResponse) GetReadme() GitHubReadme`

GetReadme returns the Readme field if non-nil, zero value otherwise.

### GetReadmeOk

`func (o *GitHubProfileResponse) GetReadmeOk() (*GitHubReadme, bool)`

GetReadmeOk returns a tuple with the Readme field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReadme

`func (o *GitHubProfileResponse) SetReadme(v GitHubReadme)`

SetReadme sets Readme field to given value.

### HasReadme

`func (o *GitHubProfileResponse) HasReadme() bool`

HasReadme returns a boolean if a field has been set.

### SetReadmeNil

`func (o *GitHubProfileResponse) SetReadmeNil(b bool)`

 SetReadmeNil sets the value for Readme to be an explicit nil

### UnsetReadme
`func (o *GitHubProfileResponse) UnsetReadme()`

UnsetReadme ensures that no value is present for Readme, not even an explicit nil
### GetOrganizations

`func (o *GitHubProfileResponse) GetOrganizations() []GitHubAccountPreview`

GetOrganizations returns the Organizations field if non-nil, zero value otherwise.

### GetOrganizationsOk

`func (o *GitHubProfileResponse) GetOrganizationsOk() (*[]GitHubAccountPreview, bool)`

GetOrganizationsOk returns a tuple with the Organizations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganizations

`func (o *GitHubProfileResponse) SetOrganizations(v []GitHubAccountPreview)`

SetOrganizations sets Organizations field to given value.

### HasOrganizations

`func (o *GitHubProfileResponse) HasOrganizations() bool`

HasOrganizations returns a boolean if a field has been set.

### SetOrganizationsNil

`func (o *GitHubProfileResponse) SetOrganizationsNil(b bool)`

 SetOrganizationsNil sets the value for Organizations to be an explicit nil

### UnsetOrganizations
`func (o *GitHubProfileResponse) UnsetOrganizations()`

UnsetOrganizations ensures that no value is present for Organizations, not even an explicit nil
### GetSponsors

`func (o *GitHubProfileResponse) GetSponsors() []GitHubAccountPreview`

GetSponsors returns the Sponsors field if non-nil, zero value otherwise.

### GetSponsorsOk

`func (o *GitHubProfileResponse) GetSponsorsOk() (*[]GitHubAccountPreview, bool)`

GetSponsorsOk returns a tuple with the Sponsors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSponsors

`func (o *GitHubProfileResponse) SetSponsors(v []GitHubAccountPreview)`

SetSponsors sets Sponsors field to given value.

### HasSponsors

`func (o *GitHubProfileResponse) HasSponsors() bool`

HasSponsors returns a boolean if a field has been set.

### SetSponsorsNil

`func (o *GitHubProfileResponse) SetSponsorsNil(b bool)`

 SetSponsorsNil sets the value for Sponsors to be an explicit nil

### UnsetSponsors
`func (o *GitHubProfileResponse) UnsetSponsors()`

UnsetSponsors ensures that no value is present for Sponsors, not even an explicit nil
### GetSponsoring

`func (o *GitHubProfileResponse) GetSponsoring() []GitHubAccountPreview`

GetSponsoring returns the Sponsoring field if non-nil, zero value otherwise.

### GetSponsoringOk

`func (o *GitHubProfileResponse) GetSponsoringOk() (*[]GitHubAccountPreview, bool)`

GetSponsoringOk returns a tuple with the Sponsoring field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSponsoring

`func (o *GitHubProfileResponse) SetSponsoring(v []GitHubAccountPreview)`

SetSponsoring sets Sponsoring field to given value.

### HasSponsoring

`func (o *GitHubProfileResponse) HasSponsoring() bool`

HasSponsoring returns a boolean if a field has been set.

### SetSponsoringNil

`func (o *GitHubProfileResponse) SetSponsoringNil(b bool)`

 SetSponsoringNil sets the value for Sponsoring to be an explicit nil

### UnsetSponsoring
`func (o *GitHubProfileResponse) UnsetSponsoring()`

UnsetSponsoring ensures that no value is present for Sponsoring, not even an explicit nil
### GetAdditionalSponsorsCount

`func (o *GitHubProfileResponse) GetAdditionalSponsorsCount() int32`

GetAdditionalSponsorsCount returns the AdditionalSponsorsCount field if non-nil, zero value otherwise.

### GetAdditionalSponsorsCountOk

`func (o *GitHubProfileResponse) GetAdditionalSponsorsCountOk() (*int32, bool)`

GetAdditionalSponsorsCountOk returns a tuple with the AdditionalSponsorsCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdditionalSponsorsCount

`func (o *GitHubProfileResponse) SetAdditionalSponsorsCount(v int32)`

SetAdditionalSponsorsCount sets AdditionalSponsorsCount field to given value.

### HasAdditionalSponsorsCount

`func (o *GitHubProfileResponse) HasAdditionalSponsorsCount() bool`

HasAdditionalSponsorsCount returns a boolean if a field has been set.

### SetAdditionalSponsorsCountNil

`func (o *GitHubProfileResponse) SetAdditionalSponsorsCountNil(b bool)`

 SetAdditionalSponsorsCountNil sets the value for AdditionalSponsorsCount to be an explicit nil

### UnsetAdditionalSponsorsCount
`func (o *GitHubProfileResponse) UnsetAdditionalSponsorsCount()`

UnsetAdditionalSponsorsCount ensures that no value is present for AdditionalSponsorsCount, not even an explicit nil
### GetAdditionalSponsoringCount

`func (o *GitHubProfileResponse) GetAdditionalSponsoringCount() int32`

GetAdditionalSponsoringCount returns the AdditionalSponsoringCount field if non-nil, zero value otherwise.

### GetAdditionalSponsoringCountOk

`func (o *GitHubProfileResponse) GetAdditionalSponsoringCountOk() (*int32, bool)`

GetAdditionalSponsoringCountOk returns a tuple with the AdditionalSponsoringCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdditionalSponsoringCount

`func (o *GitHubProfileResponse) SetAdditionalSponsoringCount(v int32)`

SetAdditionalSponsoringCount sets AdditionalSponsoringCount field to given value.

### HasAdditionalSponsoringCount

`func (o *GitHubProfileResponse) HasAdditionalSponsoringCount() bool`

HasAdditionalSponsoringCount returns a boolean if a field has been set.

### SetAdditionalSponsoringCountNil

`func (o *GitHubProfileResponse) SetAdditionalSponsoringCountNil(b bool)`

 SetAdditionalSponsoringCountNil sets the value for AdditionalSponsoringCount to be an explicit nil

### UnsetAdditionalSponsoringCount
`func (o *GitHubProfileResponse) UnsetAdditionalSponsoringCount()`

UnsetAdditionalSponsoringCount ensures that no value is present for AdditionalSponsoringCount, not even an explicit nil
### GetAchievements

`func (o *GitHubProfileResponse) GetAchievements() []GitHubAchievement`

GetAchievements returns the Achievements field if non-nil, zero value otherwise.

### GetAchievementsOk

`func (o *GitHubProfileResponse) GetAchievementsOk() (*[]GitHubAchievement, bool)`

GetAchievementsOk returns a tuple with the Achievements field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAchievements

`func (o *GitHubProfileResponse) SetAchievements(v []GitHubAchievement)`

SetAchievements sets Achievements field to given value.

### HasAchievements

`func (o *GitHubProfileResponse) HasAchievements() bool`

HasAchievements returns a boolean if a field has been set.

### SetAchievementsNil

`func (o *GitHubProfileResponse) SetAchievementsNil(b bool)`

 SetAchievementsNil sets the value for Achievements to be an explicit nil

### UnsetAchievements
`func (o *GitHubProfileResponse) UnsetAchievements()`

UnsetAchievements ensures that no value is present for Achievements, not even an explicit nil
### GetHighlights

`func (o *GitHubProfileResponse) GetHighlights() []GitHubTextLink`

GetHighlights returns the Highlights field if non-nil, zero value otherwise.

### GetHighlightsOk

`func (o *GitHubProfileResponse) GetHighlightsOk() (*[]GitHubTextLink, bool)`

GetHighlightsOk returns a tuple with the Highlights field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHighlights

`func (o *GitHubProfileResponse) SetHighlights(v []GitHubTextLink)`

SetHighlights sets Highlights field to given value.

### HasHighlights

`func (o *GitHubProfileResponse) HasHighlights() bool`

HasHighlights returns a boolean if a field has been set.

### SetHighlightsNil

`func (o *GitHubProfileResponse) SetHighlightsNil(b bool)`

 SetHighlightsNil sets the value for Highlights to be an explicit nil

### UnsetHighlights
`func (o *GitHubProfileResponse) UnsetHighlights()`

UnsetHighlights ensures that no value is present for Highlights, not even an explicit nil
### GetContributions

`func (o *GitHubProfileResponse) GetContributions() GitHubContributions`

GetContributions returns the Contributions field if non-nil, zero value otherwise.

### GetContributionsOk

`func (o *GitHubProfileResponse) GetContributionsOk() (*GitHubContributions, bool)`

GetContributionsOk returns a tuple with the Contributions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContributions

`func (o *GitHubProfileResponse) SetContributions(v GitHubContributions)`

SetContributions sets Contributions field to given value.

### HasContributions

`func (o *GitHubProfileResponse) HasContributions() bool`

HasContributions returns a boolean if a field has been set.

### SetContributionsNil

`func (o *GitHubProfileResponse) SetContributionsNil(b bool)`

 SetContributionsNil sets the value for Contributions to be an explicit nil

### UnsetContributions
`func (o *GitHubProfileResponse) UnsetContributions()`

UnsetContributions ensures that no value is present for Contributions, not even an explicit nil
### GetRepositories

`func (o *GitHubProfileResponse) GetRepositories() []GitHubRepository`

GetRepositories returns the Repositories field if non-nil, zero value otherwise.

### GetRepositoriesOk

`func (o *GitHubProfileResponse) GetRepositoriesOk() (*[]GitHubRepository, bool)`

GetRepositoriesOk returns a tuple with the Repositories field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRepositories

`func (o *GitHubProfileResponse) SetRepositories(v []GitHubRepository)`

SetRepositories sets Repositories field to given value.

### HasRepositories

`func (o *GitHubProfileResponse) HasRepositories() bool`

HasRepositories returns a boolean if a field has been set.

### SetRepositoriesNil

`func (o *GitHubProfileResponse) SetRepositoriesNil(b bool)`

 SetRepositoriesNil sets the value for Repositories to be an explicit nil

### UnsetRepositories
`func (o *GitHubProfileResponse) UnsetRepositories()`

UnsetRepositories ensures that no value is present for Repositories, not even an explicit nil
### GetStarredRepositories

`func (o *GitHubProfileResponse) GetStarredRepositories() []GitHubRepository`

GetStarredRepositories returns the StarredRepositories field if non-nil, zero value otherwise.

### GetStarredRepositoriesOk

`func (o *GitHubProfileResponse) GetStarredRepositoriesOk() (*[]GitHubRepository, bool)`

GetStarredRepositoriesOk returns a tuple with the StarredRepositories field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStarredRepositories

`func (o *GitHubProfileResponse) SetStarredRepositories(v []GitHubRepository)`

SetStarredRepositories sets StarredRepositories field to given value.

### HasStarredRepositories

`func (o *GitHubProfileResponse) HasStarredRepositories() bool`

HasStarredRepositories returns a boolean if a field has been set.

### SetStarredRepositoriesNil

`func (o *GitHubProfileResponse) SetStarredRepositoriesNil(b bool)`

 SetStarredRepositoriesNil sets the value for StarredRepositories to be an explicit nil

### UnsetStarredRepositories
`func (o *GitHubProfileResponse) UnsetStarredRepositories()`

UnsetStarredRepositories ensures that no value is present for StarredRepositories, not even an explicit nil
### GetStarLists

`func (o *GitHubProfileResponse) GetStarLists() []GitHubNamedLink`

GetStarLists returns the StarLists field if non-nil, zero value otherwise.

### GetStarListsOk

`func (o *GitHubProfileResponse) GetStarListsOk() (*[]GitHubNamedLink, bool)`

GetStarListsOk returns a tuple with the StarLists field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStarLists

`func (o *GitHubProfileResponse) SetStarLists(v []GitHubNamedLink)`

SetStarLists sets StarLists field to given value.

### HasStarLists

`func (o *GitHubProfileResponse) HasStarLists() bool`

HasStarLists returns a boolean if a field has been set.

### SetStarListsNil

`func (o *GitHubProfileResponse) SetStarListsNil(b bool)`

 SetStarListsNil sets the value for StarLists to be an explicit nil

### UnsetStarLists
`func (o *GitHubProfileResponse) UnsetStarLists()`

UnsetStarLists ensures that no value is present for StarLists, not even an explicit nil
### GetPagination

`func (o *GitHubProfileResponse) GetPagination() GitHubPagination`

GetPagination returns the Pagination field if non-nil, zero value otherwise.

### GetPaginationOk

`func (o *GitHubProfileResponse) GetPaginationOk() (*GitHubPagination, bool)`

GetPaginationOk returns a tuple with the Pagination field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPagination

`func (o *GitHubProfileResponse) SetPagination(v GitHubPagination)`

SetPagination sets Pagination field to given value.

### HasPagination

`func (o *GitHubProfileResponse) HasPagination() bool`

HasPagination returns a boolean if a field has been set.

### SetPaginationNil

`func (o *GitHubProfileResponse) SetPaginationNil(b bool)`

 SetPaginationNil sets the value for Pagination to be an explicit nil

### UnsetPagination
`func (o *GitHubProfileResponse) UnsetPagination()`

UnsetPagination ensures that no value is present for Pagination, not even an explicit nil
### GetTopLanguages

`func (o *GitHubProfileResponse) GetTopLanguages() []GitHubLanguage`

GetTopLanguages returns the TopLanguages field if non-nil, zero value otherwise.

### GetTopLanguagesOk

`func (o *GitHubProfileResponse) GetTopLanguagesOk() (*[]GitHubLanguage, bool)`

GetTopLanguagesOk returns a tuple with the TopLanguages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTopLanguages

`func (o *GitHubProfileResponse) SetTopLanguages(v []GitHubLanguage)`

SetTopLanguages sets TopLanguages field to given value.

### HasTopLanguages

`func (o *GitHubProfileResponse) HasTopLanguages() bool`

HasTopLanguages returns a boolean if a field has been set.

### SetTopLanguagesNil

`func (o *GitHubProfileResponse) SetTopLanguagesNil(b bool)`

 SetTopLanguagesNil sets the value for TopLanguages to be an explicit nil

### UnsetTopLanguages
`func (o *GitHubProfileResponse) UnsetTopLanguages()`

UnsetTopLanguages ensures that no value is present for TopLanguages, not even an explicit nil
### GetTopics

`func (o *GitHubProfileResponse) GetTopics() []string`

GetTopics returns the Topics field if non-nil, zero value otherwise.

### GetTopicsOk

`func (o *GitHubProfileResponse) GetTopicsOk() (*[]string, bool)`

GetTopicsOk returns a tuple with the Topics field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTopics

`func (o *GitHubProfileResponse) SetTopics(v []string)`

SetTopics sets Topics field to given value.

### HasTopics

`func (o *GitHubProfileResponse) HasTopics() bool`

HasTopics returns a boolean if a field has been set.

### SetTopicsNil

`func (o *GitHubProfileResponse) SetTopicsNil(b bool)`

 SetTopicsNil sets the value for Topics to be an explicit nil

### UnsetTopics
`func (o *GitHubProfileResponse) UnsetTopics()`

UnsetTopics ensures that no value is present for Topics, not even an explicit nil
### GetPeople

`func (o *GitHubProfileResponse) GetPeople() []GitHubAccountPreview`

GetPeople returns the People field if non-nil, zero value otherwise.

### GetPeopleOk

`func (o *GitHubProfileResponse) GetPeopleOk() (*[]GitHubAccountPreview, bool)`

GetPeopleOk returns a tuple with the People field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPeople

`func (o *GitHubProfileResponse) SetPeople(v []GitHubAccountPreview)`

SetPeople sets People field to given value.

### HasPeople

`func (o *GitHubProfileResponse) HasPeople() bool`

HasPeople returns a boolean if a field has been set.

### SetPeopleNil

`func (o *GitHubProfileResponse) SetPeopleNil(b bool)`

 SetPeopleNil sets the value for People to be an explicit nil

### UnsetPeople
`func (o *GitHubProfileResponse) UnsetPeople()`

UnsetPeople ensures that no value is present for People, not even an explicit nil
### GetVerifiedDomains

`func (o *GitHubProfileResponse) GetVerifiedDomains() []string`

GetVerifiedDomains returns the VerifiedDomains field if non-nil, zero value otherwise.

### GetVerifiedDomainsOk

`func (o *GitHubProfileResponse) GetVerifiedDomainsOk() (*[]string, bool)`

GetVerifiedDomainsOk returns a tuple with the VerifiedDomains field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVerifiedDomains

`func (o *GitHubProfileResponse) SetVerifiedDomains(v []string)`

SetVerifiedDomains sets VerifiedDomains field to given value.

### HasVerifiedDomains

`func (o *GitHubProfileResponse) HasVerifiedDomains() bool`

HasVerifiedDomains returns a boolean if a field has been set.

### SetVerifiedDomainsNil

`func (o *GitHubProfileResponse) SetVerifiedDomainsNil(b bool)`

 SetVerifiedDomainsNil sets the value for VerifiedDomains to be an explicit nil

### UnsetVerifiedDomains
`func (o *GitHubProfileResponse) UnsetVerifiedDomains()`

UnsetVerifiedDomains ensures that no value is present for VerifiedDomains, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



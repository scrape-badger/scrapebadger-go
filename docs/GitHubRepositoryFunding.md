# GitHubRepositoryFunding

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**GithubSponsors** | Pointer to [**[]GitHubRepositoryAccount**](GitHubRepositoryAccount.md) |  | [optional] 
**Links** | Pointer to [**[]GitHubFundingLink**](GitHubFundingLink.md) |  | [optional] 
**SponsorableCount** | Pointer to **NullableInt32** |  | [optional] 
**SponsorsLink** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewGitHubRepositoryFunding

`func NewGitHubRepositoryFunding() *GitHubRepositoryFunding`

NewGitHubRepositoryFunding instantiates a new GitHubRepositoryFunding object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubRepositoryFundingWithDefaults

`func NewGitHubRepositoryFundingWithDefaults() *GitHubRepositoryFunding`

NewGitHubRepositoryFundingWithDefaults instantiates a new GitHubRepositoryFunding object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetGithubSponsors

`func (o *GitHubRepositoryFunding) GetGithubSponsors() []GitHubRepositoryAccount`

GetGithubSponsors returns the GithubSponsors field if non-nil, zero value otherwise.

### GetGithubSponsorsOk

`func (o *GitHubRepositoryFunding) GetGithubSponsorsOk() (*[]GitHubRepositoryAccount, bool)`

GetGithubSponsorsOk returns a tuple with the GithubSponsors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGithubSponsors

`func (o *GitHubRepositoryFunding) SetGithubSponsors(v []GitHubRepositoryAccount)`

SetGithubSponsors sets GithubSponsors field to given value.

### HasGithubSponsors

`func (o *GitHubRepositoryFunding) HasGithubSponsors() bool`

HasGithubSponsors returns a boolean if a field has been set.

### SetGithubSponsorsNil

`func (o *GitHubRepositoryFunding) SetGithubSponsorsNil(b bool)`

 SetGithubSponsorsNil sets the value for GithubSponsors to be an explicit nil

### UnsetGithubSponsors
`func (o *GitHubRepositoryFunding) UnsetGithubSponsors()`

UnsetGithubSponsors ensures that no value is present for GithubSponsors, not even an explicit nil
### GetLinks

`func (o *GitHubRepositoryFunding) GetLinks() []GitHubFundingLink`

GetLinks returns the Links field if non-nil, zero value otherwise.

### GetLinksOk

`func (o *GitHubRepositoryFunding) GetLinksOk() (*[]GitHubFundingLink, bool)`

GetLinksOk returns a tuple with the Links field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLinks

`func (o *GitHubRepositoryFunding) SetLinks(v []GitHubFundingLink)`

SetLinks sets Links field to given value.

### HasLinks

`func (o *GitHubRepositoryFunding) HasLinks() bool`

HasLinks returns a boolean if a field has been set.

### SetLinksNil

`func (o *GitHubRepositoryFunding) SetLinksNil(b bool)`

 SetLinksNil sets the value for Links to be an explicit nil

### UnsetLinks
`func (o *GitHubRepositoryFunding) UnsetLinks()`

UnsetLinks ensures that no value is present for Links, not even an explicit nil
### GetSponsorableCount

`func (o *GitHubRepositoryFunding) GetSponsorableCount() int32`

GetSponsorableCount returns the SponsorableCount field if non-nil, zero value otherwise.

### GetSponsorableCountOk

`func (o *GitHubRepositoryFunding) GetSponsorableCountOk() (*int32, bool)`

GetSponsorableCountOk returns a tuple with the SponsorableCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSponsorableCount

`func (o *GitHubRepositoryFunding) SetSponsorableCount(v int32)`

SetSponsorableCount sets SponsorableCount field to given value.

### HasSponsorableCount

`func (o *GitHubRepositoryFunding) HasSponsorableCount() bool`

HasSponsorableCount returns a boolean if a field has been set.

### SetSponsorableCountNil

`func (o *GitHubRepositoryFunding) SetSponsorableCountNil(b bool)`

 SetSponsorableCountNil sets the value for SponsorableCount to be an explicit nil

### UnsetSponsorableCount
`func (o *GitHubRepositoryFunding) UnsetSponsorableCount()`

UnsetSponsorableCount ensures that no value is present for SponsorableCount, not even an explicit nil
### GetSponsorsLink

`func (o *GitHubRepositoryFunding) GetSponsorsLink() string`

GetSponsorsLink returns the SponsorsLink field if non-nil, zero value otherwise.

### GetSponsorsLinkOk

`func (o *GitHubRepositoryFunding) GetSponsorsLinkOk() (*string, bool)`

GetSponsorsLinkOk returns a tuple with the SponsorsLink field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSponsorsLink

`func (o *GitHubRepositoryFunding) SetSponsorsLink(v string)`

SetSponsorsLink sets SponsorsLink field to given value.

### HasSponsorsLink

`func (o *GitHubRepositoryFunding) HasSponsorsLink() bool`

HasSponsorsLink returns a boolean if a field has been set.

### SetSponsorsLinkNil

`func (o *GitHubRepositoryFunding) SetSponsorsLinkNil(b bool)`

 SetSponsorsLinkNil sets the value for SponsorsLink to be an explicit nil

### UnsetSponsorsLink
`func (o *GitHubRepositoryFunding) UnsetSponsorsLink()`

UnsetSponsorsLink ensures that no value is present for SponsorsLink, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



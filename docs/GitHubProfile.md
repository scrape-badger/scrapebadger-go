# GitHubProfile

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Login** | **string** |  | 
**Link** | **string** |  | 
**IsOrganization** | **bool** |  | 
**Id** | Pointer to **NullableInt32** |  | [optional] 
**NodeId** | Pointer to **NullableString** |  | [optional] 
**Type** | Pointer to **NullableString** |  | [optional] 
**UserViewType** | Pointer to **NullableString** |  | [optional] 
**SiteAdmin** | Pointer to **NullableBool** |  | [optional] 
**Name** | Pointer to **NullableString** |  | [optional] 
**AvatarUrl** | Pointer to **NullableString** |  | [optional] 
**Bio** | Pointer to **NullableString** |  | [optional] 
**Description** | Pointer to **NullableString** |  | [optional] 
**Pronouns** | Pointer to **NullableString** |  | [optional] 
**LocalTime** | Pointer to **NullableString** |  | [optional] 
**UtcOffset** | Pointer to **NullableFloat32** |  | [optional] 
**Company** | Pointer to **NullableString** |  | [optional] 
**Location** | Pointer to **NullableString** |  | [optional] 
**Email** | Pointer to **NullableString** |  | [optional] 
**Website** | Pointer to **NullableString** |  | [optional] 
**TwitterUsername** | Pointer to **NullableString** |  | [optional] 
**Hireable** | Pointer to **NullableBool** |  | [optional] 
**SocialAccounts** | Pointer to [**[]GitHubSocialAccount**](GitHubSocialAccount.md) |  | [optional] 
**Status** | Pointer to [**NullableGitHubStatus**](GitHubStatus.md) |  | [optional] 
**Followers** | Pointer to **NullableInt32** |  | [optional] 
**Following** | Pointer to **NullableInt32** |  | [optional] 
**Repos** | Pointer to **NullableInt32** |  | [optional] 
**PublicRepos** | Pointer to **NullableInt32** |  | [optional] 
**PublicGists** | Pointer to **NullableInt32** |  | [optional] 
**FollowersDisplayCount** | Pointer to **NullableInt32** |  | [optional] 
**FollowingDisplayCount** | Pointer to **NullableInt32** |  | [optional] 
**ReposDisplayCount** | Pointer to **NullableInt32** |  | [optional] 
**FollowersApproximate** | Pointer to **NullableBool** |  | [optional] 
**FollowingApproximate** | Pointer to **NullableBool** |  | [optional] 
**ReposApproximate** | Pointer to **NullableBool** |  | [optional] 
**StarredCount** | Pointer to **NullableInt32** |  | [optional] 
**StarredCountApproximate** | Pointer to **NullableBool** |  | [optional] 
**ProjectsCount** | Pointer to **NullableInt32** |  | [optional] 
**ProjectsCountApproximate** | Pointer to **NullableBool** |  | [optional] 
**PackagesCount** | Pointer to **NullableInt32** |  | [optional] 
**PackagesCountApproximate** | Pointer to **NullableBool** |  | [optional] 
**SponsoringCount** | Pointer to **NullableInt32** |  | [optional] 
**SponsoringCountApproximate** | Pointer to **NullableBool** |  | [optional] 
**IsSponsorable** | Pointer to **NullableBool** |  | [optional] 
**SponsorsLink** | Pointer to **NullableString** |  | [optional] 
**IsVerified** | Pointer to **NullableBool** |  | [optional] 
**HasOrganizationProjects** | Pointer to **NullableBool** |  | [optional] 
**HasRepositoryProjects** | Pointer to **NullableBool** |  | [optional] 
**CreatedAt** | Pointer to **NullableString** |  | [optional] 
**CreatedUtc** | Pointer to **NullableFloat32** |  | [optional] 
**UpdatedAt** | Pointer to **NullableString** |  | [optional] 
**UpdatedUtc** | Pointer to **NullableFloat32** |  | [optional] 
**ArchivedAt** | Pointer to **NullableString** |  | [optional] 
**ArchivedUtc** | Pointer to **NullableFloat32** |  | [optional] 

## Methods

### NewGitHubProfile

`func NewGitHubProfile(login string, link string, isOrganization bool, ) *GitHubProfile`

NewGitHubProfile instantiates a new GitHubProfile object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubProfileWithDefaults

`func NewGitHubProfileWithDefaults() *GitHubProfile`

NewGitHubProfileWithDefaults instantiates a new GitHubProfile object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLogin

`func (o *GitHubProfile) GetLogin() string`

GetLogin returns the Login field if non-nil, zero value otherwise.

### GetLoginOk

`func (o *GitHubProfile) GetLoginOk() (*string, bool)`

GetLoginOk returns a tuple with the Login field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogin

`func (o *GitHubProfile) SetLogin(v string)`

SetLogin sets Login field to given value.


### GetLink

`func (o *GitHubProfile) GetLink() string`

GetLink returns the Link field if non-nil, zero value otherwise.

### GetLinkOk

`func (o *GitHubProfile) GetLinkOk() (*string, bool)`

GetLinkOk returns a tuple with the Link field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLink

`func (o *GitHubProfile) SetLink(v string)`

SetLink sets Link field to given value.


### GetIsOrganization

`func (o *GitHubProfile) GetIsOrganization() bool`

GetIsOrganization returns the IsOrganization field if non-nil, zero value otherwise.

### GetIsOrganizationOk

`func (o *GitHubProfile) GetIsOrganizationOk() (*bool, bool)`

GetIsOrganizationOk returns a tuple with the IsOrganization field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsOrganization

`func (o *GitHubProfile) SetIsOrganization(v bool)`

SetIsOrganization sets IsOrganization field to given value.


### GetId

`func (o *GitHubProfile) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *GitHubProfile) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *GitHubProfile) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *GitHubProfile) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *GitHubProfile) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *GitHubProfile) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil
### GetNodeId

`func (o *GitHubProfile) GetNodeId() string`

GetNodeId returns the NodeId field if non-nil, zero value otherwise.

### GetNodeIdOk

`func (o *GitHubProfile) GetNodeIdOk() (*string, bool)`

GetNodeIdOk returns a tuple with the NodeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNodeId

`func (o *GitHubProfile) SetNodeId(v string)`

SetNodeId sets NodeId field to given value.

### HasNodeId

`func (o *GitHubProfile) HasNodeId() bool`

HasNodeId returns a boolean if a field has been set.

### SetNodeIdNil

`func (o *GitHubProfile) SetNodeIdNil(b bool)`

 SetNodeIdNil sets the value for NodeId to be an explicit nil

### UnsetNodeId
`func (o *GitHubProfile) UnsetNodeId()`

UnsetNodeId ensures that no value is present for NodeId, not even an explicit nil
### GetType

`func (o *GitHubProfile) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *GitHubProfile) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *GitHubProfile) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *GitHubProfile) HasType() bool`

HasType returns a boolean if a field has been set.

### SetTypeNil

`func (o *GitHubProfile) SetTypeNil(b bool)`

 SetTypeNil sets the value for Type to be an explicit nil

### UnsetType
`func (o *GitHubProfile) UnsetType()`

UnsetType ensures that no value is present for Type, not even an explicit nil
### GetUserViewType

`func (o *GitHubProfile) GetUserViewType() string`

GetUserViewType returns the UserViewType field if non-nil, zero value otherwise.

### GetUserViewTypeOk

`func (o *GitHubProfile) GetUserViewTypeOk() (*string, bool)`

GetUserViewTypeOk returns a tuple with the UserViewType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserViewType

`func (o *GitHubProfile) SetUserViewType(v string)`

SetUserViewType sets UserViewType field to given value.

### HasUserViewType

`func (o *GitHubProfile) HasUserViewType() bool`

HasUserViewType returns a boolean if a field has been set.

### SetUserViewTypeNil

`func (o *GitHubProfile) SetUserViewTypeNil(b bool)`

 SetUserViewTypeNil sets the value for UserViewType to be an explicit nil

### UnsetUserViewType
`func (o *GitHubProfile) UnsetUserViewType()`

UnsetUserViewType ensures that no value is present for UserViewType, not even an explicit nil
### GetSiteAdmin

`func (o *GitHubProfile) GetSiteAdmin() bool`

GetSiteAdmin returns the SiteAdmin field if non-nil, zero value otherwise.

### GetSiteAdminOk

`func (o *GitHubProfile) GetSiteAdminOk() (*bool, bool)`

GetSiteAdminOk returns a tuple with the SiteAdmin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSiteAdmin

`func (o *GitHubProfile) SetSiteAdmin(v bool)`

SetSiteAdmin sets SiteAdmin field to given value.

### HasSiteAdmin

`func (o *GitHubProfile) HasSiteAdmin() bool`

HasSiteAdmin returns a boolean if a field has been set.

### SetSiteAdminNil

`func (o *GitHubProfile) SetSiteAdminNil(b bool)`

 SetSiteAdminNil sets the value for SiteAdmin to be an explicit nil

### UnsetSiteAdmin
`func (o *GitHubProfile) UnsetSiteAdmin()`

UnsetSiteAdmin ensures that no value is present for SiteAdmin, not even an explicit nil
### GetName

`func (o *GitHubProfile) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *GitHubProfile) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *GitHubProfile) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *GitHubProfile) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *GitHubProfile) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *GitHubProfile) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetAvatarUrl

`func (o *GitHubProfile) GetAvatarUrl() string`

GetAvatarUrl returns the AvatarUrl field if non-nil, zero value otherwise.

### GetAvatarUrlOk

`func (o *GitHubProfile) GetAvatarUrlOk() (*string, bool)`

GetAvatarUrlOk returns a tuple with the AvatarUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAvatarUrl

`func (o *GitHubProfile) SetAvatarUrl(v string)`

SetAvatarUrl sets AvatarUrl field to given value.

### HasAvatarUrl

`func (o *GitHubProfile) HasAvatarUrl() bool`

HasAvatarUrl returns a boolean if a field has been set.

### SetAvatarUrlNil

`func (o *GitHubProfile) SetAvatarUrlNil(b bool)`

 SetAvatarUrlNil sets the value for AvatarUrl to be an explicit nil

### UnsetAvatarUrl
`func (o *GitHubProfile) UnsetAvatarUrl()`

UnsetAvatarUrl ensures that no value is present for AvatarUrl, not even an explicit nil
### GetBio

`func (o *GitHubProfile) GetBio() string`

GetBio returns the Bio field if non-nil, zero value otherwise.

### GetBioOk

`func (o *GitHubProfile) GetBioOk() (*string, bool)`

GetBioOk returns a tuple with the Bio field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBio

`func (o *GitHubProfile) SetBio(v string)`

SetBio sets Bio field to given value.

### HasBio

`func (o *GitHubProfile) HasBio() bool`

HasBio returns a boolean if a field has been set.

### SetBioNil

`func (o *GitHubProfile) SetBioNil(b bool)`

 SetBioNil sets the value for Bio to be an explicit nil

### UnsetBio
`func (o *GitHubProfile) UnsetBio()`

UnsetBio ensures that no value is present for Bio, not even an explicit nil
### GetDescription

`func (o *GitHubProfile) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *GitHubProfile) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *GitHubProfile) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *GitHubProfile) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *GitHubProfile) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *GitHubProfile) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetPronouns

`func (o *GitHubProfile) GetPronouns() string`

GetPronouns returns the Pronouns field if non-nil, zero value otherwise.

### GetPronounsOk

`func (o *GitHubProfile) GetPronounsOk() (*string, bool)`

GetPronounsOk returns a tuple with the Pronouns field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPronouns

`func (o *GitHubProfile) SetPronouns(v string)`

SetPronouns sets Pronouns field to given value.

### HasPronouns

`func (o *GitHubProfile) HasPronouns() bool`

HasPronouns returns a boolean if a field has been set.

### SetPronounsNil

`func (o *GitHubProfile) SetPronounsNil(b bool)`

 SetPronounsNil sets the value for Pronouns to be an explicit nil

### UnsetPronouns
`func (o *GitHubProfile) UnsetPronouns()`

UnsetPronouns ensures that no value is present for Pronouns, not even an explicit nil
### GetLocalTime

`func (o *GitHubProfile) GetLocalTime() string`

GetLocalTime returns the LocalTime field if non-nil, zero value otherwise.

### GetLocalTimeOk

`func (o *GitHubProfile) GetLocalTimeOk() (*string, bool)`

GetLocalTimeOk returns a tuple with the LocalTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocalTime

`func (o *GitHubProfile) SetLocalTime(v string)`

SetLocalTime sets LocalTime field to given value.

### HasLocalTime

`func (o *GitHubProfile) HasLocalTime() bool`

HasLocalTime returns a boolean if a field has been set.

### SetLocalTimeNil

`func (o *GitHubProfile) SetLocalTimeNil(b bool)`

 SetLocalTimeNil sets the value for LocalTime to be an explicit nil

### UnsetLocalTime
`func (o *GitHubProfile) UnsetLocalTime()`

UnsetLocalTime ensures that no value is present for LocalTime, not even an explicit nil
### GetUtcOffset

`func (o *GitHubProfile) GetUtcOffset() float32`

GetUtcOffset returns the UtcOffset field if non-nil, zero value otherwise.

### GetUtcOffsetOk

`func (o *GitHubProfile) GetUtcOffsetOk() (*float32, bool)`

GetUtcOffsetOk returns a tuple with the UtcOffset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUtcOffset

`func (o *GitHubProfile) SetUtcOffset(v float32)`

SetUtcOffset sets UtcOffset field to given value.

### HasUtcOffset

`func (o *GitHubProfile) HasUtcOffset() bool`

HasUtcOffset returns a boolean if a field has been set.

### SetUtcOffsetNil

`func (o *GitHubProfile) SetUtcOffsetNil(b bool)`

 SetUtcOffsetNil sets the value for UtcOffset to be an explicit nil

### UnsetUtcOffset
`func (o *GitHubProfile) UnsetUtcOffset()`

UnsetUtcOffset ensures that no value is present for UtcOffset, not even an explicit nil
### GetCompany

`func (o *GitHubProfile) GetCompany() string`

GetCompany returns the Company field if non-nil, zero value otherwise.

### GetCompanyOk

`func (o *GitHubProfile) GetCompanyOk() (*string, bool)`

GetCompanyOk returns a tuple with the Company field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompany

`func (o *GitHubProfile) SetCompany(v string)`

SetCompany sets Company field to given value.

### HasCompany

`func (o *GitHubProfile) HasCompany() bool`

HasCompany returns a boolean if a field has been set.

### SetCompanyNil

`func (o *GitHubProfile) SetCompanyNil(b bool)`

 SetCompanyNil sets the value for Company to be an explicit nil

### UnsetCompany
`func (o *GitHubProfile) UnsetCompany()`

UnsetCompany ensures that no value is present for Company, not even an explicit nil
### GetLocation

`func (o *GitHubProfile) GetLocation() string`

GetLocation returns the Location field if non-nil, zero value otherwise.

### GetLocationOk

`func (o *GitHubProfile) GetLocationOk() (*string, bool)`

GetLocationOk returns a tuple with the Location field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocation

`func (o *GitHubProfile) SetLocation(v string)`

SetLocation sets Location field to given value.

### HasLocation

`func (o *GitHubProfile) HasLocation() bool`

HasLocation returns a boolean if a field has been set.

### SetLocationNil

`func (o *GitHubProfile) SetLocationNil(b bool)`

 SetLocationNil sets the value for Location to be an explicit nil

### UnsetLocation
`func (o *GitHubProfile) UnsetLocation()`

UnsetLocation ensures that no value is present for Location, not even an explicit nil
### GetEmail

`func (o *GitHubProfile) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *GitHubProfile) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *GitHubProfile) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *GitHubProfile) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### SetEmailNil

`func (o *GitHubProfile) SetEmailNil(b bool)`

 SetEmailNil sets the value for Email to be an explicit nil

### UnsetEmail
`func (o *GitHubProfile) UnsetEmail()`

UnsetEmail ensures that no value is present for Email, not even an explicit nil
### GetWebsite

`func (o *GitHubProfile) GetWebsite() string`

GetWebsite returns the Website field if non-nil, zero value otherwise.

### GetWebsiteOk

`func (o *GitHubProfile) GetWebsiteOk() (*string, bool)`

GetWebsiteOk returns a tuple with the Website field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebsite

`func (o *GitHubProfile) SetWebsite(v string)`

SetWebsite sets Website field to given value.

### HasWebsite

`func (o *GitHubProfile) HasWebsite() bool`

HasWebsite returns a boolean if a field has been set.

### SetWebsiteNil

`func (o *GitHubProfile) SetWebsiteNil(b bool)`

 SetWebsiteNil sets the value for Website to be an explicit nil

### UnsetWebsite
`func (o *GitHubProfile) UnsetWebsite()`

UnsetWebsite ensures that no value is present for Website, not even an explicit nil
### GetTwitterUsername

`func (o *GitHubProfile) GetTwitterUsername() string`

GetTwitterUsername returns the TwitterUsername field if non-nil, zero value otherwise.

### GetTwitterUsernameOk

`func (o *GitHubProfile) GetTwitterUsernameOk() (*string, bool)`

GetTwitterUsernameOk returns a tuple with the TwitterUsername field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTwitterUsername

`func (o *GitHubProfile) SetTwitterUsername(v string)`

SetTwitterUsername sets TwitterUsername field to given value.

### HasTwitterUsername

`func (o *GitHubProfile) HasTwitterUsername() bool`

HasTwitterUsername returns a boolean if a field has been set.

### SetTwitterUsernameNil

`func (o *GitHubProfile) SetTwitterUsernameNil(b bool)`

 SetTwitterUsernameNil sets the value for TwitterUsername to be an explicit nil

### UnsetTwitterUsername
`func (o *GitHubProfile) UnsetTwitterUsername()`

UnsetTwitterUsername ensures that no value is present for TwitterUsername, not even an explicit nil
### GetHireable

`func (o *GitHubProfile) GetHireable() bool`

GetHireable returns the Hireable field if non-nil, zero value otherwise.

### GetHireableOk

`func (o *GitHubProfile) GetHireableOk() (*bool, bool)`

GetHireableOk returns a tuple with the Hireable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHireable

`func (o *GitHubProfile) SetHireable(v bool)`

SetHireable sets Hireable field to given value.

### HasHireable

`func (o *GitHubProfile) HasHireable() bool`

HasHireable returns a boolean if a field has been set.

### SetHireableNil

`func (o *GitHubProfile) SetHireableNil(b bool)`

 SetHireableNil sets the value for Hireable to be an explicit nil

### UnsetHireable
`func (o *GitHubProfile) UnsetHireable()`

UnsetHireable ensures that no value is present for Hireable, not even an explicit nil
### GetSocialAccounts

`func (o *GitHubProfile) GetSocialAccounts() []GitHubSocialAccount`

GetSocialAccounts returns the SocialAccounts field if non-nil, zero value otherwise.

### GetSocialAccountsOk

`func (o *GitHubProfile) GetSocialAccountsOk() (*[]GitHubSocialAccount, bool)`

GetSocialAccountsOk returns a tuple with the SocialAccounts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSocialAccounts

`func (o *GitHubProfile) SetSocialAccounts(v []GitHubSocialAccount)`

SetSocialAccounts sets SocialAccounts field to given value.

### HasSocialAccounts

`func (o *GitHubProfile) HasSocialAccounts() bool`

HasSocialAccounts returns a boolean if a field has been set.

### SetSocialAccountsNil

`func (o *GitHubProfile) SetSocialAccountsNil(b bool)`

 SetSocialAccountsNil sets the value for SocialAccounts to be an explicit nil

### UnsetSocialAccounts
`func (o *GitHubProfile) UnsetSocialAccounts()`

UnsetSocialAccounts ensures that no value is present for SocialAccounts, not even an explicit nil
### GetStatus

`func (o *GitHubProfile) GetStatus() GitHubStatus`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *GitHubProfile) GetStatusOk() (*GitHubStatus, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *GitHubProfile) SetStatus(v GitHubStatus)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *GitHubProfile) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### SetStatusNil

`func (o *GitHubProfile) SetStatusNil(b bool)`

 SetStatusNil sets the value for Status to be an explicit nil

### UnsetStatus
`func (o *GitHubProfile) UnsetStatus()`

UnsetStatus ensures that no value is present for Status, not even an explicit nil
### GetFollowers

`func (o *GitHubProfile) GetFollowers() int32`

GetFollowers returns the Followers field if non-nil, zero value otherwise.

### GetFollowersOk

`func (o *GitHubProfile) GetFollowersOk() (*int32, bool)`

GetFollowersOk returns a tuple with the Followers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFollowers

`func (o *GitHubProfile) SetFollowers(v int32)`

SetFollowers sets Followers field to given value.

### HasFollowers

`func (o *GitHubProfile) HasFollowers() bool`

HasFollowers returns a boolean if a field has been set.

### SetFollowersNil

`func (o *GitHubProfile) SetFollowersNil(b bool)`

 SetFollowersNil sets the value for Followers to be an explicit nil

### UnsetFollowers
`func (o *GitHubProfile) UnsetFollowers()`

UnsetFollowers ensures that no value is present for Followers, not even an explicit nil
### GetFollowing

`func (o *GitHubProfile) GetFollowing() int32`

GetFollowing returns the Following field if non-nil, zero value otherwise.

### GetFollowingOk

`func (o *GitHubProfile) GetFollowingOk() (*int32, bool)`

GetFollowingOk returns a tuple with the Following field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFollowing

`func (o *GitHubProfile) SetFollowing(v int32)`

SetFollowing sets Following field to given value.

### HasFollowing

`func (o *GitHubProfile) HasFollowing() bool`

HasFollowing returns a boolean if a field has been set.

### SetFollowingNil

`func (o *GitHubProfile) SetFollowingNil(b bool)`

 SetFollowingNil sets the value for Following to be an explicit nil

### UnsetFollowing
`func (o *GitHubProfile) UnsetFollowing()`

UnsetFollowing ensures that no value is present for Following, not even an explicit nil
### GetRepos

`func (o *GitHubProfile) GetRepos() int32`

GetRepos returns the Repos field if non-nil, zero value otherwise.

### GetReposOk

`func (o *GitHubProfile) GetReposOk() (*int32, bool)`

GetReposOk returns a tuple with the Repos field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRepos

`func (o *GitHubProfile) SetRepos(v int32)`

SetRepos sets Repos field to given value.

### HasRepos

`func (o *GitHubProfile) HasRepos() bool`

HasRepos returns a boolean if a field has been set.

### SetReposNil

`func (o *GitHubProfile) SetReposNil(b bool)`

 SetReposNil sets the value for Repos to be an explicit nil

### UnsetRepos
`func (o *GitHubProfile) UnsetRepos()`

UnsetRepos ensures that no value is present for Repos, not even an explicit nil
### GetPublicRepos

`func (o *GitHubProfile) GetPublicRepos() int32`

GetPublicRepos returns the PublicRepos field if non-nil, zero value otherwise.

### GetPublicReposOk

`func (o *GitHubProfile) GetPublicReposOk() (*int32, bool)`

GetPublicReposOk returns a tuple with the PublicRepos field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPublicRepos

`func (o *GitHubProfile) SetPublicRepos(v int32)`

SetPublicRepos sets PublicRepos field to given value.

### HasPublicRepos

`func (o *GitHubProfile) HasPublicRepos() bool`

HasPublicRepos returns a boolean if a field has been set.

### SetPublicReposNil

`func (o *GitHubProfile) SetPublicReposNil(b bool)`

 SetPublicReposNil sets the value for PublicRepos to be an explicit nil

### UnsetPublicRepos
`func (o *GitHubProfile) UnsetPublicRepos()`

UnsetPublicRepos ensures that no value is present for PublicRepos, not even an explicit nil
### GetPublicGists

`func (o *GitHubProfile) GetPublicGists() int32`

GetPublicGists returns the PublicGists field if non-nil, zero value otherwise.

### GetPublicGistsOk

`func (o *GitHubProfile) GetPublicGistsOk() (*int32, bool)`

GetPublicGistsOk returns a tuple with the PublicGists field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPublicGists

`func (o *GitHubProfile) SetPublicGists(v int32)`

SetPublicGists sets PublicGists field to given value.

### HasPublicGists

`func (o *GitHubProfile) HasPublicGists() bool`

HasPublicGists returns a boolean if a field has been set.

### SetPublicGistsNil

`func (o *GitHubProfile) SetPublicGistsNil(b bool)`

 SetPublicGistsNil sets the value for PublicGists to be an explicit nil

### UnsetPublicGists
`func (o *GitHubProfile) UnsetPublicGists()`

UnsetPublicGists ensures that no value is present for PublicGists, not even an explicit nil
### GetFollowersDisplayCount

`func (o *GitHubProfile) GetFollowersDisplayCount() int32`

GetFollowersDisplayCount returns the FollowersDisplayCount field if non-nil, zero value otherwise.

### GetFollowersDisplayCountOk

`func (o *GitHubProfile) GetFollowersDisplayCountOk() (*int32, bool)`

GetFollowersDisplayCountOk returns a tuple with the FollowersDisplayCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFollowersDisplayCount

`func (o *GitHubProfile) SetFollowersDisplayCount(v int32)`

SetFollowersDisplayCount sets FollowersDisplayCount field to given value.

### HasFollowersDisplayCount

`func (o *GitHubProfile) HasFollowersDisplayCount() bool`

HasFollowersDisplayCount returns a boolean if a field has been set.

### SetFollowersDisplayCountNil

`func (o *GitHubProfile) SetFollowersDisplayCountNil(b bool)`

 SetFollowersDisplayCountNil sets the value for FollowersDisplayCount to be an explicit nil

### UnsetFollowersDisplayCount
`func (o *GitHubProfile) UnsetFollowersDisplayCount()`

UnsetFollowersDisplayCount ensures that no value is present for FollowersDisplayCount, not even an explicit nil
### GetFollowingDisplayCount

`func (o *GitHubProfile) GetFollowingDisplayCount() int32`

GetFollowingDisplayCount returns the FollowingDisplayCount field if non-nil, zero value otherwise.

### GetFollowingDisplayCountOk

`func (o *GitHubProfile) GetFollowingDisplayCountOk() (*int32, bool)`

GetFollowingDisplayCountOk returns a tuple with the FollowingDisplayCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFollowingDisplayCount

`func (o *GitHubProfile) SetFollowingDisplayCount(v int32)`

SetFollowingDisplayCount sets FollowingDisplayCount field to given value.

### HasFollowingDisplayCount

`func (o *GitHubProfile) HasFollowingDisplayCount() bool`

HasFollowingDisplayCount returns a boolean if a field has been set.

### SetFollowingDisplayCountNil

`func (o *GitHubProfile) SetFollowingDisplayCountNil(b bool)`

 SetFollowingDisplayCountNil sets the value for FollowingDisplayCount to be an explicit nil

### UnsetFollowingDisplayCount
`func (o *GitHubProfile) UnsetFollowingDisplayCount()`

UnsetFollowingDisplayCount ensures that no value is present for FollowingDisplayCount, not even an explicit nil
### GetReposDisplayCount

`func (o *GitHubProfile) GetReposDisplayCount() int32`

GetReposDisplayCount returns the ReposDisplayCount field if non-nil, zero value otherwise.

### GetReposDisplayCountOk

`func (o *GitHubProfile) GetReposDisplayCountOk() (*int32, bool)`

GetReposDisplayCountOk returns a tuple with the ReposDisplayCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReposDisplayCount

`func (o *GitHubProfile) SetReposDisplayCount(v int32)`

SetReposDisplayCount sets ReposDisplayCount field to given value.

### HasReposDisplayCount

`func (o *GitHubProfile) HasReposDisplayCount() bool`

HasReposDisplayCount returns a boolean if a field has been set.

### SetReposDisplayCountNil

`func (o *GitHubProfile) SetReposDisplayCountNil(b bool)`

 SetReposDisplayCountNil sets the value for ReposDisplayCount to be an explicit nil

### UnsetReposDisplayCount
`func (o *GitHubProfile) UnsetReposDisplayCount()`

UnsetReposDisplayCount ensures that no value is present for ReposDisplayCount, not even an explicit nil
### GetFollowersApproximate

`func (o *GitHubProfile) GetFollowersApproximate() bool`

GetFollowersApproximate returns the FollowersApproximate field if non-nil, zero value otherwise.

### GetFollowersApproximateOk

`func (o *GitHubProfile) GetFollowersApproximateOk() (*bool, bool)`

GetFollowersApproximateOk returns a tuple with the FollowersApproximate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFollowersApproximate

`func (o *GitHubProfile) SetFollowersApproximate(v bool)`

SetFollowersApproximate sets FollowersApproximate field to given value.

### HasFollowersApproximate

`func (o *GitHubProfile) HasFollowersApproximate() bool`

HasFollowersApproximate returns a boolean if a field has been set.

### SetFollowersApproximateNil

`func (o *GitHubProfile) SetFollowersApproximateNil(b bool)`

 SetFollowersApproximateNil sets the value for FollowersApproximate to be an explicit nil

### UnsetFollowersApproximate
`func (o *GitHubProfile) UnsetFollowersApproximate()`

UnsetFollowersApproximate ensures that no value is present for FollowersApproximate, not even an explicit nil
### GetFollowingApproximate

`func (o *GitHubProfile) GetFollowingApproximate() bool`

GetFollowingApproximate returns the FollowingApproximate field if non-nil, zero value otherwise.

### GetFollowingApproximateOk

`func (o *GitHubProfile) GetFollowingApproximateOk() (*bool, bool)`

GetFollowingApproximateOk returns a tuple with the FollowingApproximate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFollowingApproximate

`func (o *GitHubProfile) SetFollowingApproximate(v bool)`

SetFollowingApproximate sets FollowingApproximate field to given value.

### HasFollowingApproximate

`func (o *GitHubProfile) HasFollowingApproximate() bool`

HasFollowingApproximate returns a boolean if a field has been set.

### SetFollowingApproximateNil

`func (o *GitHubProfile) SetFollowingApproximateNil(b bool)`

 SetFollowingApproximateNil sets the value for FollowingApproximate to be an explicit nil

### UnsetFollowingApproximate
`func (o *GitHubProfile) UnsetFollowingApproximate()`

UnsetFollowingApproximate ensures that no value is present for FollowingApproximate, not even an explicit nil
### GetReposApproximate

`func (o *GitHubProfile) GetReposApproximate() bool`

GetReposApproximate returns the ReposApproximate field if non-nil, zero value otherwise.

### GetReposApproximateOk

`func (o *GitHubProfile) GetReposApproximateOk() (*bool, bool)`

GetReposApproximateOk returns a tuple with the ReposApproximate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReposApproximate

`func (o *GitHubProfile) SetReposApproximate(v bool)`

SetReposApproximate sets ReposApproximate field to given value.

### HasReposApproximate

`func (o *GitHubProfile) HasReposApproximate() bool`

HasReposApproximate returns a boolean if a field has been set.

### SetReposApproximateNil

`func (o *GitHubProfile) SetReposApproximateNil(b bool)`

 SetReposApproximateNil sets the value for ReposApproximate to be an explicit nil

### UnsetReposApproximate
`func (o *GitHubProfile) UnsetReposApproximate()`

UnsetReposApproximate ensures that no value is present for ReposApproximate, not even an explicit nil
### GetStarredCount

`func (o *GitHubProfile) GetStarredCount() int32`

GetStarredCount returns the StarredCount field if non-nil, zero value otherwise.

### GetStarredCountOk

`func (o *GitHubProfile) GetStarredCountOk() (*int32, bool)`

GetStarredCountOk returns a tuple with the StarredCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStarredCount

`func (o *GitHubProfile) SetStarredCount(v int32)`

SetStarredCount sets StarredCount field to given value.

### HasStarredCount

`func (o *GitHubProfile) HasStarredCount() bool`

HasStarredCount returns a boolean if a field has been set.

### SetStarredCountNil

`func (o *GitHubProfile) SetStarredCountNil(b bool)`

 SetStarredCountNil sets the value for StarredCount to be an explicit nil

### UnsetStarredCount
`func (o *GitHubProfile) UnsetStarredCount()`

UnsetStarredCount ensures that no value is present for StarredCount, not even an explicit nil
### GetStarredCountApproximate

`func (o *GitHubProfile) GetStarredCountApproximate() bool`

GetStarredCountApproximate returns the StarredCountApproximate field if non-nil, zero value otherwise.

### GetStarredCountApproximateOk

`func (o *GitHubProfile) GetStarredCountApproximateOk() (*bool, bool)`

GetStarredCountApproximateOk returns a tuple with the StarredCountApproximate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStarredCountApproximate

`func (o *GitHubProfile) SetStarredCountApproximate(v bool)`

SetStarredCountApproximate sets StarredCountApproximate field to given value.

### HasStarredCountApproximate

`func (o *GitHubProfile) HasStarredCountApproximate() bool`

HasStarredCountApproximate returns a boolean if a field has been set.

### SetStarredCountApproximateNil

`func (o *GitHubProfile) SetStarredCountApproximateNil(b bool)`

 SetStarredCountApproximateNil sets the value for StarredCountApproximate to be an explicit nil

### UnsetStarredCountApproximate
`func (o *GitHubProfile) UnsetStarredCountApproximate()`

UnsetStarredCountApproximate ensures that no value is present for StarredCountApproximate, not even an explicit nil
### GetProjectsCount

`func (o *GitHubProfile) GetProjectsCount() int32`

GetProjectsCount returns the ProjectsCount field if non-nil, zero value otherwise.

### GetProjectsCountOk

`func (o *GitHubProfile) GetProjectsCountOk() (*int32, bool)`

GetProjectsCountOk returns a tuple with the ProjectsCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectsCount

`func (o *GitHubProfile) SetProjectsCount(v int32)`

SetProjectsCount sets ProjectsCount field to given value.

### HasProjectsCount

`func (o *GitHubProfile) HasProjectsCount() bool`

HasProjectsCount returns a boolean if a field has been set.

### SetProjectsCountNil

`func (o *GitHubProfile) SetProjectsCountNil(b bool)`

 SetProjectsCountNil sets the value for ProjectsCount to be an explicit nil

### UnsetProjectsCount
`func (o *GitHubProfile) UnsetProjectsCount()`

UnsetProjectsCount ensures that no value is present for ProjectsCount, not even an explicit nil
### GetProjectsCountApproximate

`func (o *GitHubProfile) GetProjectsCountApproximate() bool`

GetProjectsCountApproximate returns the ProjectsCountApproximate field if non-nil, zero value otherwise.

### GetProjectsCountApproximateOk

`func (o *GitHubProfile) GetProjectsCountApproximateOk() (*bool, bool)`

GetProjectsCountApproximateOk returns a tuple with the ProjectsCountApproximate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectsCountApproximate

`func (o *GitHubProfile) SetProjectsCountApproximate(v bool)`

SetProjectsCountApproximate sets ProjectsCountApproximate field to given value.

### HasProjectsCountApproximate

`func (o *GitHubProfile) HasProjectsCountApproximate() bool`

HasProjectsCountApproximate returns a boolean if a field has been set.

### SetProjectsCountApproximateNil

`func (o *GitHubProfile) SetProjectsCountApproximateNil(b bool)`

 SetProjectsCountApproximateNil sets the value for ProjectsCountApproximate to be an explicit nil

### UnsetProjectsCountApproximate
`func (o *GitHubProfile) UnsetProjectsCountApproximate()`

UnsetProjectsCountApproximate ensures that no value is present for ProjectsCountApproximate, not even an explicit nil
### GetPackagesCount

`func (o *GitHubProfile) GetPackagesCount() int32`

GetPackagesCount returns the PackagesCount field if non-nil, zero value otherwise.

### GetPackagesCountOk

`func (o *GitHubProfile) GetPackagesCountOk() (*int32, bool)`

GetPackagesCountOk returns a tuple with the PackagesCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPackagesCount

`func (o *GitHubProfile) SetPackagesCount(v int32)`

SetPackagesCount sets PackagesCount field to given value.

### HasPackagesCount

`func (o *GitHubProfile) HasPackagesCount() bool`

HasPackagesCount returns a boolean if a field has been set.

### SetPackagesCountNil

`func (o *GitHubProfile) SetPackagesCountNil(b bool)`

 SetPackagesCountNil sets the value for PackagesCount to be an explicit nil

### UnsetPackagesCount
`func (o *GitHubProfile) UnsetPackagesCount()`

UnsetPackagesCount ensures that no value is present for PackagesCount, not even an explicit nil
### GetPackagesCountApproximate

`func (o *GitHubProfile) GetPackagesCountApproximate() bool`

GetPackagesCountApproximate returns the PackagesCountApproximate field if non-nil, zero value otherwise.

### GetPackagesCountApproximateOk

`func (o *GitHubProfile) GetPackagesCountApproximateOk() (*bool, bool)`

GetPackagesCountApproximateOk returns a tuple with the PackagesCountApproximate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPackagesCountApproximate

`func (o *GitHubProfile) SetPackagesCountApproximate(v bool)`

SetPackagesCountApproximate sets PackagesCountApproximate field to given value.

### HasPackagesCountApproximate

`func (o *GitHubProfile) HasPackagesCountApproximate() bool`

HasPackagesCountApproximate returns a boolean if a field has been set.

### SetPackagesCountApproximateNil

`func (o *GitHubProfile) SetPackagesCountApproximateNil(b bool)`

 SetPackagesCountApproximateNil sets the value for PackagesCountApproximate to be an explicit nil

### UnsetPackagesCountApproximate
`func (o *GitHubProfile) UnsetPackagesCountApproximate()`

UnsetPackagesCountApproximate ensures that no value is present for PackagesCountApproximate, not even an explicit nil
### GetSponsoringCount

`func (o *GitHubProfile) GetSponsoringCount() int32`

GetSponsoringCount returns the SponsoringCount field if non-nil, zero value otherwise.

### GetSponsoringCountOk

`func (o *GitHubProfile) GetSponsoringCountOk() (*int32, bool)`

GetSponsoringCountOk returns a tuple with the SponsoringCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSponsoringCount

`func (o *GitHubProfile) SetSponsoringCount(v int32)`

SetSponsoringCount sets SponsoringCount field to given value.

### HasSponsoringCount

`func (o *GitHubProfile) HasSponsoringCount() bool`

HasSponsoringCount returns a boolean if a field has been set.

### SetSponsoringCountNil

`func (o *GitHubProfile) SetSponsoringCountNil(b bool)`

 SetSponsoringCountNil sets the value for SponsoringCount to be an explicit nil

### UnsetSponsoringCount
`func (o *GitHubProfile) UnsetSponsoringCount()`

UnsetSponsoringCount ensures that no value is present for SponsoringCount, not even an explicit nil
### GetSponsoringCountApproximate

`func (o *GitHubProfile) GetSponsoringCountApproximate() bool`

GetSponsoringCountApproximate returns the SponsoringCountApproximate field if non-nil, zero value otherwise.

### GetSponsoringCountApproximateOk

`func (o *GitHubProfile) GetSponsoringCountApproximateOk() (*bool, bool)`

GetSponsoringCountApproximateOk returns a tuple with the SponsoringCountApproximate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSponsoringCountApproximate

`func (o *GitHubProfile) SetSponsoringCountApproximate(v bool)`

SetSponsoringCountApproximate sets SponsoringCountApproximate field to given value.

### HasSponsoringCountApproximate

`func (o *GitHubProfile) HasSponsoringCountApproximate() bool`

HasSponsoringCountApproximate returns a boolean if a field has been set.

### SetSponsoringCountApproximateNil

`func (o *GitHubProfile) SetSponsoringCountApproximateNil(b bool)`

 SetSponsoringCountApproximateNil sets the value for SponsoringCountApproximate to be an explicit nil

### UnsetSponsoringCountApproximate
`func (o *GitHubProfile) UnsetSponsoringCountApproximate()`

UnsetSponsoringCountApproximate ensures that no value is present for SponsoringCountApproximate, not even an explicit nil
### GetIsSponsorable

`func (o *GitHubProfile) GetIsSponsorable() bool`

GetIsSponsorable returns the IsSponsorable field if non-nil, zero value otherwise.

### GetIsSponsorableOk

`func (o *GitHubProfile) GetIsSponsorableOk() (*bool, bool)`

GetIsSponsorableOk returns a tuple with the IsSponsorable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsSponsorable

`func (o *GitHubProfile) SetIsSponsorable(v bool)`

SetIsSponsorable sets IsSponsorable field to given value.

### HasIsSponsorable

`func (o *GitHubProfile) HasIsSponsorable() bool`

HasIsSponsorable returns a boolean if a field has been set.

### SetIsSponsorableNil

`func (o *GitHubProfile) SetIsSponsorableNil(b bool)`

 SetIsSponsorableNil sets the value for IsSponsorable to be an explicit nil

### UnsetIsSponsorable
`func (o *GitHubProfile) UnsetIsSponsorable()`

UnsetIsSponsorable ensures that no value is present for IsSponsorable, not even an explicit nil
### GetSponsorsLink

`func (o *GitHubProfile) GetSponsorsLink() string`

GetSponsorsLink returns the SponsorsLink field if non-nil, zero value otherwise.

### GetSponsorsLinkOk

`func (o *GitHubProfile) GetSponsorsLinkOk() (*string, bool)`

GetSponsorsLinkOk returns a tuple with the SponsorsLink field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSponsorsLink

`func (o *GitHubProfile) SetSponsorsLink(v string)`

SetSponsorsLink sets SponsorsLink field to given value.

### HasSponsorsLink

`func (o *GitHubProfile) HasSponsorsLink() bool`

HasSponsorsLink returns a boolean if a field has been set.

### SetSponsorsLinkNil

`func (o *GitHubProfile) SetSponsorsLinkNil(b bool)`

 SetSponsorsLinkNil sets the value for SponsorsLink to be an explicit nil

### UnsetSponsorsLink
`func (o *GitHubProfile) UnsetSponsorsLink()`

UnsetSponsorsLink ensures that no value is present for SponsorsLink, not even an explicit nil
### GetIsVerified

`func (o *GitHubProfile) GetIsVerified() bool`

GetIsVerified returns the IsVerified field if non-nil, zero value otherwise.

### GetIsVerifiedOk

`func (o *GitHubProfile) GetIsVerifiedOk() (*bool, bool)`

GetIsVerifiedOk returns a tuple with the IsVerified field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsVerified

`func (o *GitHubProfile) SetIsVerified(v bool)`

SetIsVerified sets IsVerified field to given value.

### HasIsVerified

`func (o *GitHubProfile) HasIsVerified() bool`

HasIsVerified returns a boolean if a field has been set.

### SetIsVerifiedNil

`func (o *GitHubProfile) SetIsVerifiedNil(b bool)`

 SetIsVerifiedNil sets the value for IsVerified to be an explicit nil

### UnsetIsVerified
`func (o *GitHubProfile) UnsetIsVerified()`

UnsetIsVerified ensures that no value is present for IsVerified, not even an explicit nil
### GetHasOrganizationProjects

`func (o *GitHubProfile) GetHasOrganizationProjects() bool`

GetHasOrganizationProjects returns the HasOrganizationProjects field if non-nil, zero value otherwise.

### GetHasOrganizationProjectsOk

`func (o *GitHubProfile) GetHasOrganizationProjectsOk() (*bool, bool)`

GetHasOrganizationProjectsOk returns a tuple with the HasOrganizationProjects field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasOrganizationProjects

`func (o *GitHubProfile) SetHasOrganizationProjects(v bool)`

SetHasOrganizationProjects sets HasOrganizationProjects field to given value.

### HasHasOrganizationProjects

`func (o *GitHubProfile) HasHasOrganizationProjects() bool`

HasHasOrganizationProjects returns a boolean if a field has been set.

### SetHasOrganizationProjectsNil

`func (o *GitHubProfile) SetHasOrganizationProjectsNil(b bool)`

 SetHasOrganizationProjectsNil sets the value for HasOrganizationProjects to be an explicit nil

### UnsetHasOrganizationProjects
`func (o *GitHubProfile) UnsetHasOrganizationProjects()`

UnsetHasOrganizationProjects ensures that no value is present for HasOrganizationProjects, not even an explicit nil
### GetHasRepositoryProjects

`func (o *GitHubProfile) GetHasRepositoryProjects() bool`

GetHasRepositoryProjects returns the HasRepositoryProjects field if non-nil, zero value otherwise.

### GetHasRepositoryProjectsOk

`func (o *GitHubProfile) GetHasRepositoryProjectsOk() (*bool, bool)`

GetHasRepositoryProjectsOk returns a tuple with the HasRepositoryProjects field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasRepositoryProjects

`func (o *GitHubProfile) SetHasRepositoryProjects(v bool)`

SetHasRepositoryProjects sets HasRepositoryProjects field to given value.

### HasHasRepositoryProjects

`func (o *GitHubProfile) HasHasRepositoryProjects() bool`

HasHasRepositoryProjects returns a boolean if a field has been set.

### SetHasRepositoryProjectsNil

`func (o *GitHubProfile) SetHasRepositoryProjectsNil(b bool)`

 SetHasRepositoryProjectsNil sets the value for HasRepositoryProjects to be an explicit nil

### UnsetHasRepositoryProjects
`func (o *GitHubProfile) UnsetHasRepositoryProjects()`

UnsetHasRepositoryProjects ensures that no value is present for HasRepositoryProjects, not even an explicit nil
### GetCreatedAt

`func (o *GitHubProfile) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *GitHubProfile) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *GitHubProfile) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *GitHubProfile) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### SetCreatedAtNil

`func (o *GitHubProfile) SetCreatedAtNil(b bool)`

 SetCreatedAtNil sets the value for CreatedAt to be an explicit nil

### UnsetCreatedAt
`func (o *GitHubProfile) UnsetCreatedAt()`

UnsetCreatedAt ensures that no value is present for CreatedAt, not even an explicit nil
### GetCreatedUtc

`func (o *GitHubProfile) GetCreatedUtc() float32`

GetCreatedUtc returns the CreatedUtc field if non-nil, zero value otherwise.

### GetCreatedUtcOk

`func (o *GitHubProfile) GetCreatedUtcOk() (*float32, bool)`

GetCreatedUtcOk returns a tuple with the CreatedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedUtc

`func (o *GitHubProfile) SetCreatedUtc(v float32)`

SetCreatedUtc sets CreatedUtc field to given value.

### HasCreatedUtc

`func (o *GitHubProfile) HasCreatedUtc() bool`

HasCreatedUtc returns a boolean if a field has been set.

### SetCreatedUtcNil

`func (o *GitHubProfile) SetCreatedUtcNil(b bool)`

 SetCreatedUtcNil sets the value for CreatedUtc to be an explicit nil

### UnsetCreatedUtc
`func (o *GitHubProfile) UnsetCreatedUtc()`

UnsetCreatedUtc ensures that no value is present for CreatedUtc, not even an explicit nil
### GetUpdatedAt

`func (o *GitHubProfile) GetUpdatedAt() string`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *GitHubProfile) GetUpdatedAtOk() (*string, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *GitHubProfile) SetUpdatedAt(v string)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *GitHubProfile) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.

### SetUpdatedAtNil

`func (o *GitHubProfile) SetUpdatedAtNil(b bool)`

 SetUpdatedAtNil sets the value for UpdatedAt to be an explicit nil

### UnsetUpdatedAt
`func (o *GitHubProfile) UnsetUpdatedAt()`

UnsetUpdatedAt ensures that no value is present for UpdatedAt, not even an explicit nil
### GetUpdatedUtc

`func (o *GitHubProfile) GetUpdatedUtc() float32`

GetUpdatedUtc returns the UpdatedUtc field if non-nil, zero value otherwise.

### GetUpdatedUtcOk

`func (o *GitHubProfile) GetUpdatedUtcOk() (*float32, bool)`

GetUpdatedUtcOk returns a tuple with the UpdatedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedUtc

`func (o *GitHubProfile) SetUpdatedUtc(v float32)`

SetUpdatedUtc sets UpdatedUtc field to given value.

### HasUpdatedUtc

`func (o *GitHubProfile) HasUpdatedUtc() bool`

HasUpdatedUtc returns a boolean if a field has been set.

### SetUpdatedUtcNil

`func (o *GitHubProfile) SetUpdatedUtcNil(b bool)`

 SetUpdatedUtcNil sets the value for UpdatedUtc to be an explicit nil

### UnsetUpdatedUtc
`func (o *GitHubProfile) UnsetUpdatedUtc()`

UnsetUpdatedUtc ensures that no value is present for UpdatedUtc, not even an explicit nil
### GetArchivedAt

`func (o *GitHubProfile) GetArchivedAt() string`

GetArchivedAt returns the ArchivedAt field if non-nil, zero value otherwise.

### GetArchivedAtOk

`func (o *GitHubProfile) GetArchivedAtOk() (*string, bool)`

GetArchivedAtOk returns a tuple with the ArchivedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchivedAt

`func (o *GitHubProfile) SetArchivedAt(v string)`

SetArchivedAt sets ArchivedAt field to given value.

### HasArchivedAt

`func (o *GitHubProfile) HasArchivedAt() bool`

HasArchivedAt returns a boolean if a field has been set.

### SetArchivedAtNil

`func (o *GitHubProfile) SetArchivedAtNil(b bool)`

 SetArchivedAtNil sets the value for ArchivedAt to be an explicit nil

### UnsetArchivedAt
`func (o *GitHubProfile) UnsetArchivedAt()`

UnsetArchivedAt ensures that no value is present for ArchivedAt, not even an explicit nil
### GetArchivedUtc

`func (o *GitHubProfile) GetArchivedUtc() float32`

GetArchivedUtc returns the ArchivedUtc field if non-nil, zero value otherwise.

### GetArchivedUtcOk

`func (o *GitHubProfile) GetArchivedUtcOk() (*float32, bool)`

GetArchivedUtcOk returns a tuple with the ArchivedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchivedUtc

`func (o *GitHubProfile) SetArchivedUtc(v float32)`

SetArchivedUtc sets ArchivedUtc field to given value.

### HasArchivedUtc

`func (o *GitHubProfile) HasArchivedUtc() bool`

HasArchivedUtc returns a boolean if a field has been set.

### SetArchivedUtcNil

`func (o *GitHubProfile) SetArchivedUtcNil(b bool)`

 SetArchivedUtcNil sets the value for ArchivedUtc to be an explicit nil

### UnsetArchivedUtc
`func (o *GitHubProfile) UnsetArchivedUtc()`

UnsetArchivedUtc ensures that no value is present for ArchivedUtc, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



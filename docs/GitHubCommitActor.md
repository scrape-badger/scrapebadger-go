# GitHubCommitActor

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Login** | Pointer to **NullableString** |  | [optional] 
**Name** | Pointer to **NullableString** |  | [optional] 
**ProfileName** | Pointer to **NullableString** |  | [optional] 
**Link** | Pointer to **NullableString** |  | [optional] 
**AvatarUrl** | Pointer to **NullableString** |  | [optional] 
**Id** | Pointer to **NullableInt32** |  | [optional] 
**IsGithub** | Pointer to **NullableBool** |  | [optional] 

## Methods

### NewGitHubCommitActor

`func NewGitHubCommitActor() *GitHubCommitActor`

NewGitHubCommitActor instantiates a new GitHubCommitActor object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubCommitActorWithDefaults

`func NewGitHubCommitActorWithDefaults() *GitHubCommitActor`

NewGitHubCommitActorWithDefaults instantiates a new GitHubCommitActor object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLogin

`func (o *GitHubCommitActor) GetLogin() string`

GetLogin returns the Login field if non-nil, zero value otherwise.

### GetLoginOk

`func (o *GitHubCommitActor) GetLoginOk() (*string, bool)`

GetLoginOk returns a tuple with the Login field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogin

`func (o *GitHubCommitActor) SetLogin(v string)`

SetLogin sets Login field to given value.

### HasLogin

`func (o *GitHubCommitActor) HasLogin() bool`

HasLogin returns a boolean if a field has been set.

### SetLoginNil

`func (o *GitHubCommitActor) SetLoginNil(b bool)`

 SetLoginNil sets the value for Login to be an explicit nil

### UnsetLogin
`func (o *GitHubCommitActor) UnsetLogin()`

UnsetLogin ensures that no value is present for Login, not even an explicit nil
### GetName

`func (o *GitHubCommitActor) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *GitHubCommitActor) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *GitHubCommitActor) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *GitHubCommitActor) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *GitHubCommitActor) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *GitHubCommitActor) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetProfileName

`func (o *GitHubCommitActor) GetProfileName() string`

GetProfileName returns the ProfileName field if non-nil, zero value otherwise.

### GetProfileNameOk

`func (o *GitHubCommitActor) GetProfileNameOk() (*string, bool)`

GetProfileNameOk returns a tuple with the ProfileName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProfileName

`func (o *GitHubCommitActor) SetProfileName(v string)`

SetProfileName sets ProfileName field to given value.

### HasProfileName

`func (o *GitHubCommitActor) HasProfileName() bool`

HasProfileName returns a boolean if a field has been set.

### SetProfileNameNil

`func (o *GitHubCommitActor) SetProfileNameNil(b bool)`

 SetProfileNameNil sets the value for ProfileName to be an explicit nil

### UnsetProfileName
`func (o *GitHubCommitActor) UnsetProfileName()`

UnsetProfileName ensures that no value is present for ProfileName, not even an explicit nil
### GetLink

`func (o *GitHubCommitActor) GetLink() string`

GetLink returns the Link field if non-nil, zero value otherwise.

### GetLinkOk

`func (o *GitHubCommitActor) GetLinkOk() (*string, bool)`

GetLinkOk returns a tuple with the Link field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLink

`func (o *GitHubCommitActor) SetLink(v string)`

SetLink sets Link field to given value.

### HasLink

`func (o *GitHubCommitActor) HasLink() bool`

HasLink returns a boolean if a field has been set.

### SetLinkNil

`func (o *GitHubCommitActor) SetLinkNil(b bool)`

 SetLinkNil sets the value for Link to be an explicit nil

### UnsetLink
`func (o *GitHubCommitActor) UnsetLink()`

UnsetLink ensures that no value is present for Link, not even an explicit nil
### GetAvatarUrl

`func (o *GitHubCommitActor) GetAvatarUrl() string`

GetAvatarUrl returns the AvatarUrl field if non-nil, zero value otherwise.

### GetAvatarUrlOk

`func (o *GitHubCommitActor) GetAvatarUrlOk() (*string, bool)`

GetAvatarUrlOk returns a tuple with the AvatarUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAvatarUrl

`func (o *GitHubCommitActor) SetAvatarUrl(v string)`

SetAvatarUrl sets AvatarUrl field to given value.

### HasAvatarUrl

`func (o *GitHubCommitActor) HasAvatarUrl() bool`

HasAvatarUrl returns a boolean if a field has been set.

### SetAvatarUrlNil

`func (o *GitHubCommitActor) SetAvatarUrlNil(b bool)`

 SetAvatarUrlNil sets the value for AvatarUrl to be an explicit nil

### UnsetAvatarUrl
`func (o *GitHubCommitActor) UnsetAvatarUrl()`

UnsetAvatarUrl ensures that no value is present for AvatarUrl, not even an explicit nil
### GetId

`func (o *GitHubCommitActor) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *GitHubCommitActor) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *GitHubCommitActor) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *GitHubCommitActor) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *GitHubCommitActor) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *GitHubCommitActor) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil
### GetIsGithub

`func (o *GitHubCommitActor) GetIsGithub() bool`

GetIsGithub returns the IsGithub field if non-nil, zero value otherwise.

### GetIsGithubOk

`func (o *GitHubCommitActor) GetIsGithubOk() (*bool, bool)`

GetIsGithubOk returns a tuple with the IsGithub field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsGithub

`func (o *GitHubCommitActor) SetIsGithub(v bool)`

SetIsGithub sets IsGithub field to given value.

### HasIsGithub

`func (o *GitHubCommitActor) HasIsGithub() bool`

HasIsGithub returns a boolean if a field has been set.

### SetIsGithubNil

`func (o *GitHubCommitActor) SetIsGithubNil(b bool)`

 SetIsGithubNil sets the value for IsGithub to be an explicit nil

### UnsetIsGithub
`func (o *GitHubCommitActor) UnsetIsGithub()`

UnsetIsGithub ensures that no value is present for IsGithub, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



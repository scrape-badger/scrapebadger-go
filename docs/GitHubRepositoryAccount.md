# GitHubRepositoryAccount

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Login** | **string** |  | 
**Link** | Pointer to **NullableString** |  | [optional] 
**Id** | Pointer to **NullableInt32** |  | [optional] 
**AvatarUrl** | Pointer to **NullableString** |  | [optional] 
**NodeId** | Pointer to **NullableString** |  | [optional] 
**Name** | Pointer to **NullableString** |  | [optional] 
**Type** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewGitHubRepositoryAccount

`func NewGitHubRepositoryAccount(login string, ) *GitHubRepositoryAccount`

NewGitHubRepositoryAccount instantiates a new GitHubRepositoryAccount object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubRepositoryAccountWithDefaults

`func NewGitHubRepositoryAccountWithDefaults() *GitHubRepositoryAccount`

NewGitHubRepositoryAccountWithDefaults instantiates a new GitHubRepositoryAccount object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLogin

`func (o *GitHubRepositoryAccount) GetLogin() string`

GetLogin returns the Login field if non-nil, zero value otherwise.

### GetLoginOk

`func (o *GitHubRepositoryAccount) GetLoginOk() (*string, bool)`

GetLoginOk returns a tuple with the Login field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogin

`func (o *GitHubRepositoryAccount) SetLogin(v string)`

SetLogin sets Login field to given value.


### GetLink

`func (o *GitHubRepositoryAccount) GetLink() string`

GetLink returns the Link field if non-nil, zero value otherwise.

### GetLinkOk

`func (o *GitHubRepositoryAccount) GetLinkOk() (*string, bool)`

GetLinkOk returns a tuple with the Link field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLink

`func (o *GitHubRepositoryAccount) SetLink(v string)`

SetLink sets Link field to given value.

### HasLink

`func (o *GitHubRepositoryAccount) HasLink() bool`

HasLink returns a boolean if a field has been set.

### SetLinkNil

`func (o *GitHubRepositoryAccount) SetLinkNil(b bool)`

 SetLinkNil sets the value for Link to be an explicit nil

### UnsetLink
`func (o *GitHubRepositoryAccount) UnsetLink()`

UnsetLink ensures that no value is present for Link, not even an explicit nil
### GetId

`func (o *GitHubRepositoryAccount) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *GitHubRepositoryAccount) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *GitHubRepositoryAccount) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *GitHubRepositoryAccount) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *GitHubRepositoryAccount) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *GitHubRepositoryAccount) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil
### GetAvatarUrl

`func (o *GitHubRepositoryAccount) GetAvatarUrl() string`

GetAvatarUrl returns the AvatarUrl field if non-nil, zero value otherwise.

### GetAvatarUrlOk

`func (o *GitHubRepositoryAccount) GetAvatarUrlOk() (*string, bool)`

GetAvatarUrlOk returns a tuple with the AvatarUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAvatarUrl

`func (o *GitHubRepositoryAccount) SetAvatarUrl(v string)`

SetAvatarUrl sets AvatarUrl field to given value.

### HasAvatarUrl

`func (o *GitHubRepositoryAccount) HasAvatarUrl() bool`

HasAvatarUrl returns a boolean if a field has been set.

### SetAvatarUrlNil

`func (o *GitHubRepositoryAccount) SetAvatarUrlNil(b bool)`

 SetAvatarUrlNil sets the value for AvatarUrl to be an explicit nil

### UnsetAvatarUrl
`func (o *GitHubRepositoryAccount) UnsetAvatarUrl()`

UnsetAvatarUrl ensures that no value is present for AvatarUrl, not even an explicit nil
### GetNodeId

`func (o *GitHubRepositoryAccount) GetNodeId() string`

GetNodeId returns the NodeId field if non-nil, zero value otherwise.

### GetNodeIdOk

`func (o *GitHubRepositoryAccount) GetNodeIdOk() (*string, bool)`

GetNodeIdOk returns a tuple with the NodeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNodeId

`func (o *GitHubRepositoryAccount) SetNodeId(v string)`

SetNodeId sets NodeId field to given value.

### HasNodeId

`func (o *GitHubRepositoryAccount) HasNodeId() bool`

HasNodeId returns a boolean if a field has been set.

### SetNodeIdNil

`func (o *GitHubRepositoryAccount) SetNodeIdNil(b bool)`

 SetNodeIdNil sets the value for NodeId to be an explicit nil

### UnsetNodeId
`func (o *GitHubRepositoryAccount) UnsetNodeId()`

UnsetNodeId ensures that no value is present for NodeId, not even an explicit nil
### GetName

`func (o *GitHubRepositoryAccount) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *GitHubRepositoryAccount) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *GitHubRepositoryAccount) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *GitHubRepositoryAccount) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *GitHubRepositoryAccount) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *GitHubRepositoryAccount) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetType

`func (o *GitHubRepositoryAccount) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *GitHubRepositoryAccount) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *GitHubRepositoryAccount) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *GitHubRepositoryAccount) HasType() bool`

HasType returns a boolean if a field has been set.

### SetTypeNil

`func (o *GitHubRepositoryAccount) SetTypeNil(b bool)`

 SetTypeNil sets the value for Type to be an explicit nil

### UnsetType
`func (o *GitHubRepositoryAccount) UnsetType()`

UnsetType ensures that no value is present for Type, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



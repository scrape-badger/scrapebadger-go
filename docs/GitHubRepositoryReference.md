# GitHubRepositoryReference

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**FullName** | **string** |  | 
**Link** | **string** |  | 
**Id** | Pointer to **NullableInt32** |  | [optional] 
**Owner** | Pointer to [**NullableGitHubRepositoryAccount**](GitHubRepositoryAccount.md) |  | [optional] 
**Description** | Pointer to **NullableString** |  | [optional] 
**DefaultBranch** | Pointer to **NullableString** |  | [optional] 
**Language** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewGitHubRepositoryReference

`func NewGitHubRepositoryReference(name string, fullName string, link string, ) *GitHubRepositoryReference`

NewGitHubRepositoryReference instantiates a new GitHubRepositoryReference object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubRepositoryReferenceWithDefaults

`func NewGitHubRepositoryReferenceWithDefaults() *GitHubRepositoryReference`

NewGitHubRepositoryReferenceWithDefaults instantiates a new GitHubRepositoryReference object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *GitHubRepositoryReference) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *GitHubRepositoryReference) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *GitHubRepositoryReference) SetName(v string)`

SetName sets Name field to given value.


### GetFullName

`func (o *GitHubRepositoryReference) GetFullName() string`

GetFullName returns the FullName field if non-nil, zero value otherwise.

### GetFullNameOk

`func (o *GitHubRepositoryReference) GetFullNameOk() (*string, bool)`

GetFullNameOk returns a tuple with the FullName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFullName

`func (o *GitHubRepositoryReference) SetFullName(v string)`

SetFullName sets FullName field to given value.


### GetLink

`func (o *GitHubRepositoryReference) GetLink() string`

GetLink returns the Link field if non-nil, zero value otherwise.

### GetLinkOk

`func (o *GitHubRepositoryReference) GetLinkOk() (*string, bool)`

GetLinkOk returns a tuple with the Link field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLink

`func (o *GitHubRepositoryReference) SetLink(v string)`

SetLink sets Link field to given value.


### GetId

`func (o *GitHubRepositoryReference) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *GitHubRepositoryReference) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *GitHubRepositoryReference) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *GitHubRepositoryReference) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *GitHubRepositoryReference) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *GitHubRepositoryReference) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil
### GetOwner

`func (o *GitHubRepositoryReference) GetOwner() GitHubRepositoryAccount`

GetOwner returns the Owner field if non-nil, zero value otherwise.

### GetOwnerOk

`func (o *GitHubRepositoryReference) GetOwnerOk() (*GitHubRepositoryAccount, bool)`

GetOwnerOk returns a tuple with the Owner field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOwner

`func (o *GitHubRepositoryReference) SetOwner(v GitHubRepositoryAccount)`

SetOwner sets Owner field to given value.

### HasOwner

`func (o *GitHubRepositoryReference) HasOwner() bool`

HasOwner returns a boolean if a field has been set.

### SetOwnerNil

`func (o *GitHubRepositoryReference) SetOwnerNil(b bool)`

 SetOwnerNil sets the value for Owner to be an explicit nil

### UnsetOwner
`func (o *GitHubRepositoryReference) UnsetOwner()`

UnsetOwner ensures that no value is present for Owner, not even an explicit nil
### GetDescription

`func (o *GitHubRepositoryReference) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *GitHubRepositoryReference) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *GitHubRepositoryReference) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *GitHubRepositoryReference) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *GitHubRepositoryReference) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *GitHubRepositoryReference) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetDefaultBranch

`func (o *GitHubRepositoryReference) GetDefaultBranch() string`

GetDefaultBranch returns the DefaultBranch field if non-nil, zero value otherwise.

### GetDefaultBranchOk

`func (o *GitHubRepositoryReference) GetDefaultBranchOk() (*string, bool)`

GetDefaultBranchOk returns a tuple with the DefaultBranch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultBranch

`func (o *GitHubRepositoryReference) SetDefaultBranch(v string)`

SetDefaultBranch sets DefaultBranch field to given value.

### HasDefaultBranch

`func (o *GitHubRepositoryReference) HasDefaultBranch() bool`

HasDefaultBranch returns a boolean if a field has been set.

### SetDefaultBranchNil

`func (o *GitHubRepositoryReference) SetDefaultBranchNil(b bool)`

 SetDefaultBranchNil sets the value for DefaultBranch to be an explicit nil

### UnsetDefaultBranch
`func (o *GitHubRepositoryReference) UnsetDefaultBranch()`

UnsetDefaultBranch ensures that no value is present for DefaultBranch, not even an explicit nil
### GetLanguage

`func (o *GitHubRepositoryReference) GetLanguage() string`

GetLanguage returns the Language field if non-nil, zero value otherwise.

### GetLanguageOk

`func (o *GitHubRepositoryReference) GetLanguageOk() (*string, bool)`

GetLanguageOk returns a tuple with the Language field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLanguage

`func (o *GitHubRepositoryReference) SetLanguage(v string)`

SetLanguage sets Language field to given value.

### HasLanguage

`func (o *GitHubRepositoryReference) HasLanguage() bool`

HasLanguage returns a boolean if a field has been set.

### SetLanguageNil

`func (o *GitHubRepositoryReference) SetLanguageNil(b bool)`

 SetLanguageNil sets the value for Language to be an explicit nil

### UnsetLanguage
`func (o *GitHubRepositoryReference) UnsetLanguage()`

UnsetLanguage ensures that no value is present for Language, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



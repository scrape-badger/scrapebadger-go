# GitHubSocialAccount

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Provider** | **string** |  | 
**Link** | **string** |  | 
**Label** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewGitHubSocialAccount

`func NewGitHubSocialAccount(provider string, link string, ) *GitHubSocialAccount`

NewGitHubSocialAccount instantiates a new GitHubSocialAccount object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubSocialAccountWithDefaults

`func NewGitHubSocialAccountWithDefaults() *GitHubSocialAccount`

NewGitHubSocialAccountWithDefaults instantiates a new GitHubSocialAccount object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProvider

`func (o *GitHubSocialAccount) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *GitHubSocialAccount) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *GitHubSocialAccount) SetProvider(v string)`

SetProvider sets Provider field to given value.


### GetLink

`func (o *GitHubSocialAccount) GetLink() string`

GetLink returns the Link field if non-nil, zero value otherwise.

### GetLinkOk

`func (o *GitHubSocialAccount) GetLinkOk() (*string, bool)`

GetLinkOk returns a tuple with the Link field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLink

`func (o *GitHubSocialAccount) SetLink(v string)`

SetLink sets Link field to given value.


### GetLabel

`func (o *GitHubSocialAccount) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *GitHubSocialAccount) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *GitHubSocialAccount) SetLabel(v string)`

SetLabel sets Label field to given value.

### HasLabel

`func (o *GitHubSocialAccount) HasLabel() bool`

HasLabel returns a boolean if a field has been set.

### SetLabelNil

`func (o *GitHubSocialAccount) SetLabelNil(b bool)`

 SetLabelNil sets the value for Label to be an explicit nil

### UnsetLabel
`func (o *GitHubSocialAccount) UnsetLabel()`

UnsetLabel ensures that no value is present for Label, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



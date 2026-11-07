# GitHubLatestCommit

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Sha** | **string** |  | 
**Link** | **string** |  | 
**Message** | **string** |  | 
**MessageHtml** | Pointer to **NullableString** |  | [optional] 
**Body** | Pointer to **NullableString** |  | [optional] 
**BodyHtml** | Pointer to **NullableString** |  | [optional] 
**CommittedAt** | Pointer to **NullableString** |  | [optional] 
**CommittedUtc** | Pointer to **NullableFloat32** |  | [optional] 
**PushedAt** | Pointer to **NullableString** |  | [optional] 
**PushedUtc** | Pointer to **NullableFloat32** |  | [optional] 
**Authors** | Pointer to [**[]GitHubCommitActor**](GitHubCommitActor.md) |  | [optional] 
**Committer** | Pointer to [**NullableGitHubCommitActor**](GitHubCommitActor.md) |  | [optional] 
**Pusher** | Pointer to [**NullableGitHubCommitActor**](GitHubCommitActor.md) |  | [optional] 
**Checks** | Pointer to [**NullableGitHubCommitChecks**](GitHubCommitChecks.md) |  | [optional] 
**IsSpoofed** | Pointer to **NullableBool** |  | [optional] 

## Methods

### NewGitHubLatestCommit

`func NewGitHubLatestCommit(sha string, link string, message string, ) *GitHubLatestCommit`

NewGitHubLatestCommit instantiates a new GitHubLatestCommit object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubLatestCommitWithDefaults

`func NewGitHubLatestCommitWithDefaults() *GitHubLatestCommit`

NewGitHubLatestCommitWithDefaults instantiates a new GitHubLatestCommit object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSha

`func (o *GitHubLatestCommit) GetSha() string`

GetSha returns the Sha field if non-nil, zero value otherwise.

### GetShaOk

`func (o *GitHubLatestCommit) GetShaOk() (*string, bool)`

GetShaOk returns a tuple with the Sha field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSha

`func (o *GitHubLatestCommit) SetSha(v string)`

SetSha sets Sha field to given value.


### GetLink

`func (o *GitHubLatestCommit) GetLink() string`

GetLink returns the Link field if non-nil, zero value otherwise.

### GetLinkOk

`func (o *GitHubLatestCommit) GetLinkOk() (*string, bool)`

GetLinkOk returns a tuple with the Link field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLink

`func (o *GitHubLatestCommit) SetLink(v string)`

SetLink sets Link field to given value.


### GetMessage

`func (o *GitHubLatestCommit) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *GitHubLatestCommit) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *GitHubLatestCommit) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetMessageHtml

`func (o *GitHubLatestCommit) GetMessageHtml() string`

GetMessageHtml returns the MessageHtml field if non-nil, zero value otherwise.

### GetMessageHtmlOk

`func (o *GitHubLatestCommit) GetMessageHtmlOk() (*string, bool)`

GetMessageHtmlOk returns a tuple with the MessageHtml field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageHtml

`func (o *GitHubLatestCommit) SetMessageHtml(v string)`

SetMessageHtml sets MessageHtml field to given value.

### HasMessageHtml

`func (o *GitHubLatestCommit) HasMessageHtml() bool`

HasMessageHtml returns a boolean if a field has been set.

### SetMessageHtmlNil

`func (o *GitHubLatestCommit) SetMessageHtmlNil(b bool)`

 SetMessageHtmlNil sets the value for MessageHtml to be an explicit nil

### UnsetMessageHtml
`func (o *GitHubLatestCommit) UnsetMessageHtml()`

UnsetMessageHtml ensures that no value is present for MessageHtml, not even an explicit nil
### GetBody

`func (o *GitHubLatestCommit) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *GitHubLatestCommit) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *GitHubLatestCommit) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *GitHubLatestCommit) HasBody() bool`

HasBody returns a boolean if a field has been set.

### SetBodyNil

`func (o *GitHubLatestCommit) SetBodyNil(b bool)`

 SetBodyNil sets the value for Body to be an explicit nil

### UnsetBody
`func (o *GitHubLatestCommit) UnsetBody()`

UnsetBody ensures that no value is present for Body, not even an explicit nil
### GetBodyHtml

`func (o *GitHubLatestCommit) GetBodyHtml() string`

GetBodyHtml returns the BodyHtml field if non-nil, zero value otherwise.

### GetBodyHtmlOk

`func (o *GitHubLatestCommit) GetBodyHtmlOk() (*string, bool)`

GetBodyHtmlOk returns a tuple with the BodyHtml field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBodyHtml

`func (o *GitHubLatestCommit) SetBodyHtml(v string)`

SetBodyHtml sets BodyHtml field to given value.

### HasBodyHtml

`func (o *GitHubLatestCommit) HasBodyHtml() bool`

HasBodyHtml returns a boolean if a field has been set.

### SetBodyHtmlNil

`func (o *GitHubLatestCommit) SetBodyHtmlNil(b bool)`

 SetBodyHtmlNil sets the value for BodyHtml to be an explicit nil

### UnsetBodyHtml
`func (o *GitHubLatestCommit) UnsetBodyHtml()`

UnsetBodyHtml ensures that no value is present for BodyHtml, not even an explicit nil
### GetCommittedAt

`func (o *GitHubLatestCommit) GetCommittedAt() string`

GetCommittedAt returns the CommittedAt field if non-nil, zero value otherwise.

### GetCommittedAtOk

`func (o *GitHubLatestCommit) GetCommittedAtOk() (*string, bool)`

GetCommittedAtOk returns a tuple with the CommittedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommittedAt

`func (o *GitHubLatestCommit) SetCommittedAt(v string)`

SetCommittedAt sets CommittedAt field to given value.

### HasCommittedAt

`func (o *GitHubLatestCommit) HasCommittedAt() bool`

HasCommittedAt returns a boolean if a field has been set.

### SetCommittedAtNil

`func (o *GitHubLatestCommit) SetCommittedAtNil(b bool)`

 SetCommittedAtNil sets the value for CommittedAt to be an explicit nil

### UnsetCommittedAt
`func (o *GitHubLatestCommit) UnsetCommittedAt()`

UnsetCommittedAt ensures that no value is present for CommittedAt, not even an explicit nil
### GetCommittedUtc

`func (o *GitHubLatestCommit) GetCommittedUtc() float32`

GetCommittedUtc returns the CommittedUtc field if non-nil, zero value otherwise.

### GetCommittedUtcOk

`func (o *GitHubLatestCommit) GetCommittedUtcOk() (*float32, bool)`

GetCommittedUtcOk returns a tuple with the CommittedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommittedUtc

`func (o *GitHubLatestCommit) SetCommittedUtc(v float32)`

SetCommittedUtc sets CommittedUtc field to given value.

### HasCommittedUtc

`func (o *GitHubLatestCommit) HasCommittedUtc() bool`

HasCommittedUtc returns a boolean if a field has been set.

### SetCommittedUtcNil

`func (o *GitHubLatestCommit) SetCommittedUtcNil(b bool)`

 SetCommittedUtcNil sets the value for CommittedUtc to be an explicit nil

### UnsetCommittedUtc
`func (o *GitHubLatestCommit) UnsetCommittedUtc()`

UnsetCommittedUtc ensures that no value is present for CommittedUtc, not even an explicit nil
### GetPushedAt

`func (o *GitHubLatestCommit) GetPushedAt() string`

GetPushedAt returns the PushedAt field if non-nil, zero value otherwise.

### GetPushedAtOk

`func (o *GitHubLatestCommit) GetPushedAtOk() (*string, bool)`

GetPushedAtOk returns a tuple with the PushedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPushedAt

`func (o *GitHubLatestCommit) SetPushedAt(v string)`

SetPushedAt sets PushedAt field to given value.

### HasPushedAt

`func (o *GitHubLatestCommit) HasPushedAt() bool`

HasPushedAt returns a boolean if a field has been set.

### SetPushedAtNil

`func (o *GitHubLatestCommit) SetPushedAtNil(b bool)`

 SetPushedAtNil sets the value for PushedAt to be an explicit nil

### UnsetPushedAt
`func (o *GitHubLatestCommit) UnsetPushedAt()`

UnsetPushedAt ensures that no value is present for PushedAt, not even an explicit nil
### GetPushedUtc

`func (o *GitHubLatestCommit) GetPushedUtc() float32`

GetPushedUtc returns the PushedUtc field if non-nil, zero value otherwise.

### GetPushedUtcOk

`func (o *GitHubLatestCommit) GetPushedUtcOk() (*float32, bool)`

GetPushedUtcOk returns a tuple with the PushedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPushedUtc

`func (o *GitHubLatestCommit) SetPushedUtc(v float32)`

SetPushedUtc sets PushedUtc field to given value.

### HasPushedUtc

`func (o *GitHubLatestCommit) HasPushedUtc() bool`

HasPushedUtc returns a boolean if a field has been set.

### SetPushedUtcNil

`func (o *GitHubLatestCommit) SetPushedUtcNil(b bool)`

 SetPushedUtcNil sets the value for PushedUtc to be an explicit nil

### UnsetPushedUtc
`func (o *GitHubLatestCommit) UnsetPushedUtc()`

UnsetPushedUtc ensures that no value is present for PushedUtc, not even an explicit nil
### GetAuthors

`func (o *GitHubLatestCommit) GetAuthors() []GitHubCommitActor`

GetAuthors returns the Authors field if non-nil, zero value otherwise.

### GetAuthorsOk

`func (o *GitHubLatestCommit) GetAuthorsOk() (*[]GitHubCommitActor, bool)`

GetAuthorsOk returns a tuple with the Authors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthors

`func (o *GitHubLatestCommit) SetAuthors(v []GitHubCommitActor)`

SetAuthors sets Authors field to given value.

### HasAuthors

`func (o *GitHubLatestCommit) HasAuthors() bool`

HasAuthors returns a boolean if a field has been set.

### SetAuthorsNil

`func (o *GitHubLatestCommit) SetAuthorsNil(b bool)`

 SetAuthorsNil sets the value for Authors to be an explicit nil

### UnsetAuthors
`func (o *GitHubLatestCommit) UnsetAuthors()`

UnsetAuthors ensures that no value is present for Authors, not even an explicit nil
### GetCommitter

`func (o *GitHubLatestCommit) GetCommitter() GitHubCommitActor`

GetCommitter returns the Committer field if non-nil, zero value otherwise.

### GetCommitterOk

`func (o *GitHubLatestCommit) GetCommitterOk() (*GitHubCommitActor, bool)`

GetCommitterOk returns a tuple with the Committer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommitter

`func (o *GitHubLatestCommit) SetCommitter(v GitHubCommitActor)`

SetCommitter sets Committer field to given value.

### HasCommitter

`func (o *GitHubLatestCommit) HasCommitter() bool`

HasCommitter returns a boolean if a field has been set.

### SetCommitterNil

`func (o *GitHubLatestCommit) SetCommitterNil(b bool)`

 SetCommitterNil sets the value for Committer to be an explicit nil

### UnsetCommitter
`func (o *GitHubLatestCommit) UnsetCommitter()`

UnsetCommitter ensures that no value is present for Committer, not even an explicit nil
### GetPusher

`func (o *GitHubLatestCommit) GetPusher() GitHubCommitActor`

GetPusher returns the Pusher field if non-nil, zero value otherwise.

### GetPusherOk

`func (o *GitHubLatestCommit) GetPusherOk() (*GitHubCommitActor, bool)`

GetPusherOk returns a tuple with the Pusher field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPusher

`func (o *GitHubLatestCommit) SetPusher(v GitHubCommitActor)`

SetPusher sets Pusher field to given value.

### HasPusher

`func (o *GitHubLatestCommit) HasPusher() bool`

HasPusher returns a boolean if a field has been set.

### SetPusherNil

`func (o *GitHubLatestCommit) SetPusherNil(b bool)`

 SetPusherNil sets the value for Pusher to be an explicit nil

### UnsetPusher
`func (o *GitHubLatestCommit) UnsetPusher()`

UnsetPusher ensures that no value is present for Pusher, not even an explicit nil
### GetChecks

`func (o *GitHubLatestCommit) GetChecks() GitHubCommitChecks`

GetChecks returns the Checks field if non-nil, zero value otherwise.

### GetChecksOk

`func (o *GitHubLatestCommit) GetChecksOk() (*GitHubCommitChecks, bool)`

GetChecksOk returns a tuple with the Checks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChecks

`func (o *GitHubLatestCommit) SetChecks(v GitHubCommitChecks)`

SetChecks sets Checks field to given value.

### HasChecks

`func (o *GitHubLatestCommit) HasChecks() bool`

HasChecks returns a boolean if a field has been set.

### SetChecksNil

`func (o *GitHubLatestCommit) SetChecksNil(b bool)`

 SetChecksNil sets the value for Checks to be an explicit nil

### UnsetChecks
`func (o *GitHubLatestCommit) UnsetChecks()`

UnsetChecks ensures that no value is present for Checks, not even an explicit nil
### GetIsSpoofed

`func (o *GitHubLatestCommit) GetIsSpoofed() bool`

GetIsSpoofed returns the IsSpoofed field if non-nil, zero value otherwise.

### GetIsSpoofedOk

`func (o *GitHubLatestCommit) GetIsSpoofedOk() (*bool, bool)`

GetIsSpoofedOk returns a tuple with the IsSpoofed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsSpoofed

`func (o *GitHubLatestCommit) SetIsSpoofed(v bool)`

SetIsSpoofed sets IsSpoofed field to given value.

### HasIsSpoofed

`func (o *GitHubLatestCommit) HasIsSpoofed() bool`

HasIsSpoofed returns a boolean if a field has been set.

### SetIsSpoofedNil

`func (o *GitHubLatestCommit) SetIsSpoofedNil(b bool)`

 SetIsSpoofedNil sets the value for IsSpoofed to be an explicit nil

### UnsetIsSpoofed
`func (o *GitHubLatestCommit) UnsetIsSpoofed()`

UnsetIsSpoofed ensures that no value is present for IsSpoofed, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



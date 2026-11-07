# GitHubContributions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Total** | **int32** |  | 
**Calendar** | [**[]GitHubCalendarDay**](GitHubCalendarDay.md) |  | 
**From** | **string** |  | 
**To** | **string** |  | 
**ActivityOverview** | Pointer to [**NullableGitHubActivityOverview**](GitHubActivityOverview.md) |  | [optional] 
**Activity** | Pointer to [**[]GitHubActivityBlock**](GitHubActivityBlock.md) |  | [optional] 
**PrivateContributions** | Pointer to **NullableInt32** |  | [optional] 
**ActivityFrom** | Pointer to **NullableString** |  | [optional] 
**ActivityTo** | Pointer to **NullableString** |  | [optional] 
**PreviousActivityUrl** | Pointer to **NullableString** |  | [optional] 
**Years** | Pointer to **[]int32** |  | [optional] 

## Methods

### NewGitHubContributions

`func NewGitHubContributions(total int32, calendar []GitHubCalendarDay, from string, to string, ) *GitHubContributions`

NewGitHubContributions instantiates a new GitHubContributions object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubContributionsWithDefaults

`func NewGitHubContributionsWithDefaults() *GitHubContributions`

NewGitHubContributionsWithDefaults instantiates a new GitHubContributions object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotal

`func (o *GitHubContributions) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *GitHubContributions) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *GitHubContributions) SetTotal(v int32)`

SetTotal sets Total field to given value.


### GetCalendar

`func (o *GitHubContributions) GetCalendar() []GitHubCalendarDay`

GetCalendar returns the Calendar field if non-nil, zero value otherwise.

### GetCalendarOk

`func (o *GitHubContributions) GetCalendarOk() (*[]GitHubCalendarDay, bool)`

GetCalendarOk returns a tuple with the Calendar field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCalendar

`func (o *GitHubContributions) SetCalendar(v []GitHubCalendarDay)`

SetCalendar sets Calendar field to given value.


### GetFrom

`func (o *GitHubContributions) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *GitHubContributions) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *GitHubContributions) SetFrom(v string)`

SetFrom sets From field to given value.


### GetTo

`func (o *GitHubContributions) GetTo() string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *GitHubContributions) GetToOk() (*string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *GitHubContributions) SetTo(v string)`

SetTo sets To field to given value.


### GetActivityOverview

`func (o *GitHubContributions) GetActivityOverview() GitHubActivityOverview`

GetActivityOverview returns the ActivityOverview field if non-nil, zero value otherwise.

### GetActivityOverviewOk

`func (o *GitHubContributions) GetActivityOverviewOk() (*GitHubActivityOverview, bool)`

GetActivityOverviewOk returns a tuple with the ActivityOverview field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActivityOverview

`func (o *GitHubContributions) SetActivityOverview(v GitHubActivityOverview)`

SetActivityOverview sets ActivityOverview field to given value.

### HasActivityOverview

`func (o *GitHubContributions) HasActivityOverview() bool`

HasActivityOverview returns a boolean if a field has been set.

### SetActivityOverviewNil

`func (o *GitHubContributions) SetActivityOverviewNil(b bool)`

 SetActivityOverviewNil sets the value for ActivityOverview to be an explicit nil

### UnsetActivityOverview
`func (o *GitHubContributions) UnsetActivityOverview()`

UnsetActivityOverview ensures that no value is present for ActivityOverview, not even an explicit nil
### GetActivity

`func (o *GitHubContributions) GetActivity() []GitHubActivityBlock`

GetActivity returns the Activity field if non-nil, zero value otherwise.

### GetActivityOk

`func (o *GitHubContributions) GetActivityOk() (*[]GitHubActivityBlock, bool)`

GetActivityOk returns a tuple with the Activity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActivity

`func (o *GitHubContributions) SetActivity(v []GitHubActivityBlock)`

SetActivity sets Activity field to given value.

### HasActivity

`func (o *GitHubContributions) HasActivity() bool`

HasActivity returns a boolean if a field has been set.

### SetActivityNil

`func (o *GitHubContributions) SetActivityNil(b bool)`

 SetActivityNil sets the value for Activity to be an explicit nil

### UnsetActivity
`func (o *GitHubContributions) UnsetActivity()`

UnsetActivity ensures that no value is present for Activity, not even an explicit nil
### GetPrivateContributions

`func (o *GitHubContributions) GetPrivateContributions() int32`

GetPrivateContributions returns the PrivateContributions field if non-nil, zero value otherwise.

### GetPrivateContributionsOk

`func (o *GitHubContributions) GetPrivateContributionsOk() (*int32, bool)`

GetPrivateContributionsOk returns a tuple with the PrivateContributions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrivateContributions

`func (o *GitHubContributions) SetPrivateContributions(v int32)`

SetPrivateContributions sets PrivateContributions field to given value.

### HasPrivateContributions

`func (o *GitHubContributions) HasPrivateContributions() bool`

HasPrivateContributions returns a boolean if a field has been set.

### SetPrivateContributionsNil

`func (o *GitHubContributions) SetPrivateContributionsNil(b bool)`

 SetPrivateContributionsNil sets the value for PrivateContributions to be an explicit nil

### UnsetPrivateContributions
`func (o *GitHubContributions) UnsetPrivateContributions()`

UnsetPrivateContributions ensures that no value is present for PrivateContributions, not even an explicit nil
### GetActivityFrom

`func (o *GitHubContributions) GetActivityFrom() string`

GetActivityFrom returns the ActivityFrom field if non-nil, zero value otherwise.

### GetActivityFromOk

`func (o *GitHubContributions) GetActivityFromOk() (*string, bool)`

GetActivityFromOk returns a tuple with the ActivityFrom field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActivityFrom

`func (o *GitHubContributions) SetActivityFrom(v string)`

SetActivityFrom sets ActivityFrom field to given value.

### HasActivityFrom

`func (o *GitHubContributions) HasActivityFrom() bool`

HasActivityFrom returns a boolean if a field has been set.

### SetActivityFromNil

`func (o *GitHubContributions) SetActivityFromNil(b bool)`

 SetActivityFromNil sets the value for ActivityFrom to be an explicit nil

### UnsetActivityFrom
`func (o *GitHubContributions) UnsetActivityFrom()`

UnsetActivityFrom ensures that no value is present for ActivityFrom, not even an explicit nil
### GetActivityTo

`func (o *GitHubContributions) GetActivityTo() string`

GetActivityTo returns the ActivityTo field if non-nil, zero value otherwise.

### GetActivityToOk

`func (o *GitHubContributions) GetActivityToOk() (*string, bool)`

GetActivityToOk returns a tuple with the ActivityTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActivityTo

`func (o *GitHubContributions) SetActivityTo(v string)`

SetActivityTo sets ActivityTo field to given value.

### HasActivityTo

`func (o *GitHubContributions) HasActivityTo() bool`

HasActivityTo returns a boolean if a field has been set.

### SetActivityToNil

`func (o *GitHubContributions) SetActivityToNil(b bool)`

 SetActivityToNil sets the value for ActivityTo to be an explicit nil

### UnsetActivityTo
`func (o *GitHubContributions) UnsetActivityTo()`

UnsetActivityTo ensures that no value is present for ActivityTo, not even an explicit nil
### GetPreviousActivityUrl

`func (o *GitHubContributions) GetPreviousActivityUrl() string`

GetPreviousActivityUrl returns the PreviousActivityUrl field if non-nil, zero value otherwise.

### GetPreviousActivityUrlOk

`func (o *GitHubContributions) GetPreviousActivityUrlOk() (*string, bool)`

GetPreviousActivityUrlOk returns a tuple with the PreviousActivityUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPreviousActivityUrl

`func (o *GitHubContributions) SetPreviousActivityUrl(v string)`

SetPreviousActivityUrl sets PreviousActivityUrl field to given value.

### HasPreviousActivityUrl

`func (o *GitHubContributions) HasPreviousActivityUrl() bool`

HasPreviousActivityUrl returns a boolean if a field has been set.

### SetPreviousActivityUrlNil

`func (o *GitHubContributions) SetPreviousActivityUrlNil(b bool)`

 SetPreviousActivityUrlNil sets the value for PreviousActivityUrl to be an explicit nil

### UnsetPreviousActivityUrl
`func (o *GitHubContributions) UnsetPreviousActivityUrl()`

UnsetPreviousActivityUrl ensures that no value is present for PreviousActivityUrl, not even an explicit nil
### GetYears

`func (o *GitHubContributions) GetYears() []int32`

GetYears returns the Years field if non-nil, zero value otherwise.

### GetYearsOk

`func (o *GitHubContributions) GetYearsOk() (*[]int32, bool)`

GetYearsOk returns a tuple with the Years field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetYears

`func (o *GitHubContributions) SetYears(v []int32)`

SetYears sets Years field to given value.

### HasYears

`func (o *GitHubContributions) HasYears() bool`

HasYears returns a boolean if a field has been set.

### SetYearsNil

`func (o *GitHubContributions) SetYearsNil(b bool)`

 SetYearsNil sets the value for Years to be an explicit nil

### UnsetYears
`func (o *GitHubContributions) UnsetYears()`

UnsetYears ensures that no value is present for Years, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



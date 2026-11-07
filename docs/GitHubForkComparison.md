# GitHubForkComparison

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Ahead** | **int32** |  | 
**Behind** | **int32** |  | 
**BaseBranch** | **string** |  | 
**CurrentRef** | **string** |  | 
**IsTrackingBranch** | Pointer to **NullableBool** |  | [optional] 

## Methods

### NewGitHubForkComparison

`func NewGitHubForkComparison(ahead int32, behind int32, baseBranch string, currentRef string, ) *GitHubForkComparison`

NewGitHubForkComparison instantiates a new GitHubForkComparison object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGitHubForkComparisonWithDefaults

`func NewGitHubForkComparisonWithDefaults() *GitHubForkComparison`

NewGitHubForkComparisonWithDefaults instantiates a new GitHubForkComparison object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAhead

`func (o *GitHubForkComparison) GetAhead() int32`

GetAhead returns the Ahead field if non-nil, zero value otherwise.

### GetAheadOk

`func (o *GitHubForkComparison) GetAheadOk() (*int32, bool)`

GetAheadOk returns a tuple with the Ahead field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAhead

`func (o *GitHubForkComparison) SetAhead(v int32)`

SetAhead sets Ahead field to given value.


### GetBehind

`func (o *GitHubForkComparison) GetBehind() int32`

GetBehind returns the Behind field if non-nil, zero value otherwise.

### GetBehindOk

`func (o *GitHubForkComparison) GetBehindOk() (*int32, bool)`

GetBehindOk returns a tuple with the Behind field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBehind

`func (o *GitHubForkComparison) SetBehind(v int32)`

SetBehind sets Behind field to given value.


### GetBaseBranch

`func (o *GitHubForkComparison) GetBaseBranch() string`

GetBaseBranch returns the BaseBranch field if non-nil, zero value otherwise.

### GetBaseBranchOk

`func (o *GitHubForkComparison) GetBaseBranchOk() (*string, bool)`

GetBaseBranchOk returns a tuple with the BaseBranch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBaseBranch

`func (o *GitHubForkComparison) SetBaseBranch(v string)`

SetBaseBranch sets BaseBranch field to given value.


### GetCurrentRef

`func (o *GitHubForkComparison) GetCurrentRef() string`

GetCurrentRef returns the CurrentRef field if non-nil, zero value otherwise.

### GetCurrentRefOk

`func (o *GitHubForkComparison) GetCurrentRefOk() (*string, bool)`

GetCurrentRefOk returns a tuple with the CurrentRef field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrentRef

`func (o *GitHubForkComparison) SetCurrentRef(v string)`

SetCurrentRef sets CurrentRef field to given value.


### GetIsTrackingBranch

`func (o *GitHubForkComparison) GetIsTrackingBranch() bool`

GetIsTrackingBranch returns the IsTrackingBranch field if non-nil, zero value otherwise.

### GetIsTrackingBranchOk

`func (o *GitHubForkComparison) GetIsTrackingBranchOk() (*bool, bool)`

GetIsTrackingBranchOk returns a tuple with the IsTrackingBranch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsTrackingBranch

`func (o *GitHubForkComparison) SetIsTrackingBranch(v bool)`

SetIsTrackingBranch sets IsTrackingBranch field to given value.

### HasIsTrackingBranch

`func (o *GitHubForkComparison) HasIsTrackingBranch() bool`

HasIsTrackingBranch returns a boolean if a field has been set.

### SetIsTrackingBranchNil

`func (o *GitHubForkComparison) SetIsTrackingBranchNil(b bool)`

 SetIsTrackingBranchNil sets the value for IsTrackingBranch to be an explicit nil

### UnsetIsTrackingBranch
`func (o *GitHubForkComparison) UnsetIsTrackingBranch()`

UnsetIsTrackingBranch ensures that no value is present for IsTrackingBranch, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



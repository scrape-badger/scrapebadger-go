# AgentTrialInfo

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CreditsRemaining** | **int32** |  | 
**ExpiresAt** | Pointer to **NullableTime** |  | [optional] 
**ClaimUrl** | **string** |  | 

## Methods

### NewAgentTrialInfo

`func NewAgentTrialInfo(creditsRemaining int32, claimUrl string, ) *AgentTrialInfo`

NewAgentTrialInfo instantiates a new AgentTrialInfo object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAgentTrialInfoWithDefaults

`func NewAgentTrialInfoWithDefaults() *AgentTrialInfo`

NewAgentTrialInfoWithDefaults instantiates a new AgentTrialInfo object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCreditsRemaining

`func (o *AgentTrialInfo) GetCreditsRemaining() int32`

GetCreditsRemaining returns the CreditsRemaining field if non-nil, zero value otherwise.

### GetCreditsRemainingOk

`func (o *AgentTrialInfo) GetCreditsRemainingOk() (*int32, bool)`

GetCreditsRemainingOk returns a tuple with the CreditsRemaining field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreditsRemaining

`func (o *AgentTrialInfo) SetCreditsRemaining(v int32)`

SetCreditsRemaining sets CreditsRemaining field to given value.


### GetExpiresAt

`func (o *AgentTrialInfo) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *AgentTrialInfo) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *AgentTrialInfo) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *AgentTrialInfo) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### SetExpiresAtNil

`func (o *AgentTrialInfo) SetExpiresAtNil(b bool)`

 SetExpiresAtNil sets the value for ExpiresAt to be an explicit nil

### UnsetExpiresAt
`func (o *AgentTrialInfo) UnsetExpiresAt()`

UnsetExpiresAt ensures that no value is present for ExpiresAt, not even an explicit nil
### GetClaimUrl

`func (o *AgentTrialInfo) GetClaimUrl() string`

GetClaimUrl returns the ClaimUrl field if non-nil, zero value otherwise.

### GetClaimUrlOk

`func (o *AgentTrialInfo) GetClaimUrlOk() (*string, bool)`

GetClaimUrlOk returns a tuple with the ClaimUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClaimUrl

`func (o *AgentTrialInfo) SetClaimUrl(v string)`

SetClaimUrl sets ClaimUrl field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



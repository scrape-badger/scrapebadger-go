# UserProfileResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**User** | [**VintedUserProfile**](VintedUserProfile.md) |  | 
**Market** | **string** |  | 

## Methods

### NewUserProfileResponse

`func NewUserProfileResponse(user VintedUserProfile, market string, ) *UserProfileResponse`

NewUserProfileResponse instantiates a new UserProfileResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUserProfileResponseWithDefaults

`func NewUserProfileResponseWithDefaults() *UserProfileResponse`

NewUserProfileResponseWithDefaults instantiates a new UserProfileResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUser

`func (o *UserProfileResponse) GetUser() VintedUserProfile`

GetUser returns the User field if non-nil, zero value otherwise.

### GetUserOk

`func (o *UserProfileResponse) GetUserOk() (*VintedUserProfile, bool)`

GetUserOk returns a tuple with the User field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUser

`func (o *UserProfileResponse) SetUser(v VintedUserProfile)`

SetUser sets User field to given value.


### GetMarket

`func (o *UserProfileResponse) GetMarket() string`

GetMarket returns the Market field if non-nil, zero value otherwise.

### GetMarketOk

`func (o *UserProfileResponse) GetMarketOk() (*string, bool)`

GetMarketOk returns a tuple with the Market field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMarket

`func (o *UserProfileResponse) SetMarket(v string)`

SetMarket sets Market field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



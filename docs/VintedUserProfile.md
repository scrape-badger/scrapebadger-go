# VintedUserProfile

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **int32** |  | 
**Login** | **string** |  | 
**PhotoUrl** | Pointer to **NullableString** |  | [optional] 
**Business** | Pointer to **bool** |  | [optional] [default to false]
**CountryCode** | Pointer to **NullableString** |  | [optional] 
**City** | Pointer to **NullableString** |  | [optional] 
**FeedbackCount** | Pointer to **int32** |  | [optional] [default to 0]
**FeedbackReputation** | Pointer to **float32** |  | [optional] [default to 0.0]
**PositiveFeedbackCount** | Pointer to **int32** |  | [optional] [default to 0]
**NeutralFeedbackCount** | Pointer to **int32** |  | [optional] [default to 0]
**NegativeFeedbackCount** | Pointer to **int32** |  | [optional] [default to 0]
**ItemCount** | Pointer to **int32** |  | [optional] [default to 0]
**TotalItemsCount** | Pointer to **int32** |  | [optional] [default to 0]
**FollowersCount** | Pointer to **int32** |  | [optional] [default to 0]
**FollowingCount** | Pointer to **int32** |  | [optional] [default to 0]
**IsOnline** | Pointer to **bool** |  | [optional] [default to false]
**IsOnHoliday** | Pointer to **bool** |  | [optional] [default to false]
**LastLogedOnTs** | Pointer to **NullableString** |  | [optional] 
**ProfileUrl** | Pointer to **NullableString** |  | [optional] 
**Locale** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewVintedUserProfile

`func NewVintedUserProfile(id int32, login string, ) *VintedUserProfile`

NewVintedUserProfile instantiates a new VintedUserProfile object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVintedUserProfileWithDefaults

`func NewVintedUserProfileWithDefaults() *VintedUserProfile`

NewVintedUserProfileWithDefaults instantiates a new VintedUserProfile object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *VintedUserProfile) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *VintedUserProfile) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *VintedUserProfile) SetId(v int32)`

SetId sets Id field to given value.


### GetLogin

`func (o *VintedUserProfile) GetLogin() string`

GetLogin returns the Login field if non-nil, zero value otherwise.

### GetLoginOk

`func (o *VintedUserProfile) GetLoginOk() (*string, bool)`

GetLoginOk returns a tuple with the Login field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogin

`func (o *VintedUserProfile) SetLogin(v string)`

SetLogin sets Login field to given value.


### GetPhotoUrl

`func (o *VintedUserProfile) GetPhotoUrl() string`

GetPhotoUrl returns the PhotoUrl field if non-nil, zero value otherwise.

### GetPhotoUrlOk

`func (o *VintedUserProfile) GetPhotoUrlOk() (*string, bool)`

GetPhotoUrlOk returns a tuple with the PhotoUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhotoUrl

`func (o *VintedUserProfile) SetPhotoUrl(v string)`

SetPhotoUrl sets PhotoUrl field to given value.

### HasPhotoUrl

`func (o *VintedUserProfile) HasPhotoUrl() bool`

HasPhotoUrl returns a boolean if a field has been set.

### SetPhotoUrlNil

`func (o *VintedUserProfile) SetPhotoUrlNil(b bool)`

 SetPhotoUrlNil sets the value for PhotoUrl to be an explicit nil

### UnsetPhotoUrl
`func (o *VintedUserProfile) UnsetPhotoUrl()`

UnsetPhotoUrl ensures that no value is present for PhotoUrl, not even an explicit nil
### GetBusiness

`func (o *VintedUserProfile) GetBusiness() bool`

GetBusiness returns the Business field if non-nil, zero value otherwise.

### GetBusinessOk

`func (o *VintedUserProfile) GetBusinessOk() (*bool, bool)`

GetBusinessOk returns a tuple with the Business field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBusiness

`func (o *VintedUserProfile) SetBusiness(v bool)`

SetBusiness sets Business field to given value.

### HasBusiness

`func (o *VintedUserProfile) HasBusiness() bool`

HasBusiness returns a boolean if a field has been set.

### GetCountryCode

`func (o *VintedUserProfile) GetCountryCode() string`

GetCountryCode returns the CountryCode field if non-nil, zero value otherwise.

### GetCountryCodeOk

`func (o *VintedUserProfile) GetCountryCodeOk() (*string, bool)`

GetCountryCodeOk returns a tuple with the CountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountryCode

`func (o *VintedUserProfile) SetCountryCode(v string)`

SetCountryCode sets CountryCode field to given value.

### HasCountryCode

`func (o *VintedUserProfile) HasCountryCode() bool`

HasCountryCode returns a boolean if a field has been set.

### SetCountryCodeNil

`func (o *VintedUserProfile) SetCountryCodeNil(b bool)`

 SetCountryCodeNil sets the value for CountryCode to be an explicit nil

### UnsetCountryCode
`func (o *VintedUserProfile) UnsetCountryCode()`

UnsetCountryCode ensures that no value is present for CountryCode, not even an explicit nil
### GetCity

`func (o *VintedUserProfile) GetCity() string`

GetCity returns the City field if non-nil, zero value otherwise.

### GetCityOk

`func (o *VintedUserProfile) GetCityOk() (*string, bool)`

GetCityOk returns a tuple with the City field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCity

`func (o *VintedUserProfile) SetCity(v string)`

SetCity sets City field to given value.

### HasCity

`func (o *VintedUserProfile) HasCity() bool`

HasCity returns a boolean if a field has been set.

### SetCityNil

`func (o *VintedUserProfile) SetCityNil(b bool)`

 SetCityNil sets the value for City to be an explicit nil

### UnsetCity
`func (o *VintedUserProfile) UnsetCity()`

UnsetCity ensures that no value is present for City, not even an explicit nil
### GetFeedbackCount

`func (o *VintedUserProfile) GetFeedbackCount() int32`

GetFeedbackCount returns the FeedbackCount field if non-nil, zero value otherwise.

### GetFeedbackCountOk

`func (o *VintedUserProfile) GetFeedbackCountOk() (*int32, bool)`

GetFeedbackCountOk returns a tuple with the FeedbackCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFeedbackCount

`func (o *VintedUserProfile) SetFeedbackCount(v int32)`

SetFeedbackCount sets FeedbackCount field to given value.

### HasFeedbackCount

`func (o *VintedUserProfile) HasFeedbackCount() bool`

HasFeedbackCount returns a boolean if a field has been set.

### GetFeedbackReputation

`func (o *VintedUserProfile) GetFeedbackReputation() float32`

GetFeedbackReputation returns the FeedbackReputation field if non-nil, zero value otherwise.

### GetFeedbackReputationOk

`func (o *VintedUserProfile) GetFeedbackReputationOk() (*float32, bool)`

GetFeedbackReputationOk returns a tuple with the FeedbackReputation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFeedbackReputation

`func (o *VintedUserProfile) SetFeedbackReputation(v float32)`

SetFeedbackReputation sets FeedbackReputation field to given value.

### HasFeedbackReputation

`func (o *VintedUserProfile) HasFeedbackReputation() bool`

HasFeedbackReputation returns a boolean if a field has been set.

### GetPositiveFeedbackCount

`func (o *VintedUserProfile) GetPositiveFeedbackCount() int32`

GetPositiveFeedbackCount returns the PositiveFeedbackCount field if non-nil, zero value otherwise.

### GetPositiveFeedbackCountOk

`func (o *VintedUserProfile) GetPositiveFeedbackCountOk() (*int32, bool)`

GetPositiveFeedbackCountOk returns a tuple with the PositiveFeedbackCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPositiveFeedbackCount

`func (o *VintedUserProfile) SetPositiveFeedbackCount(v int32)`

SetPositiveFeedbackCount sets PositiveFeedbackCount field to given value.

### HasPositiveFeedbackCount

`func (o *VintedUserProfile) HasPositiveFeedbackCount() bool`

HasPositiveFeedbackCount returns a boolean if a field has been set.

### GetNeutralFeedbackCount

`func (o *VintedUserProfile) GetNeutralFeedbackCount() int32`

GetNeutralFeedbackCount returns the NeutralFeedbackCount field if non-nil, zero value otherwise.

### GetNeutralFeedbackCountOk

`func (o *VintedUserProfile) GetNeutralFeedbackCountOk() (*int32, bool)`

GetNeutralFeedbackCountOk returns a tuple with the NeutralFeedbackCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNeutralFeedbackCount

`func (o *VintedUserProfile) SetNeutralFeedbackCount(v int32)`

SetNeutralFeedbackCount sets NeutralFeedbackCount field to given value.

### HasNeutralFeedbackCount

`func (o *VintedUserProfile) HasNeutralFeedbackCount() bool`

HasNeutralFeedbackCount returns a boolean if a field has been set.

### GetNegativeFeedbackCount

`func (o *VintedUserProfile) GetNegativeFeedbackCount() int32`

GetNegativeFeedbackCount returns the NegativeFeedbackCount field if non-nil, zero value otherwise.

### GetNegativeFeedbackCountOk

`func (o *VintedUserProfile) GetNegativeFeedbackCountOk() (*int32, bool)`

GetNegativeFeedbackCountOk returns a tuple with the NegativeFeedbackCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNegativeFeedbackCount

`func (o *VintedUserProfile) SetNegativeFeedbackCount(v int32)`

SetNegativeFeedbackCount sets NegativeFeedbackCount field to given value.

### HasNegativeFeedbackCount

`func (o *VintedUserProfile) HasNegativeFeedbackCount() bool`

HasNegativeFeedbackCount returns a boolean if a field has been set.

### GetItemCount

`func (o *VintedUserProfile) GetItemCount() int32`

GetItemCount returns the ItemCount field if non-nil, zero value otherwise.

### GetItemCountOk

`func (o *VintedUserProfile) GetItemCountOk() (*int32, bool)`

GetItemCountOk returns a tuple with the ItemCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItemCount

`func (o *VintedUserProfile) SetItemCount(v int32)`

SetItemCount sets ItemCount field to given value.

### HasItemCount

`func (o *VintedUserProfile) HasItemCount() bool`

HasItemCount returns a boolean if a field has been set.

### GetTotalItemsCount

`func (o *VintedUserProfile) GetTotalItemsCount() int32`

GetTotalItemsCount returns the TotalItemsCount field if non-nil, zero value otherwise.

### GetTotalItemsCountOk

`func (o *VintedUserProfile) GetTotalItemsCountOk() (*int32, bool)`

GetTotalItemsCountOk returns a tuple with the TotalItemsCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalItemsCount

`func (o *VintedUserProfile) SetTotalItemsCount(v int32)`

SetTotalItemsCount sets TotalItemsCount field to given value.

### HasTotalItemsCount

`func (o *VintedUserProfile) HasTotalItemsCount() bool`

HasTotalItemsCount returns a boolean if a field has been set.

### GetFollowersCount

`func (o *VintedUserProfile) GetFollowersCount() int32`

GetFollowersCount returns the FollowersCount field if non-nil, zero value otherwise.

### GetFollowersCountOk

`func (o *VintedUserProfile) GetFollowersCountOk() (*int32, bool)`

GetFollowersCountOk returns a tuple with the FollowersCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFollowersCount

`func (o *VintedUserProfile) SetFollowersCount(v int32)`

SetFollowersCount sets FollowersCount field to given value.

### HasFollowersCount

`func (o *VintedUserProfile) HasFollowersCount() bool`

HasFollowersCount returns a boolean if a field has been set.

### GetFollowingCount

`func (o *VintedUserProfile) GetFollowingCount() int32`

GetFollowingCount returns the FollowingCount field if non-nil, zero value otherwise.

### GetFollowingCountOk

`func (o *VintedUserProfile) GetFollowingCountOk() (*int32, bool)`

GetFollowingCountOk returns a tuple with the FollowingCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFollowingCount

`func (o *VintedUserProfile) SetFollowingCount(v int32)`

SetFollowingCount sets FollowingCount field to given value.

### HasFollowingCount

`func (o *VintedUserProfile) HasFollowingCount() bool`

HasFollowingCount returns a boolean if a field has been set.

### GetIsOnline

`func (o *VintedUserProfile) GetIsOnline() bool`

GetIsOnline returns the IsOnline field if non-nil, zero value otherwise.

### GetIsOnlineOk

`func (o *VintedUserProfile) GetIsOnlineOk() (*bool, bool)`

GetIsOnlineOk returns a tuple with the IsOnline field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsOnline

`func (o *VintedUserProfile) SetIsOnline(v bool)`

SetIsOnline sets IsOnline field to given value.

### HasIsOnline

`func (o *VintedUserProfile) HasIsOnline() bool`

HasIsOnline returns a boolean if a field has been set.

### GetIsOnHoliday

`func (o *VintedUserProfile) GetIsOnHoliday() bool`

GetIsOnHoliday returns the IsOnHoliday field if non-nil, zero value otherwise.

### GetIsOnHolidayOk

`func (o *VintedUserProfile) GetIsOnHolidayOk() (*bool, bool)`

GetIsOnHolidayOk returns a tuple with the IsOnHoliday field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsOnHoliday

`func (o *VintedUserProfile) SetIsOnHoliday(v bool)`

SetIsOnHoliday sets IsOnHoliday field to given value.

### HasIsOnHoliday

`func (o *VintedUserProfile) HasIsOnHoliday() bool`

HasIsOnHoliday returns a boolean if a field has been set.

### GetLastLogedOnTs

`func (o *VintedUserProfile) GetLastLogedOnTs() string`

GetLastLogedOnTs returns the LastLogedOnTs field if non-nil, zero value otherwise.

### GetLastLogedOnTsOk

`func (o *VintedUserProfile) GetLastLogedOnTsOk() (*string, bool)`

GetLastLogedOnTsOk returns a tuple with the LastLogedOnTs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastLogedOnTs

`func (o *VintedUserProfile) SetLastLogedOnTs(v string)`

SetLastLogedOnTs sets LastLogedOnTs field to given value.

### HasLastLogedOnTs

`func (o *VintedUserProfile) HasLastLogedOnTs() bool`

HasLastLogedOnTs returns a boolean if a field has been set.

### SetLastLogedOnTsNil

`func (o *VintedUserProfile) SetLastLogedOnTsNil(b bool)`

 SetLastLogedOnTsNil sets the value for LastLogedOnTs to be an explicit nil

### UnsetLastLogedOnTs
`func (o *VintedUserProfile) UnsetLastLogedOnTs()`

UnsetLastLogedOnTs ensures that no value is present for LastLogedOnTs, not even an explicit nil
### GetProfileUrl

`func (o *VintedUserProfile) GetProfileUrl() string`

GetProfileUrl returns the ProfileUrl field if non-nil, zero value otherwise.

### GetProfileUrlOk

`func (o *VintedUserProfile) GetProfileUrlOk() (*string, bool)`

GetProfileUrlOk returns a tuple with the ProfileUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProfileUrl

`func (o *VintedUserProfile) SetProfileUrl(v string)`

SetProfileUrl sets ProfileUrl field to given value.

### HasProfileUrl

`func (o *VintedUserProfile) HasProfileUrl() bool`

HasProfileUrl returns a boolean if a field has been set.

### SetProfileUrlNil

`func (o *VintedUserProfile) SetProfileUrlNil(b bool)`

 SetProfileUrlNil sets the value for ProfileUrl to be an explicit nil

### UnsetProfileUrl
`func (o *VintedUserProfile) UnsetProfileUrl()`

UnsetProfileUrl ensures that no value is present for ProfileUrl, not even an explicit nil
### GetLocale

`func (o *VintedUserProfile) GetLocale() string`

GetLocale returns the Locale field if non-nil, zero value otherwise.

### GetLocaleOk

`func (o *VintedUserProfile) GetLocaleOk() (*string, bool)`

GetLocaleOk returns a tuple with the Locale field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocale

`func (o *VintedUserProfile) SetLocale(v string)`

SetLocale sets Locale field to given value.

### HasLocale

`func (o *VintedUserProfile) HasLocale() bool`

HasLocale returns a boolean if a field has been set.

### SetLocaleNil

`func (o *VintedUserProfile) SetLocaleNil(b bool)`

 SetLocaleNil sets the value for Locale to be an explicit nil

### UnsetLocale
`func (o *VintedUserProfile) UnsetLocale()`

UnsetLocale ensures that no value is present for Locale, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



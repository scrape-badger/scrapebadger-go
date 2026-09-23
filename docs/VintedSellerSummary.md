# VintedSellerSummary

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **int32** |  | 
**Login** | Pointer to **string** |  | [optional] [default to ""]
**PhotoUrl** | Pointer to **NullableString** |  | [optional] 
**Business** | Pointer to **bool** |  | [optional] [default to false]
**FeedbackCount** | Pointer to **int32** |  | [optional] [default to 0]
**FeedbackReputation** | Pointer to **float32** |  | [optional] [default to 0.0]
**ItemCount** | Pointer to **int32** |  | [optional] [default to 0]
**Location** | Pointer to **NullableString** |  | [optional] 
**LastSeen** | Pointer to **NullableString** |  | [optional] 
**Badges** | Pointer to **[]string** |  | [optional] 

## Methods

### NewVintedSellerSummary

`func NewVintedSellerSummary(id int32, ) *VintedSellerSummary`

NewVintedSellerSummary instantiates a new VintedSellerSummary object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVintedSellerSummaryWithDefaults

`func NewVintedSellerSummaryWithDefaults() *VintedSellerSummary`

NewVintedSellerSummaryWithDefaults instantiates a new VintedSellerSummary object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *VintedSellerSummary) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *VintedSellerSummary) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *VintedSellerSummary) SetId(v int32)`

SetId sets Id field to given value.


### GetLogin

`func (o *VintedSellerSummary) GetLogin() string`

GetLogin returns the Login field if non-nil, zero value otherwise.

### GetLoginOk

`func (o *VintedSellerSummary) GetLoginOk() (*string, bool)`

GetLoginOk returns a tuple with the Login field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogin

`func (o *VintedSellerSummary) SetLogin(v string)`

SetLogin sets Login field to given value.

### HasLogin

`func (o *VintedSellerSummary) HasLogin() bool`

HasLogin returns a boolean if a field has been set.

### GetPhotoUrl

`func (o *VintedSellerSummary) GetPhotoUrl() string`

GetPhotoUrl returns the PhotoUrl field if non-nil, zero value otherwise.

### GetPhotoUrlOk

`func (o *VintedSellerSummary) GetPhotoUrlOk() (*string, bool)`

GetPhotoUrlOk returns a tuple with the PhotoUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhotoUrl

`func (o *VintedSellerSummary) SetPhotoUrl(v string)`

SetPhotoUrl sets PhotoUrl field to given value.

### HasPhotoUrl

`func (o *VintedSellerSummary) HasPhotoUrl() bool`

HasPhotoUrl returns a boolean if a field has been set.

### SetPhotoUrlNil

`func (o *VintedSellerSummary) SetPhotoUrlNil(b bool)`

 SetPhotoUrlNil sets the value for PhotoUrl to be an explicit nil

### UnsetPhotoUrl
`func (o *VintedSellerSummary) UnsetPhotoUrl()`

UnsetPhotoUrl ensures that no value is present for PhotoUrl, not even an explicit nil
### GetBusiness

`func (o *VintedSellerSummary) GetBusiness() bool`

GetBusiness returns the Business field if non-nil, zero value otherwise.

### GetBusinessOk

`func (o *VintedSellerSummary) GetBusinessOk() (*bool, bool)`

GetBusinessOk returns a tuple with the Business field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBusiness

`func (o *VintedSellerSummary) SetBusiness(v bool)`

SetBusiness sets Business field to given value.

### HasBusiness

`func (o *VintedSellerSummary) HasBusiness() bool`

HasBusiness returns a boolean if a field has been set.

### GetFeedbackCount

`func (o *VintedSellerSummary) GetFeedbackCount() int32`

GetFeedbackCount returns the FeedbackCount field if non-nil, zero value otherwise.

### GetFeedbackCountOk

`func (o *VintedSellerSummary) GetFeedbackCountOk() (*int32, bool)`

GetFeedbackCountOk returns a tuple with the FeedbackCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFeedbackCount

`func (o *VintedSellerSummary) SetFeedbackCount(v int32)`

SetFeedbackCount sets FeedbackCount field to given value.

### HasFeedbackCount

`func (o *VintedSellerSummary) HasFeedbackCount() bool`

HasFeedbackCount returns a boolean if a field has been set.

### GetFeedbackReputation

`func (o *VintedSellerSummary) GetFeedbackReputation() float32`

GetFeedbackReputation returns the FeedbackReputation field if non-nil, zero value otherwise.

### GetFeedbackReputationOk

`func (o *VintedSellerSummary) GetFeedbackReputationOk() (*float32, bool)`

GetFeedbackReputationOk returns a tuple with the FeedbackReputation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFeedbackReputation

`func (o *VintedSellerSummary) SetFeedbackReputation(v float32)`

SetFeedbackReputation sets FeedbackReputation field to given value.

### HasFeedbackReputation

`func (o *VintedSellerSummary) HasFeedbackReputation() bool`

HasFeedbackReputation returns a boolean if a field has been set.

### GetItemCount

`func (o *VintedSellerSummary) GetItemCount() int32`

GetItemCount returns the ItemCount field if non-nil, zero value otherwise.

### GetItemCountOk

`func (o *VintedSellerSummary) GetItemCountOk() (*int32, bool)`

GetItemCountOk returns a tuple with the ItemCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItemCount

`func (o *VintedSellerSummary) SetItemCount(v int32)`

SetItemCount sets ItemCount field to given value.

### HasItemCount

`func (o *VintedSellerSummary) HasItemCount() bool`

HasItemCount returns a boolean if a field has been set.

### GetLocation

`func (o *VintedSellerSummary) GetLocation() string`

GetLocation returns the Location field if non-nil, zero value otherwise.

### GetLocationOk

`func (o *VintedSellerSummary) GetLocationOk() (*string, bool)`

GetLocationOk returns a tuple with the Location field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocation

`func (o *VintedSellerSummary) SetLocation(v string)`

SetLocation sets Location field to given value.

### HasLocation

`func (o *VintedSellerSummary) HasLocation() bool`

HasLocation returns a boolean if a field has been set.

### SetLocationNil

`func (o *VintedSellerSummary) SetLocationNil(b bool)`

 SetLocationNil sets the value for Location to be an explicit nil

### UnsetLocation
`func (o *VintedSellerSummary) UnsetLocation()`

UnsetLocation ensures that no value is present for Location, not even an explicit nil
### GetLastSeen

`func (o *VintedSellerSummary) GetLastSeen() string`

GetLastSeen returns the LastSeen field if non-nil, zero value otherwise.

### GetLastSeenOk

`func (o *VintedSellerSummary) GetLastSeenOk() (*string, bool)`

GetLastSeenOk returns a tuple with the LastSeen field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeen

`func (o *VintedSellerSummary) SetLastSeen(v string)`

SetLastSeen sets LastSeen field to given value.

### HasLastSeen

`func (o *VintedSellerSummary) HasLastSeen() bool`

HasLastSeen returns a boolean if a field has been set.

### SetLastSeenNil

`func (o *VintedSellerSummary) SetLastSeenNil(b bool)`

 SetLastSeenNil sets the value for LastSeen to be an explicit nil

### UnsetLastSeen
`func (o *VintedSellerSummary) UnsetLastSeen()`

UnsetLastSeen ensures that no value is present for LastSeen, not even an explicit nil
### GetBadges

`func (o *VintedSellerSummary) GetBadges() []string`

GetBadges returns the Badges field if non-nil, zero value otherwise.

### GetBadgesOk

`func (o *VintedSellerSummary) GetBadgesOk() (*[]string, bool)`

GetBadgesOk returns a tuple with the Badges field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBadges

`func (o *VintedSellerSummary) SetBadges(v []string)`

SetBadges sets Badges field to given value.

### HasBadges

`func (o *VintedSellerSummary) HasBadges() bool`

HasBadges returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



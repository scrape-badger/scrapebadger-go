# VintedUserSummary

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **int32** |  | 
**Login** | **string** |  | 
**PhotoUrl** | Pointer to **NullableString** |  | [optional] 
**Business** | Pointer to **bool** |  | [optional] [default to false]

## Methods

### NewVintedUserSummary

`func NewVintedUserSummary(id int32, login string, ) *VintedUserSummary`

NewVintedUserSummary instantiates a new VintedUserSummary object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVintedUserSummaryWithDefaults

`func NewVintedUserSummaryWithDefaults() *VintedUserSummary`

NewVintedUserSummaryWithDefaults instantiates a new VintedUserSummary object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *VintedUserSummary) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *VintedUserSummary) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *VintedUserSummary) SetId(v int32)`

SetId sets Id field to given value.


### GetLogin

`func (o *VintedUserSummary) GetLogin() string`

GetLogin returns the Login field if non-nil, zero value otherwise.

### GetLoginOk

`func (o *VintedUserSummary) GetLoginOk() (*string, bool)`

GetLoginOk returns a tuple with the Login field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogin

`func (o *VintedUserSummary) SetLogin(v string)`

SetLogin sets Login field to given value.


### GetPhotoUrl

`func (o *VintedUserSummary) GetPhotoUrl() string`

GetPhotoUrl returns the PhotoUrl field if non-nil, zero value otherwise.

### GetPhotoUrlOk

`func (o *VintedUserSummary) GetPhotoUrlOk() (*string, bool)`

GetPhotoUrlOk returns a tuple with the PhotoUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhotoUrl

`func (o *VintedUserSummary) SetPhotoUrl(v string)`

SetPhotoUrl sets PhotoUrl field to given value.

### HasPhotoUrl

`func (o *VintedUserSummary) HasPhotoUrl() bool`

HasPhotoUrl returns a boolean if a field has been set.

### SetPhotoUrlNil

`func (o *VintedUserSummary) SetPhotoUrlNil(b bool)`

 SetPhotoUrlNil sets the value for PhotoUrl to be an explicit nil

### UnsetPhotoUrl
`func (o *VintedUserSummary) UnsetPhotoUrl()`

UnsetPhotoUrl ensures that no value is present for PhotoUrl, not even an explicit nil
### GetBusiness

`func (o *VintedUserSummary) GetBusiness() bool`

GetBusiness returns the Business field if non-nil, zero value otherwise.

### GetBusinessOk

`func (o *VintedUserSummary) GetBusinessOk() (*bool, bool)`

GetBusinessOk returns a tuple with the Business field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBusiness

`func (o *VintedUserSummary) SetBusiness(v bool)`

SetBusiness sets Business field to given value.

### HasBusiness

`func (o *VintedUserSummary) HasBusiness() bool`

HasBusiness returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ScreenshotRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Url** | **string** | The page to fetch. | 
**WaitFor** | Pointer to **NullableString** |  | [optional] 
**Country** | Pointer to **NullableString** |  | [optional] 
**ProxyTier** | Pointer to **string** | Proxy pool: simple, premium or ultra. | [optional] [default to "simple"]
**FullPage** | Pointer to **bool** | Capture the whole scrollable page instead of the viewport. | [optional] [default to false]
**Width** | Pointer to **NullableInt32** |  | [optional] 
**Height** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewScreenshotRequest

`func NewScreenshotRequest(url string, ) *ScreenshotRequest`

NewScreenshotRequest instantiates a new ScreenshotRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScreenshotRequestWithDefaults

`func NewScreenshotRequestWithDefaults() *ScreenshotRequest`

NewScreenshotRequestWithDefaults instantiates a new ScreenshotRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUrl

`func (o *ScreenshotRequest) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *ScreenshotRequest) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *ScreenshotRequest) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetWaitFor

`func (o *ScreenshotRequest) GetWaitFor() string`

GetWaitFor returns the WaitFor field if non-nil, zero value otherwise.

### GetWaitForOk

`func (o *ScreenshotRequest) GetWaitForOk() (*string, bool)`

GetWaitForOk returns a tuple with the WaitFor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWaitFor

`func (o *ScreenshotRequest) SetWaitFor(v string)`

SetWaitFor sets WaitFor field to given value.

### HasWaitFor

`func (o *ScreenshotRequest) HasWaitFor() bool`

HasWaitFor returns a boolean if a field has been set.

### SetWaitForNil

`func (o *ScreenshotRequest) SetWaitForNil(b bool)`

 SetWaitForNil sets the value for WaitFor to be an explicit nil

### UnsetWaitFor
`func (o *ScreenshotRequest) UnsetWaitFor()`

UnsetWaitFor ensures that no value is present for WaitFor, not even an explicit nil
### GetCountry

`func (o *ScreenshotRequest) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *ScreenshotRequest) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *ScreenshotRequest) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *ScreenshotRequest) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### SetCountryNil

`func (o *ScreenshotRequest) SetCountryNil(b bool)`

 SetCountryNil sets the value for Country to be an explicit nil

### UnsetCountry
`func (o *ScreenshotRequest) UnsetCountry()`

UnsetCountry ensures that no value is present for Country, not even an explicit nil
### GetProxyTier

`func (o *ScreenshotRequest) GetProxyTier() string`

GetProxyTier returns the ProxyTier field if non-nil, zero value otherwise.

### GetProxyTierOk

`func (o *ScreenshotRequest) GetProxyTierOk() (*string, bool)`

GetProxyTierOk returns a tuple with the ProxyTier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProxyTier

`func (o *ScreenshotRequest) SetProxyTier(v string)`

SetProxyTier sets ProxyTier field to given value.

### HasProxyTier

`func (o *ScreenshotRequest) HasProxyTier() bool`

HasProxyTier returns a boolean if a field has been set.

### GetFullPage

`func (o *ScreenshotRequest) GetFullPage() bool`

GetFullPage returns the FullPage field if non-nil, zero value otherwise.

### GetFullPageOk

`func (o *ScreenshotRequest) GetFullPageOk() (*bool, bool)`

GetFullPageOk returns a tuple with the FullPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFullPage

`func (o *ScreenshotRequest) SetFullPage(v bool)`

SetFullPage sets FullPage field to given value.

### HasFullPage

`func (o *ScreenshotRequest) HasFullPage() bool`

HasFullPage returns a boolean if a field has been set.

### GetWidth

`func (o *ScreenshotRequest) GetWidth() int32`

GetWidth returns the Width field if non-nil, zero value otherwise.

### GetWidthOk

`func (o *ScreenshotRequest) GetWidthOk() (*int32, bool)`

GetWidthOk returns a tuple with the Width field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWidth

`func (o *ScreenshotRequest) SetWidth(v int32)`

SetWidth sets Width field to given value.

### HasWidth

`func (o *ScreenshotRequest) HasWidth() bool`

HasWidth returns a boolean if a field has been set.

### SetWidthNil

`func (o *ScreenshotRequest) SetWidthNil(b bool)`

 SetWidthNil sets the value for Width to be an explicit nil

### UnsetWidth
`func (o *ScreenshotRequest) UnsetWidth()`

UnsetWidth ensures that no value is present for Width, not even an explicit nil
### GetHeight

`func (o *ScreenshotRequest) GetHeight() int32`

GetHeight returns the Height field if non-nil, zero value otherwise.

### GetHeightOk

`func (o *ScreenshotRequest) GetHeightOk() (*int32, bool)`

GetHeightOk returns a tuple with the Height field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeight

`func (o *ScreenshotRequest) SetHeight(v int32)`

SetHeight sets Height field to given value.

### HasHeight

`func (o *ScreenshotRequest) HasHeight() bool`

HasHeight returns a boolean if a field has been set.

### SetHeightNil

`func (o *ScreenshotRequest) SetHeightNil(b bool)`

 SetHeightNil sets the value for Height to be an explicit nil

### UnsetHeight
`func (o *ScreenshotRequest) UnsetHeight()`

UnsetHeight ensures that no value is present for Height, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



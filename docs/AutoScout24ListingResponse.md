# AutoScout24ListingResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Market** | **string** |  | 
**SourceUrl** | **string** |  | 
**Listing** | [**AutoScout24ListingDetail**](AutoScout24ListingDetail.md) |  | 
**LatencyMs** | **int32** |  | 

## Methods

### NewAutoScout24ListingResponse

`func NewAutoScout24ListingResponse(market string, sourceUrl string, listing AutoScout24ListingDetail, latencyMs int32, ) *AutoScout24ListingResponse`

NewAutoScout24ListingResponse instantiates a new AutoScout24ListingResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAutoScout24ListingResponseWithDefaults

`func NewAutoScout24ListingResponseWithDefaults() *AutoScout24ListingResponse`

NewAutoScout24ListingResponseWithDefaults instantiates a new AutoScout24ListingResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMarket

`func (o *AutoScout24ListingResponse) GetMarket() string`

GetMarket returns the Market field if non-nil, zero value otherwise.

### GetMarketOk

`func (o *AutoScout24ListingResponse) GetMarketOk() (*string, bool)`

GetMarketOk returns a tuple with the Market field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMarket

`func (o *AutoScout24ListingResponse) SetMarket(v string)`

SetMarket sets Market field to given value.


### GetSourceUrl

`func (o *AutoScout24ListingResponse) GetSourceUrl() string`

GetSourceUrl returns the SourceUrl field if non-nil, zero value otherwise.

### GetSourceUrlOk

`func (o *AutoScout24ListingResponse) GetSourceUrlOk() (*string, bool)`

GetSourceUrlOk returns a tuple with the SourceUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceUrl

`func (o *AutoScout24ListingResponse) SetSourceUrl(v string)`

SetSourceUrl sets SourceUrl field to given value.


### GetListing

`func (o *AutoScout24ListingResponse) GetListing() AutoScout24ListingDetail`

GetListing returns the Listing field if non-nil, zero value otherwise.

### GetListingOk

`func (o *AutoScout24ListingResponse) GetListingOk() (*AutoScout24ListingDetail, bool)`

GetListingOk returns a tuple with the Listing field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListing

`func (o *AutoScout24ListingResponse) SetListing(v AutoScout24ListingDetail)`

SetListing sets Listing field to given value.


### GetLatencyMs

`func (o *AutoScout24ListingResponse) GetLatencyMs() int32`

GetLatencyMs returns the LatencyMs field if non-nil, zero value otherwise.

### GetLatencyMsOk

`func (o *AutoScout24ListingResponse) GetLatencyMsOk() (*int32, bool)`

GetLatencyMsOk returns a tuple with the LatencyMs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatencyMs

`func (o *AutoScout24ListingResponse) SetLatencyMs(v int32)`

SetLatencyMs sets LatencyMs field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



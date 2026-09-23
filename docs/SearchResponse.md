# SearchResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Items** | [**[]VintedItemSummary**](VintedItemSummary.md) |  | 
**Pagination** | [**VintedPagination**](VintedPagination.md) |  | 
**Market** | **string** |  | 
**SellerCountry** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewSearchResponse

`func NewSearchResponse(items []VintedItemSummary, pagination VintedPagination, market string, ) *SearchResponse`

NewSearchResponse instantiates a new SearchResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSearchResponseWithDefaults

`func NewSearchResponseWithDefaults() *SearchResponse`

NewSearchResponseWithDefaults instantiates a new SearchResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetItems

`func (o *SearchResponse) GetItems() []VintedItemSummary`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *SearchResponse) GetItemsOk() (*[]VintedItemSummary, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *SearchResponse) SetItems(v []VintedItemSummary)`

SetItems sets Items field to given value.


### GetPagination

`func (o *SearchResponse) GetPagination() VintedPagination`

GetPagination returns the Pagination field if non-nil, zero value otherwise.

### GetPaginationOk

`func (o *SearchResponse) GetPaginationOk() (*VintedPagination, bool)`

GetPaginationOk returns a tuple with the Pagination field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPagination

`func (o *SearchResponse) SetPagination(v VintedPagination)`

SetPagination sets Pagination field to given value.


### GetMarket

`func (o *SearchResponse) GetMarket() string`

GetMarket returns the Market field if non-nil, zero value otherwise.

### GetMarketOk

`func (o *SearchResponse) GetMarketOk() (*string, bool)`

GetMarketOk returns a tuple with the Market field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMarket

`func (o *SearchResponse) SetMarket(v string)`

SetMarket sets Market field to given value.


### GetSellerCountry

`func (o *SearchResponse) GetSellerCountry() string`

GetSellerCountry returns the SellerCountry field if non-nil, zero value otherwise.

### GetSellerCountryOk

`func (o *SearchResponse) GetSellerCountryOk() (*string, bool)`

GetSellerCountryOk returns a tuple with the SellerCountry field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSellerCountry

`func (o *SearchResponse) SetSellerCountry(v string)`

SetSellerCountry sets SellerCountry field to given value.

### HasSellerCountry

`func (o *SearchResponse) HasSellerCountry() bool`

HasSellerCountry returns a boolean if a field has been set.

### SetSellerCountryNil

`func (o *SearchResponse) SetSellerCountryNil(b bool)`

 SetSellerCountryNil sets the value for SellerCountry to be an explicit nil

### UnsetSellerCountry
`func (o *SearchResponse) UnsetSellerCountry()`

UnsetSellerCountry ensures that no value is present for SellerCountry, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



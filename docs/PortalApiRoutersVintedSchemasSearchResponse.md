# PortalApiRoutersVintedSchemasSearchResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Items** | [**[]VintedItemSummary**](VintedItemSummary.md) |  | 
**Pagination** | [**VintedPagination**](VintedPagination.md) |  | 
**Market** | **string** |  | 
**SellerCountry** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewPortalApiRoutersVintedSchemasSearchResponse

`func NewPortalApiRoutersVintedSchemasSearchResponse(items []VintedItemSummary, pagination VintedPagination, market string, ) *PortalApiRoutersVintedSchemasSearchResponse`

NewPortalApiRoutersVintedSchemasSearchResponse instantiates a new PortalApiRoutersVintedSchemasSearchResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPortalApiRoutersVintedSchemasSearchResponseWithDefaults

`func NewPortalApiRoutersVintedSchemasSearchResponseWithDefaults() *PortalApiRoutersVintedSchemasSearchResponse`

NewPortalApiRoutersVintedSchemasSearchResponseWithDefaults instantiates a new PortalApiRoutersVintedSchemasSearchResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetItems

`func (o *PortalApiRoutersVintedSchemasSearchResponse) GetItems() []VintedItemSummary`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *PortalApiRoutersVintedSchemasSearchResponse) GetItemsOk() (*[]VintedItemSummary, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *PortalApiRoutersVintedSchemasSearchResponse) SetItems(v []VintedItemSummary)`

SetItems sets Items field to given value.


### GetPagination

`func (o *PortalApiRoutersVintedSchemasSearchResponse) GetPagination() VintedPagination`

GetPagination returns the Pagination field if non-nil, zero value otherwise.

### GetPaginationOk

`func (o *PortalApiRoutersVintedSchemasSearchResponse) GetPaginationOk() (*VintedPagination, bool)`

GetPaginationOk returns a tuple with the Pagination field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPagination

`func (o *PortalApiRoutersVintedSchemasSearchResponse) SetPagination(v VintedPagination)`

SetPagination sets Pagination field to given value.


### GetMarket

`func (o *PortalApiRoutersVintedSchemasSearchResponse) GetMarket() string`

GetMarket returns the Market field if non-nil, zero value otherwise.

### GetMarketOk

`func (o *PortalApiRoutersVintedSchemasSearchResponse) GetMarketOk() (*string, bool)`

GetMarketOk returns a tuple with the Market field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMarket

`func (o *PortalApiRoutersVintedSchemasSearchResponse) SetMarket(v string)`

SetMarket sets Market field to given value.


### GetSellerCountry

`func (o *PortalApiRoutersVintedSchemasSearchResponse) GetSellerCountry() string`

GetSellerCountry returns the SellerCountry field if non-nil, zero value otherwise.

### GetSellerCountryOk

`func (o *PortalApiRoutersVintedSchemasSearchResponse) GetSellerCountryOk() (*string, bool)`

GetSellerCountryOk returns a tuple with the SellerCountry field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSellerCountry

`func (o *PortalApiRoutersVintedSchemasSearchResponse) SetSellerCountry(v string)`

SetSellerCountry sets SellerCountry field to given value.

### HasSellerCountry

`func (o *PortalApiRoutersVintedSchemasSearchResponse) HasSellerCountry() bool`

HasSellerCountry returns a boolean if a field has been set.

### SetSellerCountryNil

`func (o *PortalApiRoutersVintedSchemasSearchResponse) SetSellerCountryNil(b bool)`

 SetSellerCountryNil sets the value for SellerCountry to be an explicit nil

### UnsetSellerCountry
`func (o *PortalApiRoutersVintedSchemasSearchResponse) UnsetSellerCountry()`

UnsetSellerCountry ensures that no value is present for SellerCountry, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



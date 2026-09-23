# UserItemsResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Items** | [**[]VintedItemSummary**](VintedItemSummary.md) |  | 
**Pagination** | [**VintedPagination**](VintedPagination.md) |  | 
**Market** | **string** |  | 

## Methods

### NewUserItemsResponse

`func NewUserItemsResponse(items []VintedItemSummary, pagination VintedPagination, market string, ) *UserItemsResponse`

NewUserItemsResponse instantiates a new UserItemsResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUserItemsResponseWithDefaults

`func NewUserItemsResponseWithDefaults() *UserItemsResponse`

NewUserItemsResponseWithDefaults instantiates a new UserItemsResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetItems

`func (o *UserItemsResponse) GetItems() []VintedItemSummary`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *UserItemsResponse) GetItemsOk() (*[]VintedItemSummary, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *UserItemsResponse) SetItems(v []VintedItemSummary)`

SetItems sets Items field to given value.


### GetPagination

`func (o *UserItemsResponse) GetPagination() VintedPagination`

GetPagination returns the Pagination field if non-nil, zero value otherwise.

### GetPaginationOk

`func (o *UserItemsResponse) GetPaginationOk() (*VintedPagination, bool)`

GetPaginationOk returns a tuple with the Pagination field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPagination

`func (o *UserItemsResponse) SetPagination(v VintedPagination)`

SetPagination sets Pagination field to given value.


### GetMarket

`func (o *UserItemsResponse) GetMarket() string`

GetMarket returns the Market field if non-nil, zero value otherwise.

### GetMarketOk

`func (o *UserItemsResponse) GetMarketOk() (*string, bool)`

GetMarketOk returns a tuple with the Market field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMarket

`func (o *UserItemsResponse) SetMarket(v string)`

SetMarket sets Market field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



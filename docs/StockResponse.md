# StockResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Market** | **string** |  | 
**Products** | [**[]StockProduct**](StockProduct.md) |  | 
**MissingProductIds** | Pointer to **[]int32** |  | [optional] 

## Methods

### NewStockResponse

`func NewStockResponse(market string, products []StockProduct, ) *StockResponse`

NewStockResponse instantiates a new StockResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStockResponseWithDefaults

`func NewStockResponseWithDefaults() *StockResponse`

NewStockResponseWithDefaults instantiates a new StockResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMarket

`func (o *StockResponse) GetMarket() string`

GetMarket returns the Market field if non-nil, zero value otherwise.

### GetMarketOk

`func (o *StockResponse) GetMarketOk() (*string, bool)`

GetMarketOk returns a tuple with the Market field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMarket

`func (o *StockResponse) SetMarket(v string)`

SetMarket sets Market field to given value.


### GetProducts

`func (o *StockResponse) GetProducts() []StockProduct`

GetProducts returns the Products field if non-nil, zero value otherwise.

### GetProductsOk

`func (o *StockResponse) GetProductsOk() (*[]StockProduct, bool)`

GetProductsOk returns a tuple with the Products field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProducts

`func (o *StockResponse) SetProducts(v []StockProduct)`

SetProducts sets Products field to given value.


### GetMissingProductIds

`func (o *StockResponse) GetMissingProductIds() []int32`

GetMissingProductIds returns the MissingProductIds field if non-nil, zero value otherwise.

### GetMissingProductIdsOk

`func (o *StockResponse) GetMissingProductIdsOk() (*[]int32, bool)`

GetMissingProductIdsOk returns a tuple with the MissingProductIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMissingProductIds

`func (o *StockResponse) SetMissingProductIds(v []int32)`

SetMissingProductIds sets MissingProductIds field to given value.

### HasMissingProductIds

`func (o *StockResponse) HasMissingProductIds() bool`

HasMissingProductIds returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



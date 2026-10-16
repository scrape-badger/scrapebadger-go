# ProductResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Market** | **string** |  | 
**Product** | [**Product**](Product.md) |  | 

## Methods

### NewProductResponse

`func NewProductResponse(market string, product Product, ) *ProductResponse`

NewProductResponse instantiates a new ProductResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProductResponseWithDefaults

`func NewProductResponseWithDefaults() *ProductResponse`

NewProductResponseWithDefaults instantiates a new ProductResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMarket

`func (o *ProductResponse) GetMarket() string`

GetMarket returns the Market field if non-nil, zero value otherwise.

### GetMarketOk

`func (o *ProductResponse) GetMarketOk() (*string, bool)`

GetMarketOk returns a tuple with the Market field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMarket

`func (o *ProductResponse) SetMarket(v string)`

SetMarket sets Market field to given value.


### GetProduct

`func (o *ProductResponse) GetProduct() Product`

GetProduct returns the Product field if non-nil, zero value otherwise.

### GetProductOk

`func (o *ProductResponse) GetProductOk() (*Product, bool)`

GetProductOk returns a tuple with the Product field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProduct

`func (o *ProductResponse) SetProduct(v Product)`

SetProduct sets Product field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



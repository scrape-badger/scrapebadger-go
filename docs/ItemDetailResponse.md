# ItemDetailResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Item** | [**VintedItemDetail**](VintedItemDetail.md) |  | 
**Market** | **string** |  | 

## Methods

### NewItemDetailResponse

`func NewItemDetailResponse(item VintedItemDetail, market string, ) *ItemDetailResponse`

NewItemDetailResponse instantiates a new ItemDetailResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewItemDetailResponseWithDefaults

`func NewItemDetailResponseWithDefaults() *ItemDetailResponse`

NewItemDetailResponseWithDefaults instantiates a new ItemDetailResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetItem

`func (o *ItemDetailResponse) GetItem() VintedItemDetail`

GetItem returns the Item field if non-nil, zero value otherwise.

### GetItemOk

`func (o *ItemDetailResponse) GetItemOk() (*VintedItemDetail, bool)`

GetItemOk returns a tuple with the Item field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItem

`func (o *ItemDetailResponse) SetItem(v VintedItemDetail)`

SetItem sets Item field to given value.


### GetMarket

`func (o *ItemDetailResponse) GetMarket() string`

GetMarket returns the Market field if non-nil, zero value otherwise.

### GetMarketOk

`func (o *ItemDetailResponse) GetMarketOk() (*string, bool)`

GetMarketOk returns a tuple with the Market field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMarket

`func (o *ItemDetailResponse) SetMarket(v string)`

SetMarket sets Market field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# PortalApiRoutersV1AsosSearchResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Market** | **string** |  | 
**SearchTerm** | Pointer to [**Searchterm**](Searchterm.md) |  | [optional] 
**CategoryName** | Pointer to [**Categoryname**](Categoryname.md) |  | [optional] 
**TotalResults** | **int32** |  | 
**Offset** | **int32** |  | 
**Limit** | **int32** |  | 
**NextOffset** | Pointer to [**NextOffset**](NextOffset.md) |  | [optional] 
**Products** | [**[]Product**](Product.md) |  | 
**Facets** | Pointer to **[]map[string]interface{}** |  | [optional] 

## Methods

### NewPortalApiRoutersV1AsosSearchResponse

`func NewPortalApiRoutersV1AsosSearchResponse(market string, totalResults int32, offset int32, limit int32, products []Product, ) *PortalApiRoutersV1AsosSearchResponse`

NewPortalApiRoutersV1AsosSearchResponse instantiates a new PortalApiRoutersV1AsosSearchResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPortalApiRoutersV1AsosSearchResponseWithDefaults

`func NewPortalApiRoutersV1AsosSearchResponseWithDefaults() *PortalApiRoutersV1AsosSearchResponse`

NewPortalApiRoutersV1AsosSearchResponseWithDefaults instantiates a new PortalApiRoutersV1AsosSearchResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMarket

`func (o *PortalApiRoutersV1AsosSearchResponse) GetMarket() string`

GetMarket returns the Market field if non-nil, zero value otherwise.

### GetMarketOk

`func (o *PortalApiRoutersV1AsosSearchResponse) GetMarketOk() (*string, bool)`

GetMarketOk returns a tuple with the Market field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMarket

`func (o *PortalApiRoutersV1AsosSearchResponse) SetMarket(v string)`

SetMarket sets Market field to given value.


### GetSearchTerm

`func (o *PortalApiRoutersV1AsosSearchResponse) GetSearchTerm() Searchterm`

GetSearchTerm returns the SearchTerm field if non-nil, zero value otherwise.

### GetSearchTermOk

`func (o *PortalApiRoutersV1AsosSearchResponse) GetSearchTermOk() (*Searchterm, bool)`

GetSearchTermOk returns a tuple with the SearchTerm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSearchTerm

`func (o *PortalApiRoutersV1AsosSearchResponse) SetSearchTerm(v Searchterm)`

SetSearchTerm sets SearchTerm field to given value.

### HasSearchTerm

`func (o *PortalApiRoutersV1AsosSearchResponse) HasSearchTerm() bool`

HasSearchTerm returns a boolean if a field has been set.

### GetCategoryName

`func (o *PortalApiRoutersV1AsosSearchResponse) GetCategoryName() Categoryname`

GetCategoryName returns the CategoryName field if non-nil, zero value otherwise.

### GetCategoryNameOk

`func (o *PortalApiRoutersV1AsosSearchResponse) GetCategoryNameOk() (*Categoryname, bool)`

GetCategoryNameOk returns a tuple with the CategoryName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategoryName

`func (o *PortalApiRoutersV1AsosSearchResponse) SetCategoryName(v Categoryname)`

SetCategoryName sets CategoryName field to given value.

### HasCategoryName

`func (o *PortalApiRoutersV1AsosSearchResponse) HasCategoryName() bool`

HasCategoryName returns a boolean if a field has been set.

### GetTotalResults

`func (o *PortalApiRoutersV1AsosSearchResponse) GetTotalResults() int32`

GetTotalResults returns the TotalResults field if non-nil, zero value otherwise.

### GetTotalResultsOk

`func (o *PortalApiRoutersV1AsosSearchResponse) GetTotalResultsOk() (*int32, bool)`

GetTotalResultsOk returns a tuple with the TotalResults field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalResults

`func (o *PortalApiRoutersV1AsosSearchResponse) SetTotalResults(v int32)`

SetTotalResults sets TotalResults field to given value.


### GetOffset

`func (o *PortalApiRoutersV1AsosSearchResponse) GetOffset() int32`

GetOffset returns the Offset field if non-nil, zero value otherwise.

### GetOffsetOk

`func (o *PortalApiRoutersV1AsosSearchResponse) GetOffsetOk() (*int32, bool)`

GetOffsetOk returns a tuple with the Offset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOffset

`func (o *PortalApiRoutersV1AsosSearchResponse) SetOffset(v int32)`

SetOffset sets Offset field to given value.


### GetLimit

`func (o *PortalApiRoutersV1AsosSearchResponse) GetLimit() int32`

GetLimit returns the Limit field if non-nil, zero value otherwise.

### GetLimitOk

`func (o *PortalApiRoutersV1AsosSearchResponse) GetLimitOk() (*int32, bool)`

GetLimitOk returns a tuple with the Limit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimit

`func (o *PortalApiRoutersV1AsosSearchResponse) SetLimit(v int32)`

SetLimit sets Limit field to given value.


### GetNextOffset

`func (o *PortalApiRoutersV1AsosSearchResponse) GetNextOffset() NextOffset`

GetNextOffset returns the NextOffset field if non-nil, zero value otherwise.

### GetNextOffsetOk

`func (o *PortalApiRoutersV1AsosSearchResponse) GetNextOffsetOk() (*NextOffset, bool)`

GetNextOffsetOk returns a tuple with the NextOffset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextOffset

`func (o *PortalApiRoutersV1AsosSearchResponse) SetNextOffset(v NextOffset)`

SetNextOffset sets NextOffset field to given value.

### HasNextOffset

`func (o *PortalApiRoutersV1AsosSearchResponse) HasNextOffset() bool`

HasNextOffset returns a boolean if a field has been set.

### GetProducts

`func (o *PortalApiRoutersV1AsosSearchResponse) GetProducts() []Product`

GetProducts returns the Products field if non-nil, zero value otherwise.

### GetProductsOk

`func (o *PortalApiRoutersV1AsosSearchResponse) GetProductsOk() (*[]Product, bool)`

GetProductsOk returns a tuple with the Products field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProducts

`func (o *PortalApiRoutersV1AsosSearchResponse) SetProducts(v []Product)`

SetProducts sets Products field to given value.


### GetFacets

`func (o *PortalApiRoutersV1AsosSearchResponse) GetFacets() []*map[string]interface{}`

GetFacets returns the Facets field if non-nil, zero value otherwise.

### GetFacetsOk

`func (o *PortalApiRoutersV1AsosSearchResponse) GetFacetsOk() (*[]*map[string]interface{}, bool)`

GetFacetsOk returns a tuple with the Facets field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFacets

`func (o *PortalApiRoutersV1AsosSearchResponse) SetFacets(v []*map[string]interface{})`

SetFacets sets Facets field to given value.

### HasFacets

`func (o *PortalApiRoutersV1AsosSearchResponse) HasFacets() bool`

HasFacets returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



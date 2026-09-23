# BrandsResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Brands** | [**[]VintedBrand**](VintedBrand.md) |  | 
**Pagination** | Pointer to [**NullableVintedPagination**](VintedPagination.md) |  | [optional] 

## Methods

### NewBrandsResponse

`func NewBrandsResponse(brands []VintedBrand, ) *BrandsResponse`

NewBrandsResponse instantiates a new BrandsResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBrandsResponseWithDefaults

`func NewBrandsResponseWithDefaults() *BrandsResponse`

NewBrandsResponseWithDefaults instantiates a new BrandsResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBrands

`func (o *BrandsResponse) GetBrands() []VintedBrand`

GetBrands returns the Brands field if non-nil, zero value otherwise.

### GetBrandsOk

`func (o *BrandsResponse) GetBrandsOk() (*[]VintedBrand, bool)`

GetBrandsOk returns a tuple with the Brands field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBrands

`func (o *BrandsResponse) SetBrands(v []VintedBrand)`

SetBrands sets Brands field to given value.


### GetPagination

`func (o *BrandsResponse) GetPagination() VintedPagination`

GetPagination returns the Pagination field if non-nil, zero value otherwise.

### GetPaginationOk

`func (o *BrandsResponse) GetPaginationOk() (*VintedPagination, bool)`

GetPaginationOk returns a tuple with the Pagination field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPagination

`func (o *BrandsResponse) SetPagination(v VintedPagination)`

SetPagination sets Pagination field to given value.

### HasPagination

`func (o *BrandsResponse) HasPagination() bool`

HasPagination returns a boolean if a field has been set.

### SetPaginationNil

`func (o *BrandsResponse) SetPaginationNil(b bool)`

 SetPaginationNil sets the value for Pagination to be an explicit nil

### UnsetPagination
`func (o *BrandsResponse) UnsetPagination()`

UnsetPagination ensures that no value is present for Pagination, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



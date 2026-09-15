# VintedMobileReadRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Market** | Pointer to **string** | Vinted market code; uk aliases gb | [optional] [default to "fr"]
**Parameters** | Pointer to **map[string]interface{}** | Operation-specific parameters. GET /v1/vinted/mobile/operations lists types, required fields and examples. | [optional] 

## Methods

### NewVintedMobileReadRequest

`func NewVintedMobileReadRequest() *VintedMobileReadRequest`

NewVintedMobileReadRequest instantiates a new VintedMobileReadRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVintedMobileReadRequestWithDefaults

`func NewVintedMobileReadRequestWithDefaults() *VintedMobileReadRequest`

NewVintedMobileReadRequestWithDefaults instantiates a new VintedMobileReadRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMarket

`func (o *VintedMobileReadRequest) GetMarket() string`

GetMarket returns the Market field if non-nil, zero value otherwise.

### GetMarketOk

`func (o *VintedMobileReadRequest) GetMarketOk() (*string, bool)`

GetMarketOk returns a tuple with the Market field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMarket

`func (o *VintedMobileReadRequest) SetMarket(v string)`

SetMarket sets Market field to given value.

### HasMarket

`func (o *VintedMobileReadRequest) HasMarket() bool`

HasMarket returns a boolean if a field has been set.

### GetParameters

`func (o *VintedMobileReadRequest) GetParameters() map[string]interface{}`

GetParameters returns the Parameters field if non-nil, zero value otherwise.

### GetParametersOk

`func (o *VintedMobileReadRequest) GetParametersOk() (*map[string]interface{}, bool)`

GetParametersOk returns a tuple with the Parameters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParameters

`func (o *VintedMobileReadRequest) SetParameters(v map[string]interface{})`

SetParameters sets Parameters field to given value.

### HasParameters

`func (o *VintedMobileReadRequest) HasParameters() bool`

HasParameters returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



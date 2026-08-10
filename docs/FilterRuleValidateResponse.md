# FilterRuleValidateResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Valid** | **bool** |  | 
**Query** | **string** |  | 
**Error** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewFilterRuleValidateResponse

`func NewFilterRuleValidateResponse(valid bool, query string, ) *FilterRuleValidateResponse`

NewFilterRuleValidateResponse instantiates a new FilterRuleValidateResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFilterRuleValidateResponseWithDefaults

`func NewFilterRuleValidateResponseWithDefaults() *FilterRuleValidateResponse`

NewFilterRuleValidateResponseWithDefaults instantiates a new FilterRuleValidateResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetValid

`func (o *FilterRuleValidateResponse) GetValid() bool`

GetValid returns the Valid field if non-nil, zero value otherwise.

### GetValidOk

`func (o *FilterRuleValidateResponse) GetValidOk() (*bool, bool)`

GetValidOk returns a tuple with the Valid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValid

`func (o *FilterRuleValidateResponse) SetValid(v bool)`

SetValid sets Valid field to given value.


### GetQuery

`func (o *FilterRuleValidateResponse) GetQuery() string`

GetQuery returns the Query field if non-nil, zero value otherwise.

### GetQueryOk

`func (o *FilterRuleValidateResponse) GetQueryOk() (*string, bool)`

GetQueryOk returns a tuple with the Query field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuery

`func (o *FilterRuleValidateResponse) SetQuery(v string)`

SetQuery sets Query field to given value.


### GetError

`func (o *FilterRuleValidateResponse) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *FilterRuleValidateResponse) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *FilterRuleValidateResponse) SetError(v string)`

SetError sets Error field to given value.

### HasError

`func (o *FilterRuleValidateResponse) HasError() bool`

HasError returns a boolean if a field has been set.

### SetErrorNil

`func (o *FilterRuleValidateResponse) SetErrorNil(b bool)`

 SetErrorNil sets the value for Error to be an explicit nil

### UnsetError
`func (o *FilterRuleValidateResponse) UnsetError()`

UnsetError ensures that no value is present for Error, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



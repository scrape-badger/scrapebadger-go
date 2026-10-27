# BatchItem

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Method** | Pointer to **string** |  | [optional] [default to "GET"]
**Path** | **string** |  | 
**Query** | Pointer to [**map[string]BatchItemQueryValue**](BatchItemQueryValue.md) |  | [optional] 

## Methods

### NewBatchItem

`func NewBatchItem(path string, ) *BatchItem`

NewBatchItem instantiates a new BatchItem object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBatchItemWithDefaults

`func NewBatchItemWithDefaults() *BatchItem`

NewBatchItemWithDefaults instantiates a new BatchItem object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMethod

`func (o *BatchItem) GetMethod() string`

GetMethod returns the Method field if non-nil, zero value otherwise.

### GetMethodOk

`func (o *BatchItem) GetMethodOk() (*string, bool)`

GetMethodOk returns a tuple with the Method field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMethod

`func (o *BatchItem) SetMethod(v string)`

SetMethod sets Method field to given value.

### HasMethod

`func (o *BatchItem) HasMethod() bool`

HasMethod returns a boolean if a field has been set.

### GetPath

`func (o *BatchItem) GetPath() string`

GetPath returns the Path field if non-nil, zero value otherwise.

### GetPathOk

`func (o *BatchItem) GetPathOk() (*string, bool)`

GetPathOk returns a tuple with the Path field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPath

`func (o *BatchItem) SetPath(v string)`

SetPath sets Path field to given value.


### GetQuery

`func (o *BatchItem) GetQuery() map[string]BatchItemQueryValue`

GetQuery returns the Query field if non-nil, zero value otherwise.

### GetQueryOk

`func (o *BatchItem) GetQueryOk() (*map[string]BatchItemQueryValue, bool)`

GetQueryOk returns a tuple with the Query field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuery

`func (o *BatchItem) SetQuery(v map[string]BatchItemQueryValue)`

SetQuery sets Query field to given value.

### HasQuery

`func (o *BatchItem) HasQuery() bool`

HasQuery returns a boolean if a field has been set.

### SetQueryNil

`func (o *BatchItem) SetQueryNil(b bool)`

 SetQueryNil sets the value for Query to be an explicit nil

### UnsetQuery
`func (o *BatchItem) UnsetQuery()`

UnsetQuery ensures that no value is present for Query, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



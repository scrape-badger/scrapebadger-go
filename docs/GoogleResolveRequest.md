# GoogleResolveRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Results** | [**[]GoogleResolveItem**](GoogleResolveItem.md) | The results to resolve, 1 to 25. Each needs a &#x60;link_token&#x60;. Any other field (&#x60;position&#x60;, &#x60;title&#x60;, your own id) is returned unchanged on its row, so the &#x60;organic_results&#x60; items of a search response can be sent as they are. | 

## Methods

### NewGoogleResolveRequest

`func NewGoogleResolveRequest(results []GoogleResolveItem, ) *GoogleResolveRequest`

NewGoogleResolveRequest instantiates a new GoogleResolveRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGoogleResolveRequestWithDefaults

`func NewGoogleResolveRequestWithDefaults() *GoogleResolveRequest`

NewGoogleResolveRequestWithDefaults instantiates a new GoogleResolveRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetResults

`func (o *GoogleResolveRequest) GetResults() []GoogleResolveItem`

GetResults returns the Results field if non-nil, zero value otherwise.

### GetResultsOk

`func (o *GoogleResolveRequest) GetResultsOk() (*[]GoogleResolveItem, bool)`

GetResultsOk returns a tuple with the Results field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResults

`func (o *GoogleResolveRequest) SetResults(v []GoogleResolveItem)`

SetResults sets Results field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



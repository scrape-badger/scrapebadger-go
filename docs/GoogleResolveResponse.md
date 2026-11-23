# GoogleResolveResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Results** | [**[]GoogleResolveRow**](GoogleResolveRow.md) | One row for each result sent, in the order sent. | 
**RetryAfterSeconds** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewGoogleResolveResponse

`func NewGoogleResolveResponse(results []GoogleResolveRow, ) *GoogleResolveResponse`

NewGoogleResolveResponse instantiates a new GoogleResolveResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGoogleResolveResponseWithDefaults

`func NewGoogleResolveResponseWithDefaults() *GoogleResolveResponse`

NewGoogleResolveResponseWithDefaults instantiates a new GoogleResolveResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetResults

`func (o *GoogleResolveResponse) GetResults() []GoogleResolveRow`

GetResults returns the Results field if non-nil, zero value otherwise.

### GetResultsOk

`func (o *GoogleResolveResponse) GetResultsOk() (*[]GoogleResolveRow, bool)`

GetResultsOk returns a tuple with the Results field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResults

`func (o *GoogleResolveResponse) SetResults(v []GoogleResolveRow)`

SetResults sets Results field to given value.


### GetRetryAfterSeconds

`func (o *GoogleResolveResponse) GetRetryAfterSeconds() int32`

GetRetryAfterSeconds returns the RetryAfterSeconds field if non-nil, zero value otherwise.

### GetRetryAfterSecondsOk

`func (o *GoogleResolveResponse) GetRetryAfterSecondsOk() (*int32, bool)`

GetRetryAfterSecondsOk returns a tuple with the RetryAfterSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRetryAfterSeconds

`func (o *GoogleResolveResponse) SetRetryAfterSeconds(v int32)`

SetRetryAfterSeconds sets RetryAfterSeconds field to given value.

### HasRetryAfterSeconds

`func (o *GoogleResolveResponse) HasRetryAfterSeconds() bool`

HasRetryAfterSeconds returns a boolean if a field has been set.

### SetRetryAfterSecondsNil

`func (o *GoogleResolveResponse) SetRetryAfterSecondsNil(b bool)`

 SetRetryAfterSecondsNil sets the value for RetryAfterSeconds to be an explicit nil

### UnsetRetryAfterSeconds
`func (o *GoogleResolveResponse) UnsetRetryAfterSeconds()`

UnsetRetryAfterSeconds ensures that no value is present for RetryAfterSeconds, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



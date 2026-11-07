# YelpHours

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Day** | **string** |  | 
**Open** | **string** | Local wall time HH:MM. | 
**Close** | **string** | Local wall time HH:MM; may be past midnight. | 

## Methods

### NewYelpHours

`func NewYelpHours(day string, open string, close string, ) *YelpHours`

NewYelpHours instantiates a new YelpHours object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewYelpHoursWithDefaults

`func NewYelpHoursWithDefaults() *YelpHours`

NewYelpHoursWithDefaults instantiates a new YelpHours object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDay

`func (o *YelpHours) GetDay() string`

GetDay returns the Day field if non-nil, zero value otherwise.

### GetDayOk

`func (o *YelpHours) GetDayOk() (*string, bool)`

GetDayOk returns a tuple with the Day field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDay

`func (o *YelpHours) SetDay(v string)`

SetDay sets Day field to given value.


### GetOpen

`func (o *YelpHours) GetOpen() string`

GetOpen returns the Open field if non-nil, zero value otherwise.

### GetOpenOk

`func (o *YelpHours) GetOpenOk() (*string, bool)`

GetOpenOk returns a tuple with the Open field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOpen

`func (o *YelpHours) SetOpen(v string)`

SetOpen sets Open field to given value.


### GetClose

`func (o *YelpHours) GetClose() string`

GetClose returns the Close field if non-nil, zero value otherwise.

### GetCloseOk

`func (o *YelpHours) GetCloseOk() (*string, bool)`

GetCloseOk returns a tuple with the Close field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClose

`func (o *YelpHours) SetClose(v string)`

SetClose sets Close field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



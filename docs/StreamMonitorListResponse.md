# StreamMonitorListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Monitors** | [**[]StreamMonitorResponse**](StreamMonitorResponse.md) |  | 
**Total** | **int32** |  | 
**Page** | **int32** |  | 
**PageSize** | **int32** |  | 

## Methods

### NewStreamMonitorListResponse

`func NewStreamMonitorListResponse(monitors []StreamMonitorResponse, total int32, page int32, pageSize int32, ) *StreamMonitorListResponse`

NewStreamMonitorListResponse instantiates a new StreamMonitorListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStreamMonitorListResponseWithDefaults

`func NewStreamMonitorListResponseWithDefaults() *StreamMonitorListResponse`

NewStreamMonitorListResponseWithDefaults instantiates a new StreamMonitorListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMonitors

`func (o *StreamMonitorListResponse) GetMonitors() []StreamMonitorResponse`

GetMonitors returns the Monitors field if non-nil, zero value otherwise.

### GetMonitorsOk

`func (o *StreamMonitorListResponse) GetMonitorsOk() (*[]StreamMonitorResponse, bool)`

GetMonitorsOk returns a tuple with the Monitors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMonitors

`func (o *StreamMonitorListResponse) SetMonitors(v []StreamMonitorResponse)`

SetMonitors sets Monitors field to given value.


### GetTotal

`func (o *StreamMonitorListResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *StreamMonitorListResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *StreamMonitorListResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.


### GetPage

`func (o *StreamMonitorListResponse) GetPage() int32`

GetPage returns the Page field if non-nil, zero value otherwise.

### GetPageOk

`func (o *StreamMonitorListResponse) GetPageOk() (*int32, bool)`

GetPageOk returns a tuple with the Page field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPage

`func (o *StreamMonitorListResponse) SetPage(v int32)`

SetPage sets Page field to given value.


### GetPageSize

`func (o *StreamMonitorListResponse) GetPageSize() int32`

GetPageSize returns the PageSize field if non-nil, zero value otherwise.

### GetPageSizeOk

`func (o *StreamMonitorListResponse) GetPageSizeOk() (*int32, bool)`

GetPageSizeOk returns a tuple with the PageSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageSize

`func (o *StreamMonitorListResponse) SetPageSize(v int32)`

SetPageSize sets PageSize field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



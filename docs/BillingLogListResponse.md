# BillingLogListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Logs** | [**[]BillingLogResponse**](BillingLogResponse.md) |  | 
**Total** | **int32** |  | 
**Page** | **int32** |  | 
**PageSize** | **int32** |  | 

## Methods

### NewBillingLogListResponse

`func NewBillingLogListResponse(logs []BillingLogResponse, total int32, page int32, pageSize int32, ) *BillingLogListResponse`

NewBillingLogListResponse instantiates a new BillingLogListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBillingLogListResponseWithDefaults

`func NewBillingLogListResponseWithDefaults() *BillingLogListResponse`

NewBillingLogListResponseWithDefaults instantiates a new BillingLogListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLogs

`func (o *BillingLogListResponse) GetLogs() []BillingLogResponse`

GetLogs returns the Logs field if non-nil, zero value otherwise.

### GetLogsOk

`func (o *BillingLogListResponse) GetLogsOk() (*[]BillingLogResponse, bool)`

GetLogsOk returns a tuple with the Logs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogs

`func (o *BillingLogListResponse) SetLogs(v []BillingLogResponse)`

SetLogs sets Logs field to given value.


### GetTotal

`func (o *BillingLogListResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *BillingLogListResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *BillingLogListResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.


### GetPage

`func (o *BillingLogListResponse) GetPage() int32`

GetPage returns the Page field if non-nil, zero value otherwise.

### GetPageOk

`func (o *BillingLogListResponse) GetPageOk() (*int32, bool)`

GetPageOk returns a tuple with the Page field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPage

`func (o *BillingLogListResponse) SetPage(v int32)`

SetPage sets Page field to given value.


### GetPageSize

`func (o *BillingLogListResponse) GetPageSize() int32`

GetPageSize returns the PageSize field if non-nil, zero value otherwise.

### GetPageSizeOk

`func (o *BillingLogListResponse) GetPageSizeOk() (*int32, bool)`

GetPageSizeOk returns a tuple with the PageSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageSize

`func (o *BillingLogListResponse) SetPageSize(v int32)`

SetPageSize sets PageSize field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



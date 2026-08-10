# FilterRuleListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Rules** | [**[]FilterRuleResponse**](FilterRuleResponse.md) |  | 
**Total** | **int32** |  | 
**Page** | **int32** |  | 
**PageSize** | **int32** |  | 

## Methods

### NewFilterRuleListResponse

`func NewFilterRuleListResponse(rules []FilterRuleResponse, total int32, page int32, pageSize int32, ) *FilterRuleListResponse`

NewFilterRuleListResponse instantiates a new FilterRuleListResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFilterRuleListResponseWithDefaults

`func NewFilterRuleListResponseWithDefaults() *FilterRuleListResponse`

NewFilterRuleListResponseWithDefaults instantiates a new FilterRuleListResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRules

`func (o *FilterRuleListResponse) GetRules() []FilterRuleResponse`

GetRules returns the Rules field if non-nil, zero value otherwise.

### GetRulesOk

`func (o *FilterRuleListResponse) GetRulesOk() (*[]FilterRuleResponse, bool)`

GetRulesOk returns a tuple with the Rules field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRules

`func (o *FilterRuleListResponse) SetRules(v []FilterRuleResponse)`

SetRules sets Rules field to given value.


### GetTotal

`func (o *FilterRuleListResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *FilterRuleListResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *FilterRuleListResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.


### GetPage

`func (o *FilterRuleListResponse) GetPage() int32`

GetPage returns the Page field if non-nil, zero value otherwise.

### GetPageOk

`func (o *FilterRuleListResponse) GetPageOk() (*int32, bool)`

GetPageOk returns a tuple with the Page field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPage

`func (o *FilterRuleListResponse) SetPage(v int32)`

SetPage sets Page field to given value.


### GetPageSize

`func (o *FilterRuleListResponse) GetPageSize() int32`

GetPageSize returns the PageSize field if non-nil, zero value otherwise.

### GetPageSizeOk

`func (o *FilterRuleListResponse) GetPageSizeOk() (*int32, bool)`

GetPageSizeOk returns a tuple with the PageSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageSize

`func (o *FilterRuleListResponse) SetPageSize(v int32)`

SetPageSize sets PageSize field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# WebhookListItem

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**MonitorId** | **string** |  | 
**MonitorName** | **string** |  | 
**Url** | **string** |  | 
**SecretSet** | **bool** |  | 
**CreatedAt** | **time.Time** |  | 

## Methods

### NewWebhookListItem

`func NewWebhookListItem(id string, monitorId string, monitorName string, url string, secretSet bool, createdAt time.Time, ) *WebhookListItem`

NewWebhookListItem instantiates a new WebhookListItem object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebhookListItemWithDefaults

`func NewWebhookListItemWithDefaults() *WebhookListItem`

NewWebhookListItemWithDefaults instantiates a new WebhookListItem object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *WebhookListItem) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *WebhookListItem) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *WebhookListItem) SetId(v string)`

SetId sets Id field to given value.


### GetMonitorId

`func (o *WebhookListItem) GetMonitorId() string`

GetMonitorId returns the MonitorId field if non-nil, zero value otherwise.

### GetMonitorIdOk

`func (o *WebhookListItem) GetMonitorIdOk() (*string, bool)`

GetMonitorIdOk returns a tuple with the MonitorId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMonitorId

`func (o *WebhookListItem) SetMonitorId(v string)`

SetMonitorId sets MonitorId field to given value.


### GetMonitorName

`func (o *WebhookListItem) GetMonitorName() string`

GetMonitorName returns the MonitorName field if non-nil, zero value otherwise.

### GetMonitorNameOk

`func (o *WebhookListItem) GetMonitorNameOk() (*string, bool)`

GetMonitorNameOk returns a tuple with the MonitorName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMonitorName

`func (o *WebhookListItem) SetMonitorName(v string)`

SetMonitorName sets MonitorName field to given value.


### GetUrl

`func (o *WebhookListItem) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *WebhookListItem) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *WebhookListItem) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetSecretSet

`func (o *WebhookListItem) GetSecretSet() bool`

GetSecretSet returns the SecretSet field if non-nil, zero value otherwise.

### GetSecretSetOk

`func (o *WebhookListItem) GetSecretSetOk() (*bool, bool)`

GetSecretSetOk returns a tuple with the SecretSet field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecretSet

`func (o *WebhookListItem) SetSecretSet(v bool)`

SetSecretSet sets SecretSet field to given value.


### GetCreatedAt

`func (o *WebhookListItem) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *WebhookListItem) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *WebhookListItem) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



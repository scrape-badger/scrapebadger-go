# WebhookDeliveries

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Deliveries** | [**[]WebhookDelivery**](WebhookDelivery.md) |  | 
**WindowHours** | **int32** |  | 

## Methods

### NewWebhookDeliveries

`func NewWebhookDeliveries(deliveries []WebhookDelivery, windowHours int32, ) *WebhookDeliveries`

NewWebhookDeliveries instantiates a new WebhookDeliveries object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebhookDeliveriesWithDefaults

`func NewWebhookDeliveriesWithDefaults() *WebhookDeliveries`

NewWebhookDeliveriesWithDefaults instantiates a new WebhookDeliveries object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDeliveries

`func (o *WebhookDeliveries) GetDeliveries() []WebhookDelivery`

GetDeliveries returns the Deliveries field if non-nil, zero value otherwise.

### GetDeliveriesOk

`func (o *WebhookDeliveries) GetDeliveriesOk() (*[]WebhookDelivery, bool)`

GetDeliveriesOk returns a tuple with the Deliveries field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeliveries

`func (o *WebhookDeliveries) SetDeliveries(v []WebhookDelivery)`

SetDeliveries sets Deliveries field to given value.


### GetWindowHours

`func (o *WebhookDeliveries) GetWindowHours() int32`

GetWindowHours returns the WindowHours field if non-nil, zero value otherwise.

### GetWindowHoursOk

`func (o *WebhookDeliveries) GetWindowHoursOk() (*int32, bool)`

GetWindowHoursOk returns a tuple with the WindowHours field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWindowHours

`func (o *WebhookDeliveries) SetWindowHours(v int32)`

SetWindowHours sets WindowHours field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



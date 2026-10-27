# WebhookSecret

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Secret** | **string** |  | 
**SignatureHeader** | Pointer to **string** |  | [optional] [default to "X-ScrapeBadger-Signature"]
**Algorithm** | Pointer to **string** |  | [optional] [default to "sha256=<hex HMAC-SHA256 of the raw request body>"]

## Methods

### NewWebhookSecret

`func NewWebhookSecret(secret string, ) *WebhookSecret`

NewWebhookSecret instantiates a new WebhookSecret object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebhookSecretWithDefaults

`func NewWebhookSecretWithDefaults() *WebhookSecret`

NewWebhookSecretWithDefaults instantiates a new WebhookSecret object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSecret

`func (o *WebhookSecret) GetSecret() string`

GetSecret returns the Secret field if non-nil, zero value otherwise.

### GetSecretOk

`func (o *WebhookSecret) GetSecretOk() (*string, bool)`

GetSecretOk returns a tuple with the Secret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecret

`func (o *WebhookSecret) SetSecret(v string)`

SetSecret sets Secret field to given value.


### GetSignatureHeader

`func (o *WebhookSecret) GetSignatureHeader() string`

GetSignatureHeader returns the SignatureHeader field if non-nil, zero value otherwise.

### GetSignatureHeaderOk

`func (o *WebhookSecret) GetSignatureHeaderOk() (*string, bool)`

GetSignatureHeaderOk returns a tuple with the SignatureHeader field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSignatureHeader

`func (o *WebhookSecret) SetSignatureHeader(v string)`

SetSignatureHeader sets SignatureHeader field to given value.

### HasSignatureHeader

`func (o *WebhookSecret) HasSignatureHeader() bool`

HasSignatureHeader returns a boolean if a field has been set.

### GetAlgorithm

`func (o *WebhookSecret) GetAlgorithm() string`

GetAlgorithm returns the Algorithm field if non-nil, zero value otherwise.

### GetAlgorithmOk

`func (o *WebhookSecret) GetAlgorithmOk() (*string, bool)`

GetAlgorithmOk returns a tuple with the Algorithm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAlgorithm

`func (o *WebhookSecret) SetAlgorithm(v string)`

SetAlgorithm sets Algorithm field to given value.

### HasAlgorithm

`func (o *WebhookSecret) HasAlgorithm() bool`

HasAlgorithm returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



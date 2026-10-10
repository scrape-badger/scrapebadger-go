# ExtractRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Url** | **string** | The page to fetch. | 
**WaitFor** | Pointer to **NullableString** |  | [optional] 
**Country** | Pointer to **NullableString** |  | [optional] 
**ProxyTier** | Pointer to **string** | Proxy pool: simple, premium or ultra. | [optional] [default to "simple"]
**ExtractRules** | Pointer to [**map[string]ExtractRequestExtractRulesValue**](ExtractRequestExtractRulesValue.md) |  | [optional] 
**AiExtractRules** | Pointer to **map[string]string** |  | [optional] 
**AiQuery** | Pointer to **NullableString** |  | [optional] 
**RenderJs** | Pointer to **bool** | Render the page in a browser first. | [optional] [default to false]

## Methods

### NewExtractRequest

`func NewExtractRequest(url string, ) *ExtractRequest`

NewExtractRequest instantiates a new ExtractRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExtractRequestWithDefaults

`func NewExtractRequestWithDefaults() *ExtractRequest`

NewExtractRequestWithDefaults instantiates a new ExtractRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUrl

`func (o *ExtractRequest) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *ExtractRequest) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *ExtractRequest) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetWaitFor

`func (o *ExtractRequest) GetWaitFor() string`

GetWaitFor returns the WaitFor field if non-nil, zero value otherwise.

### GetWaitForOk

`func (o *ExtractRequest) GetWaitForOk() (*string, bool)`

GetWaitForOk returns a tuple with the WaitFor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWaitFor

`func (o *ExtractRequest) SetWaitFor(v string)`

SetWaitFor sets WaitFor field to given value.

### HasWaitFor

`func (o *ExtractRequest) HasWaitFor() bool`

HasWaitFor returns a boolean if a field has been set.

### SetWaitForNil

`func (o *ExtractRequest) SetWaitForNil(b bool)`

 SetWaitForNil sets the value for WaitFor to be an explicit nil

### UnsetWaitFor
`func (o *ExtractRequest) UnsetWaitFor()`

UnsetWaitFor ensures that no value is present for WaitFor, not even an explicit nil
### GetCountry

`func (o *ExtractRequest) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *ExtractRequest) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *ExtractRequest) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *ExtractRequest) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### SetCountryNil

`func (o *ExtractRequest) SetCountryNil(b bool)`

 SetCountryNil sets the value for Country to be an explicit nil

### UnsetCountry
`func (o *ExtractRequest) UnsetCountry()`

UnsetCountry ensures that no value is present for Country, not even an explicit nil
### GetProxyTier

`func (o *ExtractRequest) GetProxyTier() string`

GetProxyTier returns the ProxyTier field if non-nil, zero value otherwise.

### GetProxyTierOk

`func (o *ExtractRequest) GetProxyTierOk() (*string, bool)`

GetProxyTierOk returns a tuple with the ProxyTier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProxyTier

`func (o *ExtractRequest) SetProxyTier(v string)`

SetProxyTier sets ProxyTier field to given value.

### HasProxyTier

`func (o *ExtractRequest) HasProxyTier() bool`

HasProxyTier returns a boolean if a field has been set.

### GetExtractRules

`func (o *ExtractRequest) GetExtractRules() map[string]ExtractRequestExtractRulesValue`

GetExtractRules returns the ExtractRules field if non-nil, zero value otherwise.

### GetExtractRulesOk

`func (o *ExtractRequest) GetExtractRulesOk() (*map[string]ExtractRequestExtractRulesValue, bool)`

GetExtractRulesOk returns a tuple with the ExtractRules field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExtractRules

`func (o *ExtractRequest) SetExtractRules(v map[string]ExtractRequestExtractRulesValue)`

SetExtractRules sets ExtractRules field to given value.

### HasExtractRules

`func (o *ExtractRequest) HasExtractRules() bool`

HasExtractRules returns a boolean if a field has been set.

### SetExtractRulesNil

`func (o *ExtractRequest) SetExtractRulesNil(b bool)`

 SetExtractRulesNil sets the value for ExtractRules to be an explicit nil

### UnsetExtractRules
`func (o *ExtractRequest) UnsetExtractRules()`

UnsetExtractRules ensures that no value is present for ExtractRules, not even an explicit nil
### GetAiExtractRules

`func (o *ExtractRequest) GetAiExtractRules() map[string]string`

GetAiExtractRules returns the AiExtractRules field if non-nil, zero value otherwise.

### GetAiExtractRulesOk

`func (o *ExtractRequest) GetAiExtractRulesOk() (*map[string]string, bool)`

GetAiExtractRulesOk returns a tuple with the AiExtractRules field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAiExtractRules

`func (o *ExtractRequest) SetAiExtractRules(v map[string]string)`

SetAiExtractRules sets AiExtractRules field to given value.

### HasAiExtractRules

`func (o *ExtractRequest) HasAiExtractRules() bool`

HasAiExtractRules returns a boolean if a field has been set.

### SetAiExtractRulesNil

`func (o *ExtractRequest) SetAiExtractRulesNil(b bool)`

 SetAiExtractRulesNil sets the value for AiExtractRules to be an explicit nil

### UnsetAiExtractRules
`func (o *ExtractRequest) UnsetAiExtractRules()`

UnsetAiExtractRules ensures that no value is present for AiExtractRules, not even an explicit nil
### GetAiQuery

`func (o *ExtractRequest) GetAiQuery() string`

GetAiQuery returns the AiQuery field if non-nil, zero value otherwise.

### GetAiQueryOk

`func (o *ExtractRequest) GetAiQueryOk() (*string, bool)`

GetAiQueryOk returns a tuple with the AiQuery field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAiQuery

`func (o *ExtractRequest) SetAiQuery(v string)`

SetAiQuery sets AiQuery field to given value.

### HasAiQuery

`func (o *ExtractRequest) HasAiQuery() bool`

HasAiQuery returns a boolean if a field has been set.

### SetAiQueryNil

`func (o *ExtractRequest) SetAiQueryNil(b bool)`

 SetAiQueryNil sets the value for AiQuery to be an explicit nil

### UnsetAiQuery
`func (o *ExtractRequest) UnsetAiQuery()`

UnsetAiQuery ensures that no value is present for AiQuery, not even an explicit nil
### GetRenderJs

`func (o *ExtractRequest) GetRenderJs() bool`

GetRenderJs returns the RenderJs field if non-nil, zero value otherwise.

### GetRenderJsOk

`func (o *ExtractRequest) GetRenderJsOk() (*bool, bool)`

GetRenderJsOk returns a tuple with the RenderJs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRenderJs

`func (o *ExtractRequest) SetRenderJs(v bool)`

SetRenderJs sets RenderJs field to given value.

### HasRenderJs

`func (o *ExtractRequest) HasRenderJs() bool`

HasRenderJs returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



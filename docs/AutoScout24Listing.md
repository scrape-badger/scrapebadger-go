# AutoScout24Listing

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**CrossReferenceId** | Pointer to **NullableString** |  | [optional] 
**Position** | **int32** |  | 
**Title** | **string** |  | 
**Url** | **string** |  | 
**Images** | Pointer to **[]string** |  | [optional] 
**OnlinePurchaseImages** | Pointer to **[]string** |  | [optional] 
**Price** | Pointer to **NullableFloat32** |  | [optional] 
**Currency** | Pointer to **string** |  | [optional] [default to "EUR"]
**PriceFormatted** | Pointer to **NullableString** |  | [optional] 
**PriceEvaluation** | Pointer to **NullableInt32** |  | [optional] 
**PriceEvaluationEnabled** | Pointer to **NullableBool** |  | [optional] 
**PriceDetails** | Pointer to **map[string]interface{}** |  | [optional] 
**OldPriceFormatted** | Pointer to **NullableString** |  | [optional] 
**IsSuperDeal** | Pointer to **NullableBool** |  | [optional] 
**IsConditionalPrice** | Pointer to **NullableBool** |  | [optional] 
**VatLabelRequired** | Pointer to **NullableBool** |  | [optional] 
**Make** | Pointer to **NullableString** |  | [optional] 
**Model** | Pointer to **NullableString** |  | [optional] 
**ModelId** | Pointer to **NullableInt32** |  | [optional] 
**ModelGroup** | Pointer to **NullableString** |  | [optional] 
**Variant** | Pointer to **NullableString** |  | [optional] 
**MotorType** | Pointer to **NullableString** |  | [optional] 
**Version** | Pointer to **NullableString** |  | [optional] 
**Subtitle** | Pointer to **NullableString** |  | [optional] 
**ArticleType** | Pointer to **NullableString** |  | [optional] 
**OfferType** | Pointer to **NullableString** |  | [optional] 
**Fuel** | Pointer to **NullableString** |  | [optional] 
**FuelType** | Pointer to **NullableString** |  | [optional] 
**Transmission** | Pointer to **NullableString** |  | [optional] 
**MileageKm** | Pointer to **NullableInt32** |  | [optional] 
**FirstRegistration** | Pointer to **NullableString** |  | [optional] 
**RegistrationYear** | Pointer to **NullableInt32** |  | [optional] 
**RegistrationMonth** | Pointer to **NullableInt32** |  | [optional] 
**PowerKw** | Pointer to **NullableFloat32** |  | [optional] 
**PowerHp** | Pointer to **NullableFloat32** |  | [optional] 
**DisplacementCc** | Pointer to **NullableInt32** |  | [optional] 
**IsDamaged** | Pointer to **NullableBool** |  | [optional] 
**AvailableNow** | Pointer to **NullableBool** |  | [optional] 
**AvailableAt** | Pointer to **NullableString** |  | [optional] 
**AvailableUtc** | Pointer to **NullableFloat32** |  | [optional] 
**AvailabilityInDays** | Pointer to **NullableInt32** |  | [optional] 
**Location** | Pointer to **map[string]interface{}** |  | [optional] 
**Seller** | Pointer to **map[string]interface{}** |  | [optional] 
**Rating** | Pointer to **NullableFloat32** |  | [optional] 
**RatingCount** | Pointer to **NullableInt32** |  | [optional] 
**RatingsEnabled** | Pointer to **NullableBool** |  | [optional] 
**Leasing** | Pointer to **map[string]interface{}** |  | [optional] 
**Seals** | Pointer to **[]map[string]interface{}** |  | [optional] 
**OnlinePurchase** | Pointer to **map[string]interface{}** |  | [optional] 
**ElectricVehicleBanner** | Pointer to **map[string]interface{}** |  | [optional] 
**IsDeliverable** | Pointer to **NullableBool** |  | [optional] 
**HasVideo** | Pointer to **NullableBool** |  | [optional] 
**Has360Image** | Pointer to **NullableBool** |  | [optional] 
**InterestLevel** | Pointer to **NullableString** |  | [optional] 
**IsTrending** | Pointer to **NullableBool** |  | [optional] 
**AdTier** | Pointer to **NullableString** |  | [optional] 
**ResultType** | Pointer to **NullableString** |  | [optional] 
**ResultSection** | Pointer to **NullableString** |  | [optional] 
**SpecialConditions** | Pointer to **[]interface{}** |  | [optional] 
**VehicleDetails** | Pointer to **[]map[string]interface{}** |  | [optional] 
**WltpValues** | Pointer to **[]string** |  | [optional] 
**Vehicle** | Pointer to **map[string]interface{}** | Additional native vehicle attributes, including localized labels. | [optional] 

## Methods

### NewAutoScout24Listing

`func NewAutoScout24Listing(id string, position int32, title string, url string, ) *AutoScout24Listing`

NewAutoScout24Listing instantiates a new AutoScout24Listing object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAutoScout24ListingWithDefaults

`func NewAutoScout24ListingWithDefaults() *AutoScout24Listing`

NewAutoScout24ListingWithDefaults instantiates a new AutoScout24Listing object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *AutoScout24Listing) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *AutoScout24Listing) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *AutoScout24Listing) SetId(v string)`

SetId sets Id field to given value.


### GetCrossReferenceId

`func (o *AutoScout24Listing) GetCrossReferenceId() string`

GetCrossReferenceId returns the CrossReferenceId field if non-nil, zero value otherwise.

### GetCrossReferenceIdOk

`func (o *AutoScout24Listing) GetCrossReferenceIdOk() (*string, bool)`

GetCrossReferenceIdOk returns a tuple with the CrossReferenceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCrossReferenceId

`func (o *AutoScout24Listing) SetCrossReferenceId(v string)`

SetCrossReferenceId sets CrossReferenceId field to given value.

### HasCrossReferenceId

`func (o *AutoScout24Listing) HasCrossReferenceId() bool`

HasCrossReferenceId returns a boolean if a field has been set.

### SetCrossReferenceIdNil

`func (o *AutoScout24Listing) SetCrossReferenceIdNil(b bool)`

 SetCrossReferenceIdNil sets the value for CrossReferenceId to be an explicit nil

### UnsetCrossReferenceId
`func (o *AutoScout24Listing) UnsetCrossReferenceId()`

UnsetCrossReferenceId ensures that no value is present for CrossReferenceId, not even an explicit nil
### GetPosition

`func (o *AutoScout24Listing) GetPosition() int32`

GetPosition returns the Position field if non-nil, zero value otherwise.

### GetPositionOk

`func (o *AutoScout24Listing) GetPositionOk() (*int32, bool)`

GetPositionOk returns a tuple with the Position field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPosition

`func (o *AutoScout24Listing) SetPosition(v int32)`

SetPosition sets Position field to given value.


### GetTitle

`func (o *AutoScout24Listing) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *AutoScout24Listing) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *AutoScout24Listing) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetUrl

`func (o *AutoScout24Listing) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *AutoScout24Listing) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *AutoScout24Listing) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetImages

`func (o *AutoScout24Listing) GetImages() []string`

GetImages returns the Images field if non-nil, zero value otherwise.

### GetImagesOk

`func (o *AutoScout24Listing) GetImagesOk() (*[]string, bool)`

GetImagesOk returns a tuple with the Images field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImages

`func (o *AutoScout24Listing) SetImages(v []string)`

SetImages sets Images field to given value.

### HasImages

`func (o *AutoScout24Listing) HasImages() bool`

HasImages returns a boolean if a field has been set.

### GetOnlinePurchaseImages

`func (o *AutoScout24Listing) GetOnlinePurchaseImages() []string`

GetOnlinePurchaseImages returns the OnlinePurchaseImages field if non-nil, zero value otherwise.

### GetOnlinePurchaseImagesOk

`func (o *AutoScout24Listing) GetOnlinePurchaseImagesOk() (*[]string, bool)`

GetOnlinePurchaseImagesOk returns a tuple with the OnlinePurchaseImages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOnlinePurchaseImages

`func (o *AutoScout24Listing) SetOnlinePurchaseImages(v []string)`

SetOnlinePurchaseImages sets OnlinePurchaseImages field to given value.

### HasOnlinePurchaseImages

`func (o *AutoScout24Listing) HasOnlinePurchaseImages() bool`

HasOnlinePurchaseImages returns a boolean if a field has been set.

### GetPrice

`func (o *AutoScout24Listing) GetPrice() float32`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *AutoScout24Listing) GetPriceOk() (*float32, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *AutoScout24Listing) SetPrice(v float32)`

SetPrice sets Price field to given value.

### HasPrice

`func (o *AutoScout24Listing) HasPrice() bool`

HasPrice returns a boolean if a field has been set.

### SetPriceNil

`func (o *AutoScout24Listing) SetPriceNil(b bool)`

 SetPriceNil sets the value for Price to be an explicit nil

### UnsetPrice
`func (o *AutoScout24Listing) UnsetPrice()`

UnsetPrice ensures that no value is present for Price, not even an explicit nil
### GetCurrency

`func (o *AutoScout24Listing) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *AutoScout24Listing) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *AutoScout24Listing) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *AutoScout24Listing) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetPriceFormatted

`func (o *AutoScout24Listing) GetPriceFormatted() string`

GetPriceFormatted returns the PriceFormatted field if non-nil, zero value otherwise.

### GetPriceFormattedOk

`func (o *AutoScout24Listing) GetPriceFormattedOk() (*string, bool)`

GetPriceFormattedOk returns a tuple with the PriceFormatted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceFormatted

`func (o *AutoScout24Listing) SetPriceFormatted(v string)`

SetPriceFormatted sets PriceFormatted field to given value.

### HasPriceFormatted

`func (o *AutoScout24Listing) HasPriceFormatted() bool`

HasPriceFormatted returns a boolean if a field has been set.

### SetPriceFormattedNil

`func (o *AutoScout24Listing) SetPriceFormattedNil(b bool)`

 SetPriceFormattedNil sets the value for PriceFormatted to be an explicit nil

### UnsetPriceFormatted
`func (o *AutoScout24Listing) UnsetPriceFormatted()`

UnsetPriceFormatted ensures that no value is present for PriceFormatted, not even an explicit nil
### GetPriceEvaluation

`func (o *AutoScout24Listing) GetPriceEvaluation() int32`

GetPriceEvaluation returns the PriceEvaluation field if non-nil, zero value otherwise.

### GetPriceEvaluationOk

`func (o *AutoScout24Listing) GetPriceEvaluationOk() (*int32, bool)`

GetPriceEvaluationOk returns a tuple with the PriceEvaluation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceEvaluation

`func (o *AutoScout24Listing) SetPriceEvaluation(v int32)`

SetPriceEvaluation sets PriceEvaluation field to given value.

### HasPriceEvaluation

`func (o *AutoScout24Listing) HasPriceEvaluation() bool`

HasPriceEvaluation returns a boolean if a field has been set.

### SetPriceEvaluationNil

`func (o *AutoScout24Listing) SetPriceEvaluationNil(b bool)`

 SetPriceEvaluationNil sets the value for PriceEvaluation to be an explicit nil

### UnsetPriceEvaluation
`func (o *AutoScout24Listing) UnsetPriceEvaluation()`

UnsetPriceEvaluation ensures that no value is present for PriceEvaluation, not even an explicit nil
### GetPriceEvaluationEnabled

`func (o *AutoScout24Listing) GetPriceEvaluationEnabled() bool`

GetPriceEvaluationEnabled returns the PriceEvaluationEnabled field if non-nil, zero value otherwise.

### GetPriceEvaluationEnabledOk

`func (o *AutoScout24Listing) GetPriceEvaluationEnabledOk() (*bool, bool)`

GetPriceEvaluationEnabledOk returns a tuple with the PriceEvaluationEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceEvaluationEnabled

`func (o *AutoScout24Listing) SetPriceEvaluationEnabled(v bool)`

SetPriceEvaluationEnabled sets PriceEvaluationEnabled field to given value.

### HasPriceEvaluationEnabled

`func (o *AutoScout24Listing) HasPriceEvaluationEnabled() bool`

HasPriceEvaluationEnabled returns a boolean if a field has been set.

### SetPriceEvaluationEnabledNil

`func (o *AutoScout24Listing) SetPriceEvaluationEnabledNil(b bool)`

 SetPriceEvaluationEnabledNil sets the value for PriceEvaluationEnabled to be an explicit nil

### UnsetPriceEvaluationEnabled
`func (o *AutoScout24Listing) UnsetPriceEvaluationEnabled()`

UnsetPriceEvaluationEnabled ensures that no value is present for PriceEvaluationEnabled, not even an explicit nil
### GetPriceDetails

`func (o *AutoScout24Listing) GetPriceDetails() map[string]interface{}`

GetPriceDetails returns the PriceDetails field if non-nil, zero value otherwise.

### GetPriceDetailsOk

`func (o *AutoScout24Listing) GetPriceDetailsOk() (*map[string]interface{}, bool)`

GetPriceDetailsOk returns a tuple with the PriceDetails field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceDetails

`func (o *AutoScout24Listing) SetPriceDetails(v map[string]interface{})`

SetPriceDetails sets PriceDetails field to given value.

### HasPriceDetails

`func (o *AutoScout24Listing) HasPriceDetails() bool`

HasPriceDetails returns a boolean if a field has been set.

### GetOldPriceFormatted

`func (o *AutoScout24Listing) GetOldPriceFormatted() string`

GetOldPriceFormatted returns the OldPriceFormatted field if non-nil, zero value otherwise.

### GetOldPriceFormattedOk

`func (o *AutoScout24Listing) GetOldPriceFormattedOk() (*string, bool)`

GetOldPriceFormattedOk returns a tuple with the OldPriceFormatted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOldPriceFormatted

`func (o *AutoScout24Listing) SetOldPriceFormatted(v string)`

SetOldPriceFormatted sets OldPriceFormatted field to given value.

### HasOldPriceFormatted

`func (o *AutoScout24Listing) HasOldPriceFormatted() bool`

HasOldPriceFormatted returns a boolean if a field has been set.

### SetOldPriceFormattedNil

`func (o *AutoScout24Listing) SetOldPriceFormattedNil(b bool)`

 SetOldPriceFormattedNil sets the value for OldPriceFormatted to be an explicit nil

### UnsetOldPriceFormatted
`func (o *AutoScout24Listing) UnsetOldPriceFormatted()`

UnsetOldPriceFormatted ensures that no value is present for OldPriceFormatted, not even an explicit nil
### GetIsSuperDeal

`func (o *AutoScout24Listing) GetIsSuperDeal() bool`

GetIsSuperDeal returns the IsSuperDeal field if non-nil, zero value otherwise.

### GetIsSuperDealOk

`func (o *AutoScout24Listing) GetIsSuperDealOk() (*bool, bool)`

GetIsSuperDealOk returns a tuple with the IsSuperDeal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsSuperDeal

`func (o *AutoScout24Listing) SetIsSuperDeal(v bool)`

SetIsSuperDeal sets IsSuperDeal field to given value.

### HasIsSuperDeal

`func (o *AutoScout24Listing) HasIsSuperDeal() bool`

HasIsSuperDeal returns a boolean if a field has been set.

### SetIsSuperDealNil

`func (o *AutoScout24Listing) SetIsSuperDealNil(b bool)`

 SetIsSuperDealNil sets the value for IsSuperDeal to be an explicit nil

### UnsetIsSuperDeal
`func (o *AutoScout24Listing) UnsetIsSuperDeal()`

UnsetIsSuperDeal ensures that no value is present for IsSuperDeal, not even an explicit nil
### GetIsConditionalPrice

`func (o *AutoScout24Listing) GetIsConditionalPrice() bool`

GetIsConditionalPrice returns the IsConditionalPrice field if non-nil, zero value otherwise.

### GetIsConditionalPriceOk

`func (o *AutoScout24Listing) GetIsConditionalPriceOk() (*bool, bool)`

GetIsConditionalPriceOk returns a tuple with the IsConditionalPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsConditionalPrice

`func (o *AutoScout24Listing) SetIsConditionalPrice(v bool)`

SetIsConditionalPrice sets IsConditionalPrice field to given value.

### HasIsConditionalPrice

`func (o *AutoScout24Listing) HasIsConditionalPrice() bool`

HasIsConditionalPrice returns a boolean if a field has been set.

### SetIsConditionalPriceNil

`func (o *AutoScout24Listing) SetIsConditionalPriceNil(b bool)`

 SetIsConditionalPriceNil sets the value for IsConditionalPrice to be an explicit nil

### UnsetIsConditionalPrice
`func (o *AutoScout24Listing) UnsetIsConditionalPrice()`

UnsetIsConditionalPrice ensures that no value is present for IsConditionalPrice, not even an explicit nil
### GetVatLabelRequired

`func (o *AutoScout24Listing) GetVatLabelRequired() bool`

GetVatLabelRequired returns the VatLabelRequired field if non-nil, zero value otherwise.

### GetVatLabelRequiredOk

`func (o *AutoScout24Listing) GetVatLabelRequiredOk() (*bool, bool)`

GetVatLabelRequiredOk returns a tuple with the VatLabelRequired field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVatLabelRequired

`func (o *AutoScout24Listing) SetVatLabelRequired(v bool)`

SetVatLabelRequired sets VatLabelRequired field to given value.

### HasVatLabelRequired

`func (o *AutoScout24Listing) HasVatLabelRequired() bool`

HasVatLabelRequired returns a boolean if a field has been set.

### SetVatLabelRequiredNil

`func (o *AutoScout24Listing) SetVatLabelRequiredNil(b bool)`

 SetVatLabelRequiredNil sets the value for VatLabelRequired to be an explicit nil

### UnsetVatLabelRequired
`func (o *AutoScout24Listing) UnsetVatLabelRequired()`

UnsetVatLabelRequired ensures that no value is present for VatLabelRequired, not even an explicit nil
### GetMake

`func (o *AutoScout24Listing) GetMake() string`

GetMake returns the Make field if non-nil, zero value otherwise.

### GetMakeOk

`func (o *AutoScout24Listing) GetMakeOk() (*string, bool)`

GetMakeOk returns a tuple with the Make field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMake

`func (o *AutoScout24Listing) SetMake(v string)`

SetMake sets Make field to given value.

### HasMake

`func (o *AutoScout24Listing) HasMake() bool`

HasMake returns a boolean if a field has been set.

### SetMakeNil

`func (o *AutoScout24Listing) SetMakeNil(b bool)`

 SetMakeNil sets the value for Make to be an explicit nil

### UnsetMake
`func (o *AutoScout24Listing) UnsetMake()`

UnsetMake ensures that no value is present for Make, not even an explicit nil
### GetModel

`func (o *AutoScout24Listing) GetModel() string`

GetModel returns the Model field if non-nil, zero value otherwise.

### GetModelOk

`func (o *AutoScout24Listing) GetModelOk() (*string, bool)`

GetModelOk returns a tuple with the Model field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModel

`func (o *AutoScout24Listing) SetModel(v string)`

SetModel sets Model field to given value.

### HasModel

`func (o *AutoScout24Listing) HasModel() bool`

HasModel returns a boolean if a field has been set.

### SetModelNil

`func (o *AutoScout24Listing) SetModelNil(b bool)`

 SetModelNil sets the value for Model to be an explicit nil

### UnsetModel
`func (o *AutoScout24Listing) UnsetModel()`

UnsetModel ensures that no value is present for Model, not even an explicit nil
### GetModelId

`func (o *AutoScout24Listing) GetModelId() int32`

GetModelId returns the ModelId field if non-nil, zero value otherwise.

### GetModelIdOk

`func (o *AutoScout24Listing) GetModelIdOk() (*int32, bool)`

GetModelIdOk returns a tuple with the ModelId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModelId

`func (o *AutoScout24Listing) SetModelId(v int32)`

SetModelId sets ModelId field to given value.

### HasModelId

`func (o *AutoScout24Listing) HasModelId() bool`

HasModelId returns a boolean if a field has been set.

### SetModelIdNil

`func (o *AutoScout24Listing) SetModelIdNil(b bool)`

 SetModelIdNil sets the value for ModelId to be an explicit nil

### UnsetModelId
`func (o *AutoScout24Listing) UnsetModelId()`

UnsetModelId ensures that no value is present for ModelId, not even an explicit nil
### GetModelGroup

`func (o *AutoScout24Listing) GetModelGroup() string`

GetModelGroup returns the ModelGroup field if non-nil, zero value otherwise.

### GetModelGroupOk

`func (o *AutoScout24Listing) GetModelGroupOk() (*string, bool)`

GetModelGroupOk returns a tuple with the ModelGroup field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModelGroup

`func (o *AutoScout24Listing) SetModelGroup(v string)`

SetModelGroup sets ModelGroup field to given value.

### HasModelGroup

`func (o *AutoScout24Listing) HasModelGroup() bool`

HasModelGroup returns a boolean if a field has been set.

### SetModelGroupNil

`func (o *AutoScout24Listing) SetModelGroupNil(b bool)`

 SetModelGroupNil sets the value for ModelGroup to be an explicit nil

### UnsetModelGroup
`func (o *AutoScout24Listing) UnsetModelGroup()`

UnsetModelGroup ensures that no value is present for ModelGroup, not even an explicit nil
### GetVariant

`func (o *AutoScout24Listing) GetVariant() string`

GetVariant returns the Variant field if non-nil, zero value otherwise.

### GetVariantOk

`func (o *AutoScout24Listing) GetVariantOk() (*string, bool)`

GetVariantOk returns a tuple with the Variant field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVariant

`func (o *AutoScout24Listing) SetVariant(v string)`

SetVariant sets Variant field to given value.

### HasVariant

`func (o *AutoScout24Listing) HasVariant() bool`

HasVariant returns a boolean if a field has been set.

### SetVariantNil

`func (o *AutoScout24Listing) SetVariantNil(b bool)`

 SetVariantNil sets the value for Variant to be an explicit nil

### UnsetVariant
`func (o *AutoScout24Listing) UnsetVariant()`

UnsetVariant ensures that no value is present for Variant, not even an explicit nil
### GetMotorType

`func (o *AutoScout24Listing) GetMotorType() string`

GetMotorType returns the MotorType field if non-nil, zero value otherwise.

### GetMotorTypeOk

`func (o *AutoScout24Listing) GetMotorTypeOk() (*string, bool)`

GetMotorTypeOk returns a tuple with the MotorType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMotorType

`func (o *AutoScout24Listing) SetMotorType(v string)`

SetMotorType sets MotorType field to given value.

### HasMotorType

`func (o *AutoScout24Listing) HasMotorType() bool`

HasMotorType returns a boolean if a field has been set.

### SetMotorTypeNil

`func (o *AutoScout24Listing) SetMotorTypeNil(b bool)`

 SetMotorTypeNil sets the value for MotorType to be an explicit nil

### UnsetMotorType
`func (o *AutoScout24Listing) UnsetMotorType()`

UnsetMotorType ensures that no value is present for MotorType, not even an explicit nil
### GetVersion

`func (o *AutoScout24Listing) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *AutoScout24Listing) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *AutoScout24Listing) SetVersion(v string)`

SetVersion sets Version field to given value.

### HasVersion

`func (o *AutoScout24Listing) HasVersion() bool`

HasVersion returns a boolean if a field has been set.

### SetVersionNil

`func (o *AutoScout24Listing) SetVersionNil(b bool)`

 SetVersionNil sets the value for Version to be an explicit nil

### UnsetVersion
`func (o *AutoScout24Listing) UnsetVersion()`

UnsetVersion ensures that no value is present for Version, not even an explicit nil
### GetSubtitle

`func (o *AutoScout24Listing) GetSubtitle() string`

GetSubtitle returns the Subtitle field if non-nil, zero value otherwise.

### GetSubtitleOk

`func (o *AutoScout24Listing) GetSubtitleOk() (*string, bool)`

GetSubtitleOk returns a tuple with the Subtitle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubtitle

`func (o *AutoScout24Listing) SetSubtitle(v string)`

SetSubtitle sets Subtitle field to given value.

### HasSubtitle

`func (o *AutoScout24Listing) HasSubtitle() bool`

HasSubtitle returns a boolean if a field has been set.

### SetSubtitleNil

`func (o *AutoScout24Listing) SetSubtitleNil(b bool)`

 SetSubtitleNil sets the value for Subtitle to be an explicit nil

### UnsetSubtitle
`func (o *AutoScout24Listing) UnsetSubtitle()`

UnsetSubtitle ensures that no value is present for Subtitle, not even an explicit nil
### GetArticleType

`func (o *AutoScout24Listing) GetArticleType() string`

GetArticleType returns the ArticleType field if non-nil, zero value otherwise.

### GetArticleTypeOk

`func (o *AutoScout24Listing) GetArticleTypeOk() (*string, bool)`

GetArticleTypeOk returns a tuple with the ArticleType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArticleType

`func (o *AutoScout24Listing) SetArticleType(v string)`

SetArticleType sets ArticleType field to given value.

### HasArticleType

`func (o *AutoScout24Listing) HasArticleType() bool`

HasArticleType returns a boolean if a field has been set.

### SetArticleTypeNil

`func (o *AutoScout24Listing) SetArticleTypeNil(b bool)`

 SetArticleTypeNil sets the value for ArticleType to be an explicit nil

### UnsetArticleType
`func (o *AutoScout24Listing) UnsetArticleType()`

UnsetArticleType ensures that no value is present for ArticleType, not even an explicit nil
### GetOfferType

`func (o *AutoScout24Listing) GetOfferType() string`

GetOfferType returns the OfferType field if non-nil, zero value otherwise.

### GetOfferTypeOk

`func (o *AutoScout24Listing) GetOfferTypeOk() (*string, bool)`

GetOfferTypeOk returns a tuple with the OfferType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOfferType

`func (o *AutoScout24Listing) SetOfferType(v string)`

SetOfferType sets OfferType field to given value.

### HasOfferType

`func (o *AutoScout24Listing) HasOfferType() bool`

HasOfferType returns a boolean if a field has been set.

### SetOfferTypeNil

`func (o *AutoScout24Listing) SetOfferTypeNil(b bool)`

 SetOfferTypeNil sets the value for OfferType to be an explicit nil

### UnsetOfferType
`func (o *AutoScout24Listing) UnsetOfferType()`

UnsetOfferType ensures that no value is present for OfferType, not even an explicit nil
### GetFuel

`func (o *AutoScout24Listing) GetFuel() string`

GetFuel returns the Fuel field if non-nil, zero value otherwise.

### GetFuelOk

`func (o *AutoScout24Listing) GetFuelOk() (*string, bool)`

GetFuelOk returns a tuple with the Fuel field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFuel

`func (o *AutoScout24Listing) SetFuel(v string)`

SetFuel sets Fuel field to given value.

### HasFuel

`func (o *AutoScout24Listing) HasFuel() bool`

HasFuel returns a boolean if a field has been set.

### SetFuelNil

`func (o *AutoScout24Listing) SetFuelNil(b bool)`

 SetFuelNil sets the value for Fuel to be an explicit nil

### UnsetFuel
`func (o *AutoScout24Listing) UnsetFuel()`

UnsetFuel ensures that no value is present for Fuel, not even an explicit nil
### GetFuelType

`func (o *AutoScout24Listing) GetFuelType() string`

GetFuelType returns the FuelType field if non-nil, zero value otherwise.

### GetFuelTypeOk

`func (o *AutoScout24Listing) GetFuelTypeOk() (*string, bool)`

GetFuelTypeOk returns a tuple with the FuelType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFuelType

`func (o *AutoScout24Listing) SetFuelType(v string)`

SetFuelType sets FuelType field to given value.

### HasFuelType

`func (o *AutoScout24Listing) HasFuelType() bool`

HasFuelType returns a boolean if a field has been set.

### SetFuelTypeNil

`func (o *AutoScout24Listing) SetFuelTypeNil(b bool)`

 SetFuelTypeNil sets the value for FuelType to be an explicit nil

### UnsetFuelType
`func (o *AutoScout24Listing) UnsetFuelType()`

UnsetFuelType ensures that no value is present for FuelType, not even an explicit nil
### GetTransmission

`func (o *AutoScout24Listing) GetTransmission() string`

GetTransmission returns the Transmission field if non-nil, zero value otherwise.

### GetTransmissionOk

`func (o *AutoScout24Listing) GetTransmissionOk() (*string, bool)`

GetTransmissionOk returns a tuple with the Transmission field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransmission

`func (o *AutoScout24Listing) SetTransmission(v string)`

SetTransmission sets Transmission field to given value.

### HasTransmission

`func (o *AutoScout24Listing) HasTransmission() bool`

HasTransmission returns a boolean if a field has been set.

### SetTransmissionNil

`func (o *AutoScout24Listing) SetTransmissionNil(b bool)`

 SetTransmissionNil sets the value for Transmission to be an explicit nil

### UnsetTransmission
`func (o *AutoScout24Listing) UnsetTransmission()`

UnsetTransmission ensures that no value is present for Transmission, not even an explicit nil
### GetMileageKm

`func (o *AutoScout24Listing) GetMileageKm() int32`

GetMileageKm returns the MileageKm field if non-nil, zero value otherwise.

### GetMileageKmOk

`func (o *AutoScout24Listing) GetMileageKmOk() (*int32, bool)`

GetMileageKmOk returns a tuple with the MileageKm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMileageKm

`func (o *AutoScout24Listing) SetMileageKm(v int32)`

SetMileageKm sets MileageKm field to given value.

### HasMileageKm

`func (o *AutoScout24Listing) HasMileageKm() bool`

HasMileageKm returns a boolean if a field has been set.

### SetMileageKmNil

`func (o *AutoScout24Listing) SetMileageKmNil(b bool)`

 SetMileageKmNil sets the value for MileageKm to be an explicit nil

### UnsetMileageKm
`func (o *AutoScout24Listing) UnsetMileageKm()`

UnsetMileageKm ensures that no value is present for MileageKm, not even an explicit nil
### GetFirstRegistration

`func (o *AutoScout24Listing) GetFirstRegistration() string`

GetFirstRegistration returns the FirstRegistration field if non-nil, zero value otherwise.

### GetFirstRegistrationOk

`func (o *AutoScout24Listing) GetFirstRegistrationOk() (*string, bool)`

GetFirstRegistrationOk returns a tuple with the FirstRegistration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFirstRegistration

`func (o *AutoScout24Listing) SetFirstRegistration(v string)`

SetFirstRegistration sets FirstRegistration field to given value.

### HasFirstRegistration

`func (o *AutoScout24Listing) HasFirstRegistration() bool`

HasFirstRegistration returns a boolean if a field has been set.

### SetFirstRegistrationNil

`func (o *AutoScout24Listing) SetFirstRegistrationNil(b bool)`

 SetFirstRegistrationNil sets the value for FirstRegistration to be an explicit nil

### UnsetFirstRegistration
`func (o *AutoScout24Listing) UnsetFirstRegistration()`

UnsetFirstRegistration ensures that no value is present for FirstRegistration, not even an explicit nil
### GetRegistrationYear

`func (o *AutoScout24Listing) GetRegistrationYear() int32`

GetRegistrationYear returns the RegistrationYear field if non-nil, zero value otherwise.

### GetRegistrationYearOk

`func (o *AutoScout24Listing) GetRegistrationYearOk() (*int32, bool)`

GetRegistrationYearOk returns a tuple with the RegistrationYear field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegistrationYear

`func (o *AutoScout24Listing) SetRegistrationYear(v int32)`

SetRegistrationYear sets RegistrationYear field to given value.

### HasRegistrationYear

`func (o *AutoScout24Listing) HasRegistrationYear() bool`

HasRegistrationYear returns a boolean if a field has been set.

### SetRegistrationYearNil

`func (o *AutoScout24Listing) SetRegistrationYearNil(b bool)`

 SetRegistrationYearNil sets the value for RegistrationYear to be an explicit nil

### UnsetRegistrationYear
`func (o *AutoScout24Listing) UnsetRegistrationYear()`

UnsetRegistrationYear ensures that no value is present for RegistrationYear, not even an explicit nil
### GetRegistrationMonth

`func (o *AutoScout24Listing) GetRegistrationMonth() int32`

GetRegistrationMonth returns the RegistrationMonth field if non-nil, zero value otherwise.

### GetRegistrationMonthOk

`func (o *AutoScout24Listing) GetRegistrationMonthOk() (*int32, bool)`

GetRegistrationMonthOk returns a tuple with the RegistrationMonth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegistrationMonth

`func (o *AutoScout24Listing) SetRegistrationMonth(v int32)`

SetRegistrationMonth sets RegistrationMonth field to given value.

### HasRegistrationMonth

`func (o *AutoScout24Listing) HasRegistrationMonth() bool`

HasRegistrationMonth returns a boolean if a field has been set.

### SetRegistrationMonthNil

`func (o *AutoScout24Listing) SetRegistrationMonthNil(b bool)`

 SetRegistrationMonthNil sets the value for RegistrationMonth to be an explicit nil

### UnsetRegistrationMonth
`func (o *AutoScout24Listing) UnsetRegistrationMonth()`

UnsetRegistrationMonth ensures that no value is present for RegistrationMonth, not even an explicit nil
### GetPowerKw

`func (o *AutoScout24Listing) GetPowerKw() float32`

GetPowerKw returns the PowerKw field if non-nil, zero value otherwise.

### GetPowerKwOk

`func (o *AutoScout24Listing) GetPowerKwOk() (*float32, bool)`

GetPowerKwOk returns a tuple with the PowerKw field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPowerKw

`func (o *AutoScout24Listing) SetPowerKw(v float32)`

SetPowerKw sets PowerKw field to given value.

### HasPowerKw

`func (o *AutoScout24Listing) HasPowerKw() bool`

HasPowerKw returns a boolean if a field has been set.

### SetPowerKwNil

`func (o *AutoScout24Listing) SetPowerKwNil(b bool)`

 SetPowerKwNil sets the value for PowerKw to be an explicit nil

### UnsetPowerKw
`func (o *AutoScout24Listing) UnsetPowerKw()`

UnsetPowerKw ensures that no value is present for PowerKw, not even an explicit nil
### GetPowerHp

`func (o *AutoScout24Listing) GetPowerHp() float32`

GetPowerHp returns the PowerHp field if non-nil, zero value otherwise.

### GetPowerHpOk

`func (o *AutoScout24Listing) GetPowerHpOk() (*float32, bool)`

GetPowerHpOk returns a tuple with the PowerHp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPowerHp

`func (o *AutoScout24Listing) SetPowerHp(v float32)`

SetPowerHp sets PowerHp field to given value.

### HasPowerHp

`func (o *AutoScout24Listing) HasPowerHp() bool`

HasPowerHp returns a boolean if a field has been set.

### SetPowerHpNil

`func (o *AutoScout24Listing) SetPowerHpNil(b bool)`

 SetPowerHpNil sets the value for PowerHp to be an explicit nil

### UnsetPowerHp
`func (o *AutoScout24Listing) UnsetPowerHp()`

UnsetPowerHp ensures that no value is present for PowerHp, not even an explicit nil
### GetDisplacementCc

`func (o *AutoScout24Listing) GetDisplacementCc() int32`

GetDisplacementCc returns the DisplacementCc field if non-nil, zero value otherwise.

### GetDisplacementCcOk

`func (o *AutoScout24Listing) GetDisplacementCcOk() (*int32, bool)`

GetDisplacementCcOk returns a tuple with the DisplacementCc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplacementCc

`func (o *AutoScout24Listing) SetDisplacementCc(v int32)`

SetDisplacementCc sets DisplacementCc field to given value.

### HasDisplacementCc

`func (o *AutoScout24Listing) HasDisplacementCc() bool`

HasDisplacementCc returns a boolean if a field has been set.

### SetDisplacementCcNil

`func (o *AutoScout24Listing) SetDisplacementCcNil(b bool)`

 SetDisplacementCcNil sets the value for DisplacementCc to be an explicit nil

### UnsetDisplacementCc
`func (o *AutoScout24Listing) UnsetDisplacementCc()`

UnsetDisplacementCc ensures that no value is present for DisplacementCc, not even an explicit nil
### GetIsDamaged

`func (o *AutoScout24Listing) GetIsDamaged() bool`

GetIsDamaged returns the IsDamaged field if non-nil, zero value otherwise.

### GetIsDamagedOk

`func (o *AutoScout24Listing) GetIsDamagedOk() (*bool, bool)`

GetIsDamagedOk returns a tuple with the IsDamaged field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDamaged

`func (o *AutoScout24Listing) SetIsDamaged(v bool)`

SetIsDamaged sets IsDamaged field to given value.

### HasIsDamaged

`func (o *AutoScout24Listing) HasIsDamaged() bool`

HasIsDamaged returns a boolean if a field has been set.

### SetIsDamagedNil

`func (o *AutoScout24Listing) SetIsDamagedNil(b bool)`

 SetIsDamagedNil sets the value for IsDamaged to be an explicit nil

### UnsetIsDamaged
`func (o *AutoScout24Listing) UnsetIsDamaged()`

UnsetIsDamaged ensures that no value is present for IsDamaged, not even an explicit nil
### GetAvailableNow

`func (o *AutoScout24Listing) GetAvailableNow() bool`

GetAvailableNow returns the AvailableNow field if non-nil, zero value otherwise.

### GetAvailableNowOk

`func (o *AutoScout24Listing) GetAvailableNowOk() (*bool, bool)`

GetAvailableNowOk returns a tuple with the AvailableNow field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAvailableNow

`func (o *AutoScout24Listing) SetAvailableNow(v bool)`

SetAvailableNow sets AvailableNow field to given value.

### HasAvailableNow

`func (o *AutoScout24Listing) HasAvailableNow() bool`

HasAvailableNow returns a boolean if a field has been set.

### SetAvailableNowNil

`func (o *AutoScout24Listing) SetAvailableNowNil(b bool)`

 SetAvailableNowNil sets the value for AvailableNow to be an explicit nil

### UnsetAvailableNow
`func (o *AutoScout24Listing) UnsetAvailableNow()`

UnsetAvailableNow ensures that no value is present for AvailableNow, not even an explicit nil
### GetAvailableAt

`func (o *AutoScout24Listing) GetAvailableAt() string`

GetAvailableAt returns the AvailableAt field if non-nil, zero value otherwise.

### GetAvailableAtOk

`func (o *AutoScout24Listing) GetAvailableAtOk() (*string, bool)`

GetAvailableAtOk returns a tuple with the AvailableAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAvailableAt

`func (o *AutoScout24Listing) SetAvailableAt(v string)`

SetAvailableAt sets AvailableAt field to given value.

### HasAvailableAt

`func (o *AutoScout24Listing) HasAvailableAt() bool`

HasAvailableAt returns a boolean if a field has been set.

### SetAvailableAtNil

`func (o *AutoScout24Listing) SetAvailableAtNil(b bool)`

 SetAvailableAtNil sets the value for AvailableAt to be an explicit nil

### UnsetAvailableAt
`func (o *AutoScout24Listing) UnsetAvailableAt()`

UnsetAvailableAt ensures that no value is present for AvailableAt, not even an explicit nil
### GetAvailableUtc

`func (o *AutoScout24Listing) GetAvailableUtc() float32`

GetAvailableUtc returns the AvailableUtc field if non-nil, zero value otherwise.

### GetAvailableUtcOk

`func (o *AutoScout24Listing) GetAvailableUtcOk() (*float32, bool)`

GetAvailableUtcOk returns a tuple with the AvailableUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAvailableUtc

`func (o *AutoScout24Listing) SetAvailableUtc(v float32)`

SetAvailableUtc sets AvailableUtc field to given value.

### HasAvailableUtc

`func (o *AutoScout24Listing) HasAvailableUtc() bool`

HasAvailableUtc returns a boolean if a field has been set.

### SetAvailableUtcNil

`func (o *AutoScout24Listing) SetAvailableUtcNil(b bool)`

 SetAvailableUtcNil sets the value for AvailableUtc to be an explicit nil

### UnsetAvailableUtc
`func (o *AutoScout24Listing) UnsetAvailableUtc()`

UnsetAvailableUtc ensures that no value is present for AvailableUtc, not even an explicit nil
### GetAvailabilityInDays

`func (o *AutoScout24Listing) GetAvailabilityInDays() int32`

GetAvailabilityInDays returns the AvailabilityInDays field if non-nil, zero value otherwise.

### GetAvailabilityInDaysOk

`func (o *AutoScout24Listing) GetAvailabilityInDaysOk() (*int32, bool)`

GetAvailabilityInDaysOk returns a tuple with the AvailabilityInDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAvailabilityInDays

`func (o *AutoScout24Listing) SetAvailabilityInDays(v int32)`

SetAvailabilityInDays sets AvailabilityInDays field to given value.

### HasAvailabilityInDays

`func (o *AutoScout24Listing) HasAvailabilityInDays() bool`

HasAvailabilityInDays returns a boolean if a field has been set.

### SetAvailabilityInDaysNil

`func (o *AutoScout24Listing) SetAvailabilityInDaysNil(b bool)`

 SetAvailabilityInDaysNil sets the value for AvailabilityInDays to be an explicit nil

### UnsetAvailabilityInDays
`func (o *AutoScout24Listing) UnsetAvailabilityInDays()`

UnsetAvailabilityInDays ensures that no value is present for AvailabilityInDays, not even an explicit nil
### GetLocation

`func (o *AutoScout24Listing) GetLocation() map[string]interface{}`

GetLocation returns the Location field if non-nil, zero value otherwise.

### GetLocationOk

`func (o *AutoScout24Listing) GetLocationOk() (*map[string]interface{}, bool)`

GetLocationOk returns a tuple with the Location field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocation

`func (o *AutoScout24Listing) SetLocation(v map[string]interface{})`

SetLocation sets Location field to given value.

### HasLocation

`func (o *AutoScout24Listing) HasLocation() bool`

HasLocation returns a boolean if a field has been set.

### GetSeller

`func (o *AutoScout24Listing) GetSeller() map[string]interface{}`

GetSeller returns the Seller field if non-nil, zero value otherwise.

### GetSellerOk

`func (o *AutoScout24Listing) GetSellerOk() (*map[string]interface{}, bool)`

GetSellerOk returns a tuple with the Seller field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeller

`func (o *AutoScout24Listing) SetSeller(v map[string]interface{})`

SetSeller sets Seller field to given value.

### HasSeller

`func (o *AutoScout24Listing) HasSeller() bool`

HasSeller returns a boolean if a field has been set.

### GetRating

`func (o *AutoScout24Listing) GetRating() float32`

GetRating returns the Rating field if non-nil, zero value otherwise.

### GetRatingOk

`func (o *AutoScout24Listing) GetRatingOk() (*float32, bool)`

GetRatingOk returns a tuple with the Rating field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRating

`func (o *AutoScout24Listing) SetRating(v float32)`

SetRating sets Rating field to given value.

### HasRating

`func (o *AutoScout24Listing) HasRating() bool`

HasRating returns a boolean if a field has been set.

### SetRatingNil

`func (o *AutoScout24Listing) SetRatingNil(b bool)`

 SetRatingNil sets the value for Rating to be an explicit nil

### UnsetRating
`func (o *AutoScout24Listing) UnsetRating()`

UnsetRating ensures that no value is present for Rating, not even an explicit nil
### GetRatingCount

`func (o *AutoScout24Listing) GetRatingCount() int32`

GetRatingCount returns the RatingCount field if non-nil, zero value otherwise.

### GetRatingCountOk

`func (o *AutoScout24Listing) GetRatingCountOk() (*int32, bool)`

GetRatingCountOk returns a tuple with the RatingCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRatingCount

`func (o *AutoScout24Listing) SetRatingCount(v int32)`

SetRatingCount sets RatingCount field to given value.

### HasRatingCount

`func (o *AutoScout24Listing) HasRatingCount() bool`

HasRatingCount returns a boolean if a field has been set.

### SetRatingCountNil

`func (o *AutoScout24Listing) SetRatingCountNil(b bool)`

 SetRatingCountNil sets the value for RatingCount to be an explicit nil

### UnsetRatingCount
`func (o *AutoScout24Listing) UnsetRatingCount()`

UnsetRatingCount ensures that no value is present for RatingCount, not even an explicit nil
### GetRatingsEnabled

`func (o *AutoScout24Listing) GetRatingsEnabled() bool`

GetRatingsEnabled returns the RatingsEnabled field if non-nil, zero value otherwise.

### GetRatingsEnabledOk

`func (o *AutoScout24Listing) GetRatingsEnabledOk() (*bool, bool)`

GetRatingsEnabledOk returns a tuple with the RatingsEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRatingsEnabled

`func (o *AutoScout24Listing) SetRatingsEnabled(v bool)`

SetRatingsEnabled sets RatingsEnabled field to given value.

### HasRatingsEnabled

`func (o *AutoScout24Listing) HasRatingsEnabled() bool`

HasRatingsEnabled returns a boolean if a field has been set.

### SetRatingsEnabledNil

`func (o *AutoScout24Listing) SetRatingsEnabledNil(b bool)`

 SetRatingsEnabledNil sets the value for RatingsEnabled to be an explicit nil

### UnsetRatingsEnabled
`func (o *AutoScout24Listing) UnsetRatingsEnabled()`

UnsetRatingsEnabled ensures that no value is present for RatingsEnabled, not even an explicit nil
### GetLeasing

`func (o *AutoScout24Listing) GetLeasing() map[string]interface{}`

GetLeasing returns the Leasing field if non-nil, zero value otherwise.

### GetLeasingOk

`func (o *AutoScout24Listing) GetLeasingOk() (*map[string]interface{}, bool)`

GetLeasingOk returns a tuple with the Leasing field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLeasing

`func (o *AutoScout24Listing) SetLeasing(v map[string]interface{})`

SetLeasing sets Leasing field to given value.

### HasLeasing

`func (o *AutoScout24Listing) HasLeasing() bool`

HasLeasing returns a boolean if a field has been set.

### SetLeasingNil

`func (o *AutoScout24Listing) SetLeasingNil(b bool)`

 SetLeasingNil sets the value for Leasing to be an explicit nil

### UnsetLeasing
`func (o *AutoScout24Listing) UnsetLeasing()`

UnsetLeasing ensures that no value is present for Leasing, not even an explicit nil
### GetSeals

`func (o *AutoScout24Listing) GetSeals() []*map[string]interface{}`

GetSeals returns the Seals field if non-nil, zero value otherwise.

### GetSealsOk

`func (o *AutoScout24Listing) GetSealsOk() (*[]*map[string]interface{}, bool)`

GetSealsOk returns a tuple with the Seals field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeals

`func (o *AutoScout24Listing) SetSeals(v []*map[string]interface{})`

SetSeals sets Seals field to given value.

### HasSeals

`func (o *AutoScout24Listing) HasSeals() bool`

HasSeals returns a boolean if a field has been set.

### GetOnlinePurchase

`func (o *AutoScout24Listing) GetOnlinePurchase() map[string]interface{}`

GetOnlinePurchase returns the OnlinePurchase field if non-nil, zero value otherwise.

### GetOnlinePurchaseOk

`func (o *AutoScout24Listing) GetOnlinePurchaseOk() (*map[string]interface{}, bool)`

GetOnlinePurchaseOk returns a tuple with the OnlinePurchase field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOnlinePurchase

`func (o *AutoScout24Listing) SetOnlinePurchase(v map[string]interface{})`

SetOnlinePurchase sets OnlinePurchase field to given value.

### HasOnlinePurchase

`func (o *AutoScout24Listing) HasOnlinePurchase() bool`

HasOnlinePurchase returns a boolean if a field has been set.

### SetOnlinePurchaseNil

`func (o *AutoScout24Listing) SetOnlinePurchaseNil(b bool)`

 SetOnlinePurchaseNil sets the value for OnlinePurchase to be an explicit nil

### UnsetOnlinePurchase
`func (o *AutoScout24Listing) UnsetOnlinePurchase()`

UnsetOnlinePurchase ensures that no value is present for OnlinePurchase, not even an explicit nil
### GetElectricVehicleBanner

`func (o *AutoScout24Listing) GetElectricVehicleBanner() map[string]interface{}`

GetElectricVehicleBanner returns the ElectricVehicleBanner field if non-nil, zero value otherwise.

### GetElectricVehicleBannerOk

`func (o *AutoScout24Listing) GetElectricVehicleBannerOk() (*map[string]interface{}, bool)`

GetElectricVehicleBannerOk returns a tuple with the ElectricVehicleBanner field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetElectricVehicleBanner

`func (o *AutoScout24Listing) SetElectricVehicleBanner(v map[string]interface{})`

SetElectricVehicleBanner sets ElectricVehicleBanner field to given value.

### HasElectricVehicleBanner

`func (o *AutoScout24Listing) HasElectricVehicleBanner() bool`

HasElectricVehicleBanner returns a boolean if a field has been set.

### SetElectricVehicleBannerNil

`func (o *AutoScout24Listing) SetElectricVehicleBannerNil(b bool)`

 SetElectricVehicleBannerNil sets the value for ElectricVehicleBanner to be an explicit nil

### UnsetElectricVehicleBanner
`func (o *AutoScout24Listing) UnsetElectricVehicleBanner()`

UnsetElectricVehicleBanner ensures that no value is present for ElectricVehicleBanner, not even an explicit nil
### GetIsDeliverable

`func (o *AutoScout24Listing) GetIsDeliverable() bool`

GetIsDeliverable returns the IsDeliverable field if non-nil, zero value otherwise.

### GetIsDeliverableOk

`func (o *AutoScout24Listing) GetIsDeliverableOk() (*bool, bool)`

GetIsDeliverableOk returns a tuple with the IsDeliverable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDeliverable

`func (o *AutoScout24Listing) SetIsDeliverable(v bool)`

SetIsDeliverable sets IsDeliverable field to given value.

### HasIsDeliverable

`func (o *AutoScout24Listing) HasIsDeliverable() bool`

HasIsDeliverable returns a boolean if a field has been set.

### SetIsDeliverableNil

`func (o *AutoScout24Listing) SetIsDeliverableNil(b bool)`

 SetIsDeliverableNil sets the value for IsDeliverable to be an explicit nil

### UnsetIsDeliverable
`func (o *AutoScout24Listing) UnsetIsDeliverable()`

UnsetIsDeliverable ensures that no value is present for IsDeliverable, not even an explicit nil
### GetHasVideo

`func (o *AutoScout24Listing) GetHasVideo() bool`

GetHasVideo returns the HasVideo field if non-nil, zero value otherwise.

### GetHasVideoOk

`func (o *AutoScout24Listing) GetHasVideoOk() (*bool, bool)`

GetHasVideoOk returns a tuple with the HasVideo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasVideo

`func (o *AutoScout24Listing) SetHasVideo(v bool)`

SetHasVideo sets HasVideo field to given value.

### HasHasVideo

`func (o *AutoScout24Listing) HasHasVideo() bool`

HasHasVideo returns a boolean if a field has been set.

### SetHasVideoNil

`func (o *AutoScout24Listing) SetHasVideoNil(b bool)`

 SetHasVideoNil sets the value for HasVideo to be an explicit nil

### UnsetHasVideo
`func (o *AutoScout24Listing) UnsetHasVideo()`

UnsetHasVideo ensures that no value is present for HasVideo, not even an explicit nil
### GetHas360Image

`func (o *AutoScout24Listing) GetHas360Image() bool`

GetHas360Image returns the Has360Image field if non-nil, zero value otherwise.

### GetHas360ImageOk

`func (o *AutoScout24Listing) GetHas360ImageOk() (*bool, bool)`

GetHas360ImageOk returns a tuple with the Has360Image field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHas360Image

`func (o *AutoScout24Listing) SetHas360Image(v bool)`

SetHas360Image sets Has360Image field to given value.

### HasHas360Image

`func (o *AutoScout24Listing) HasHas360Image() bool`

HasHas360Image returns a boolean if a field has been set.

### SetHas360ImageNil

`func (o *AutoScout24Listing) SetHas360ImageNil(b bool)`

 SetHas360ImageNil sets the value for Has360Image to be an explicit nil

### UnsetHas360Image
`func (o *AutoScout24Listing) UnsetHas360Image()`

UnsetHas360Image ensures that no value is present for Has360Image, not even an explicit nil
### GetInterestLevel

`func (o *AutoScout24Listing) GetInterestLevel() string`

GetInterestLevel returns the InterestLevel field if non-nil, zero value otherwise.

### GetInterestLevelOk

`func (o *AutoScout24Listing) GetInterestLevelOk() (*string, bool)`

GetInterestLevelOk returns a tuple with the InterestLevel field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInterestLevel

`func (o *AutoScout24Listing) SetInterestLevel(v string)`

SetInterestLevel sets InterestLevel field to given value.

### HasInterestLevel

`func (o *AutoScout24Listing) HasInterestLevel() bool`

HasInterestLevel returns a boolean if a field has been set.

### SetInterestLevelNil

`func (o *AutoScout24Listing) SetInterestLevelNil(b bool)`

 SetInterestLevelNil sets the value for InterestLevel to be an explicit nil

### UnsetInterestLevel
`func (o *AutoScout24Listing) UnsetInterestLevel()`

UnsetInterestLevel ensures that no value is present for InterestLevel, not even an explicit nil
### GetIsTrending

`func (o *AutoScout24Listing) GetIsTrending() bool`

GetIsTrending returns the IsTrending field if non-nil, zero value otherwise.

### GetIsTrendingOk

`func (o *AutoScout24Listing) GetIsTrendingOk() (*bool, bool)`

GetIsTrendingOk returns a tuple with the IsTrending field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsTrending

`func (o *AutoScout24Listing) SetIsTrending(v bool)`

SetIsTrending sets IsTrending field to given value.

### HasIsTrending

`func (o *AutoScout24Listing) HasIsTrending() bool`

HasIsTrending returns a boolean if a field has been set.

### SetIsTrendingNil

`func (o *AutoScout24Listing) SetIsTrendingNil(b bool)`

 SetIsTrendingNil sets the value for IsTrending to be an explicit nil

### UnsetIsTrending
`func (o *AutoScout24Listing) UnsetIsTrending()`

UnsetIsTrending ensures that no value is present for IsTrending, not even an explicit nil
### GetAdTier

`func (o *AutoScout24Listing) GetAdTier() string`

GetAdTier returns the AdTier field if non-nil, zero value otherwise.

### GetAdTierOk

`func (o *AutoScout24Listing) GetAdTierOk() (*string, bool)`

GetAdTierOk returns a tuple with the AdTier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdTier

`func (o *AutoScout24Listing) SetAdTier(v string)`

SetAdTier sets AdTier field to given value.

### HasAdTier

`func (o *AutoScout24Listing) HasAdTier() bool`

HasAdTier returns a boolean if a field has been set.

### SetAdTierNil

`func (o *AutoScout24Listing) SetAdTierNil(b bool)`

 SetAdTierNil sets the value for AdTier to be an explicit nil

### UnsetAdTier
`func (o *AutoScout24Listing) UnsetAdTier()`

UnsetAdTier ensures that no value is present for AdTier, not even an explicit nil
### GetResultType

`func (o *AutoScout24Listing) GetResultType() string`

GetResultType returns the ResultType field if non-nil, zero value otherwise.

### GetResultTypeOk

`func (o *AutoScout24Listing) GetResultTypeOk() (*string, bool)`

GetResultTypeOk returns a tuple with the ResultType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResultType

`func (o *AutoScout24Listing) SetResultType(v string)`

SetResultType sets ResultType field to given value.

### HasResultType

`func (o *AutoScout24Listing) HasResultType() bool`

HasResultType returns a boolean if a field has been set.

### SetResultTypeNil

`func (o *AutoScout24Listing) SetResultTypeNil(b bool)`

 SetResultTypeNil sets the value for ResultType to be an explicit nil

### UnsetResultType
`func (o *AutoScout24Listing) UnsetResultType()`

UnsetResultType ensures that no value is present for ResultType, not even an explicit nil
### GetResultSection

`func (o *AutoScout24Listing) GetResultSection() string`

GetResultSection returns the ResultSection field if non-nil, zero value otherwise.

### GetResultSectionOk

`func (o *AutoScout24Listing) GetResultSectionOk() (*string, bool)`

GetResultSectionOk returns a tuple with the ResultSection field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResultSection

`func (o *AutoScout24Listing) SetResultSection(v string)`

SetResultSection sets ResultSection field to given value.

### HasResultSection

`func (o *AutoScout24Listing) HasResultSection() bool`

HasResultSection returns a boolean if a field has been set.

### SetResultSectionNil

`func (o *AutoScout24Listing) SetResultSectionNil(b bool)`

 SetResultSectionNil sets the value for ResultSection to be an explicit nil

### UnsetResultSection
`func (o *AutoScout24Listing) UnsetResultSection()`

UnsetResultSection ensures that no value is present for ResultSection, not even an explicit nil
### GetSpecialConditions

`func (o *AutoScout24Listing) GetSpecialConditions() []interface{}`

GetSpecialConditions returns the SpecialConditions field if non-nil, zero value otherwise.

### GetSpecialConditionsOk

`func (o *AutoScout24Listing) GetSpecialConditionsOk() (*[]interface{}, bool)`

GetSpecialConditionsOk returns a tuple with the SpecialConditions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSpecialConditions

`func (o *AutoScout24Listing) SetSpecialConditions(v []interface{})`

SetSpecialConditions sets SpecialConditions field to given value.

### HasSpecialConditions

`func (o *AutoScout24Listing) HasSpecialConditions() bool`

HasSpecialConditions returns a boolean if a field has been set.

### GetVehicleDetails

`func (o *AutoScout24Listing) GetVehicleDetails() []*map[string]interface{}`

GetVehicleDetails returns the VehicleDetails field if non-nil, zero value otherwise.

### GetVehicleDetailsOk

`func (o *AutoScout24Listing) GetVehicleDetailsOk() (*[]*map[string]interface{}, bool)`

GetVehicleDetailsOk returns a tuple with the VehicleDetails field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVehicleDetails

`func (o *AutoScout24Listing) SetVehicleDetails(v []*map[string]interface{})`

SetVehicleDetails sets VehicleDetails field to given value.

### HasVehicleDetails

`func (o *AutoScout24Listing) HasVehicleDetails() bool`

HasVehicleDetails returns a boolean if a field has been set.

### GetWltpValues

`func (o *AutoScout24Listing) GetWltpValues() []string`

GetWltpValues returns the WltpValues field if non-nil, zero value otherwise.

### GetWltpValuesOk

`func (o *AutoScout24Listing) GetWltpValuesOk() (*[]string, bool)`

GetWltpValuesOk returns a tuple with the WltpValues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWltpValues

`func (o *AutoScout24Listing) SetWltpValues(v []string)`

SetWltpValues sets WltpValues field to given value.

### HasWltpValues

`func (o *AutoScout24Listing) HasWltpValues() bool`

HasWltpValues returns a boolean if a field has been set.

### GetVehicle

`func (o *AutoScout24Listing) GetVehicle() map[string]interface{}`

GetVehicle returns the Vehicle field if non-nil, zero value otherwise.

### GetVehicleOk

`func (o *AutoScout24Listing) GetVehicleOk() (*map[string]interface{}, bool)`

GetVehicleOk returns a tuple with the Vehicle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVehicle

`func (o *AutoScout24Listing) SetVehicle(v map[string]interface{})`

SetVehicle sets Vehicle field to given value.

### HasVehicle

`func (o *AutoScout24Listing) HasVehicle() bool`

HasVehicle returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



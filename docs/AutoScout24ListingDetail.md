# AutoScout24ListingDetail

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Title** | **string** |  | 
**Url** | **string** |  | 
**Description** | Pointer to **NullableString** |  | [optional] 
**DescriptionHtml** | Pointer to **NullableString** |  | [optional] 
**Status** | Pointer to **NullableString** |  | [optional] 
**Currency** | Pointer to **string** |  | [optional] [default to "EUR"]
**Price** | Pointer to **NullableFloat32** |  | [optional] 
**PriceFormatted** | Pointer to **NullableString** |  | [optional] 
**NetPrice** | Pointer to **NullableFloat32** |  | [optional] 
**VatRate** | Pointer to **NullableFloat32** |  | [optional] 
**IsVatDeductible** | Pointer to **NullableBool** |  | [optional] 
**IsNegotiable** | Pointer to **NullableBool** |  | [optional] 
**IsPriceOnRequest** | Pointer to **NullableBool** |  | [optional] 
**IsFinalPrice** | Pointer to **NullableBool** |  | [optional] 
**MedianPrice** | Pointer to **NullableFloat32** |  | [optional] 
**PriceEvaluation** | Pointer to **NullableInt32** |  | [optional] 
**PriceDetails** | Pointer to **map[string]interface{}** |  | [optional] 
**Prices** | Pointer to **map[string]interface{}** |  | [optional] 
**SuperDeal** | Pointer to **map[string]interface{}** |  | [optional] 
**Make** | Pointer to **NullableString** |  | [optional] 
**Model** | Pointer to **NullableString** |  | [optional] 
**Variant** | Pointer to **NullableString** |  | [optional] 
**Version** | Pointer to **NullableString** |  | [optional] 
**MileageKm** | Pointer to **NullableInt32** |  | [optional] 
**FirstRegistration** | Pointer to **NullableString** |  | [optional] 
**RegistrationYear** | Pointer to **NullableInt32** |  | [optional] 
**RegistrationMonth** | Pointer to **NullableInt32** |  | [optional] 
**PowerKw** | Pointer to **NullableFloat32** |  | [optional] 
**PowerHp** | Pointer to **NullableFloat32** |  | [optional] 
**DisplacementCc** | Pointer to **NullableInt32** |  | [optional] 
**Transmission** | Pointer to **NullableString** |  | [optional] 
**BodyType** | Pointer to **NullableString** |  | [optional] 
**Fuel** | Pointer to **NullableString** |  | [optional] 
**FuelType** | Pointer to **NullableString** |  | [optional] 
**Seats** | Pointer to **NullableInt32** |  | [optional] 
**Doors** | Pointer to **NullableInt32** |  | [optional] 
**Vehicle** | Pointer to **map[string]interface{}** | Complete useful native specifications, including rawData, energy and history. | [optional] 
**Equipment** | Pointer to **map[string][]interface{}** |  | [optional] 
**Images** | Pointer to **[]string** |  | [optional] 
**HeaderImage** | Pointer to **NullableString** |  | [optional] 
**ImageAltText** | Pointer to **NullableString** |  | [optional] 
**IsCoverImagePlaceholder** | Pointer to **NullableBool** |  | [optional] 
**CoverImageAttractiveness** | Pointer to **NullableFloat32** |  | [optional] 
**YoutubeLink** | Pointer to **NullableString** |  | [optional] 
**TwinnerUrl** | Pointer to **NullableString** |  | [optional] 
**Has360View** | Pointer to **NullableBool** |  | [optional] 
**ThreeSixty** | Pointer to **interface{}** |  | [optional] 
**VehicleReport** | Pointer to **interface{}** |  | [optional] 
**PartnerIntegrations** | Pointer to **[]map[string]interface{}** |  | [optional] 
**Seller** | Pointer to **map[string]interface{}** |  | [optional] 
**Location** | Pointer to **map[string]interface{}** |  | [optional] 
**Ratings** | Pointer to **map[string]interface{}** |  | [optional] 
**Rating** | Pointer to **NullableFloat32** |  | [optional] 
**RatingCount** | Pointer to **NullableInt32** |  | [optional] 
**RecommendPercentage** | Pointer to **NullableFloat32** |  | [optional] 
**WhatsappNumber** | Pointer to **NullableString** |  | [optional] 
**Identifier** | Pointer to **map[string]interface{}** |  | [optional] 
**ArticleType** | Pointer to **NullableString** |  | [optional] 
**VehicleType** | Pointer to **NullableString** |  | [optional] 
**IsNew** | Pointer to **NullableBool** |  | [optional] 
**IsDeliverable** | Pointer to **NullableBool** |  | [optional] 
**Availability** | Pointer to **map[string]interface{}** |  | [optional] 
**AvailableAt** | Pointer to **NullableString** |  | [optional] 
**AvailableUtc** | Pointer to **NullableFloat32** |  | [optional] 
**CreatedAt** | Pointer to **NullableString** |  | [optional] 
**CreatedUtc** | Pointer to **NullableFloat32** |  | [optional] 
**LeasingDetails** | Pointer to **interface{}** |  | [optional] 
**Warranty** | Pointer to **interface{}** |  | [optional] 
**HasWarranty** | Pointer to **NullableBool** |  | [optional] 
**FinancingFlags** | Pointer to **interface{}** |  | [optional] 
**FinancingAndInsurance** | Pointer to **interface{}** |  | [optional] 
**OnlinePurchase** | Pointer to **interface{}** |  | [optional] 
**Seals** | Pointer to **[]interface{}** |  | [optional] 
**SpecialConditions** | Pointer to **[]interface{}** |  | [optional] 
**SearchResultType** | Pointer to **NullableString** |  | [optional] 
**AdTier** | Pointer to **NullableString** |  | [optional] 
**AppliedAdTier** | Pointer to **NullableString** |  | [optional] 
**HasPremiumListingTreatment** | Pointer to **NullableBool** |  | [optional] 
**IsTrending** | Pointer to **NullableBool** |  | [optional] 
**IsListingBoost** | Pointer to **NullableBool** |  | [optional] 
**Statistics** | Pointer to **map[string]interface{}** |  | [optional] 
**InteractionStatistics** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewAutoScout24ListingDetail

`func NewAutoScout24ListingDetail(id string, title string, url string, ) *AutoScout24ListingDetail`

NewAutoScout24ListingDetail instantiates a new AutoScout24ListingDetail object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAutoScout24ListingDetailWithDefaults

`func NewAutoScout24ListingDetailWithDefaults() *AutoScout24ListingDetail`

NewAutoScout24ListingDetailWithDefaults instantiates a new AutoScout24ListingDetail object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *AutoScout24ListingDetail) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *AutoScout24ListingDetail) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *AutoScout24ListingDetail) SetId(v string)`

SetId sets Id field to given value.


### GetTitle

`func (o *AutoScout24ListingDetail) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *AutoScout24ListingDetail) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *AutoScout24ListingDetail) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetUrl

`func (o *AutoScout24ListingDetail) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *AutoScout24ListingDetail) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *AutoScout24ListingDetail) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetDescription

`func (o *AutoScout24ListingDetail) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *AutoScout24ListingDetail) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *AutoScout24ListingDetail) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *AutoScout24ListingDetail) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *AutoScout24ListingDetail) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *AutoScout24ListingDetail) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetDescriptionHtml

`func (o *AutoScout24ListingDetail) GetDescriptionHtml() string`

GetDescriptionHtml returns the DescriptionHtml field if non-nil, zero value otherwise.

### GetDescriptionHtmlOk

`func (o *AutoScout24ListingDetail) GetDescriptionHtmlOk() (*string, bool)`

GetDescriptionHtmlOk returns a tuple with the DescriptionHtml field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescriptionHtml

`func (o *AutoScout24ListingDetail) SetDescriptionHtml(v string)`

SetDescriptionHtml sets DescriptionHtml field to given value.

### HasDescriptionHtml

`func (o *AutoScout24ListingDetail) HasDescriptionHtml() bool`

HasDescriptionHtml returns a boolean if a field has been set.

### SetDescriptionHtmlNil

`func (o *AutoScout24ListingDetail) SetDescriptionHtmlNil(b bool)`

 SetDescriptionHtmlNil sets the value for DescriptionHtml to be an explicit nil

### UnsetDescriptionHtml
`func (o *AutoScout24ListingDetail) UnsetDescriptionHtml()`

UnsetDescriptionHtml ensures that no value is present for DescriptionHtml, not even an explicit nil
### GetStatus

`func (o *AutoScout24ListingDetail) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *AutoScout24ListingDetail) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *AutoScout24ListingDetail) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *AutoScout24ListingDetail) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### SetStatusNil

`func (o *AutoScout24ListingDetail) SetStatusNil(b bool)`

 SetStatusNil sets the value for Status to be an explicit nil

### UnsetStatus
`func (o *AutoScout24ListingDetail) UnsetStatus()`

UnsetStatus ensures that no value is present for Status, not even an explicit nil
### GetCurrency

`func (o *AutoScout24ListingDetail) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *AutoScout24ListingDetail) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *AutoScout24ListingDetail) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *AutoScout24ListingDetail) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetPrice

`func (o *AutoScout24ListingDetail) GetPrice() float32`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *AutoScout24ListingDetail) GetPriceOk() (*float32, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *AutoScout24ListingDetail) SetPrice(v float32)`

SetPrice sets Price field to given value.

### HasPrice

`func (o *AutoScout24ListingDetail) HasPrice() bool`

HasPrice returns a boolean if a field has been set.

### SetPriceNil

`func (o *AutoScout24ListingDetail) SetPriceNil(b bool)`

 SetPriceNil sets the value for Price to be an explicit nil

### UnsetPrice
`func (o *AutoScout24ListingDetail) UnsetPrice()`

UnsetPrice ensures that no value is present for Price, not even an explicit nil
### GetPriceFormatted

`func (o *AutoScout24ListingDetail) GetPriceFormatted() string`

GetPriceFormatted returns the PriceFormatted field if non-nil, zero value otherwise.

### GetPriceFormattedOk

`func (o *AutoScout24ListingDetail) GetPriceFormattedOk() (*string, bool)`

GetPriceFormattedOk returns a tuple with the PriceFormatted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceFormatted

`func (o *AutoScout24ListingDetail) SetPriceFormatted(v string)`

SetPriceFormatted sets PriceFormatted field to given value.

### HasPriceFormatted

`func (o *AutoScout24ListingDetail) HasPriceFormatted() bool`

HasPriceFormatted returns a boolean if a field has been set.

### SetPriceFormattedNil

`func (o *AutoScout24ListingDetail) SetPriceFormattedNil(b bool)`

 SetPriceFormattedNil sets the value for PriceFormatted to be an explicit nil

### UnsetPriceFormatted
`func (o *AutoScout24ListingDetail) UnsetPriceFormatted()`

UnsetPriceFormatted ensures that no value is present for PriceFormatted, not even an explicit nil
### GetNetPrice

`func (o *AutoScout24ListingDetail) GetNetPrice() float32`

GetNetPrice returns the NetPrice field if non-nil, zero value otherwise.

### GetNetPriceOk

`func (o *AutoScout24ListingDetail) GetNetPriceOk() (*float32, bool)`

GetNetPriceOk returns a tuple with the NetPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNetPrice

`func (o *AutoScout24ListingDetail) SetNetPrice(v float32)`

SetNetPrice sets NetPrice field to given value.

### HasNetPrice

`func (o *AutoScout24ListingDetail) HasNetPrice() bool`

HasNetPrice returns a boolean if a field has been set.

### SetNetPriceNil

`func (o *AutoScout24ListingDetail) SetNetPriceNil(b bool)`

 SetNetPriceNil sets the value for NetPrice to be an explicit nil

### UnsetNetPrice
`func (o *AutoScout24ListingDetail) UnsetNetPrice()`

UnsetNetPrice ensures that no value is present for NetPrice, not even an explicit nil
### GetVatRate

`func (o *AutoScout24ListingDetail) GetVatRate() float32`

GetVatRate returns the VatRate field if non-nil, zero value otherwise.

### GetVatRateOk

`func (o *AutoScout24ListingDetail) GetVatRateOk() (*float32, bool)`

GetVatRateOk returns a tuple with the VatRate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVatRate

`func (o *AutoScout24ListingDetail) SetVatRate(v float32)`

SetVatRate sets VatRate field to given value.

### HasVatRate

`func (o *AutoScout24ListingDetail) HasVatRate() bool`

HasVatRate returns a boolean if a field has been set.

### SetVatRateNil

`func (o *AutoScout24ListingDetail) SetVatRateNil(b bool)`

 SetVatRateNil sets the value for VatRate to be an explicit nil

### UnsetVatRate
`func (o *AutoScout24ListingDetail) UnsetVatRate()`

UnsetVatRate ensures that no value is present for VatRate, not even an explicit nil
### GetIsVatDeductible

`func (o *AutoScout24ListingDetail) GetIsVatDeductible() bool`

GetIsVatDeductible returns the IsVatDeductible field if non-nil, zero value otherwise.

### GetIsVatDeductibleOk

`func (o *AutoScout24ListingDetail) GetIsVatDeductibleOk() (*bool, bool)`

GetIsVatDeductibleOk returns a tuple with the IsVatDeductible field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsVatDeductible

`func (o *AutoScout24ListingDetail) SetIsVatDeductible(v bool)`

SetIsVatDeductible sets IsVatDeductible field to given value.

### HasIsVatDeductible

`func (o *AutoScout24ListingDetail) HasIsVatDeductible() bool`

HasIsVatDeductible returns a boolean if a field has been set.

### SetIsVatDeductibleNil

`func (o *AutoScout24ListingDetail) SetIsVatDeductibleNil(b bool)`

 SetIsVatDeductibleNil sets the value for IsVatDeductible to be an explicit nil

### UnsetIsVatDeductible
`func (o *AutoScout24ListingDetail) UnsetIsVatDeductible()`

UnsetIsVatDeductible ensures that no value is present for IsVatDeductible, not even an explicit nil
### GetIsNegotiable

`func (o *AutoScout24ListingDetail) GetIsNegotiable() bool`

GetIsNegotiable returns the IsNegotiable field if non-nil, zero value otherwise.

### GetIsNegotiableOk

`func (o *AutoScout24ListingDetail) GetIsNegotiableOk() (*bool, bool)`

GetIsNegotiableOk returns a tuple with the IsNegotiable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsNegotiable

`func (o *AutoScout24ListingDetail) SetIsNegotiable(v bool)`

SetIsNegotiable sets IsNegotiable field to given value.

### HasIsNegotiable

`func (o *AutoScout24ListingDetail) HasIsNegotiable() bool`

HasIsNegotiable returns a boolean if a field has been set.

### SetIsNegotiableNil

`func (o *AutoScout24ListingDetail) SetIsNegotiableNil(b bool)`

 SetIsNegotiableNil sets the value for IsNegotiable to be an explicit nil

### UnsetIsNegotiable
`func (o *AutoScout24ListingDetail) UnsetIsNegotiable()`

UnsetIsNegotiable ensures that no value is present for IsNegotiable, not even an explicit nil
### GetIsPriceOnRequest

`func (o *AutoScout24ListingDetail) GetIsPriceOnRequest() bool`

GetIsPriceOnRequest returns the IsPriceOnRequest field if non-nil, zero value otherwise.

### GetIsPriceOnRequestOk

`func (o *AutoScout24ListingDetail) GetIsPriceOnRequestOk() (*bool, bool)`

GetIsPriceOnRequestOk returns a tuple with the IsPriceOnRequest field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsPriceOnRequest

`func (o *AutoScout24ListingDetail) SetIsPriceOnRequest(v bool)`

SetIsPriceOnRequest sets IsPriceOnRequest field to given value.

### HasIsPriceOnRequest

`func (o *AutoScout24ListingDetail) HasIsPriceOnRequest() bool`

HasIsPriceOnRequest returns a boolean if a field has been set.

### SetIsPriceOnRequestNil

`func (o *AutoScout24ListingDetail) SetIsPriceOnRequestNil(b bool)`

 SetIsPriceOnRequestNil sets the value for IsPriceOnRequest to be an explicit nil

### UnsetIsPriceOnRequest
`func (o *AutoScout24ListingDetail) UnsetIsPriceOnRequest()`

UnsetIsPriceOnRequest ensures that no value is present for IsPriceOnRequest, not even an explicit nil
### GetIsFinalPrice

`func (o *AutoScout24ListingDetail) GetIsFinalPrice() bool`

GetIsFinalPrice returns the IsFinalPrice field if non-nil, zero value otherwise.

### GetIsFinalPriceOk

`func (o *AutoScout24ListingDetail) GetIsFinalPriceOk() (*bool, bool)`

GetIsFinalPriceOk returns a tuple with the IsFinalPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsFinalPrice

`func (o *AutoScout24ListingDetail) SetIsFinalPrice(v bool)`

SetIsFinalPrice sets IsFinalPrice field to given value.

### HasIsFinalPrice

`func (o *AutoScout24ListingDetail) HasIsFinalPrice() bool`

HasIsFinalPrice returns a boolean if a field has been set.

### SetIsFinalPriceNil

`func (o *AutoScout24ListingDetail) SetIsFinalPriceNil(b bool)`

 SetIsFinalPriceNil sets the value for IsFinalPrice to be an explicit nil

### UnsetIsFinalPrice
`func (o *AutoScout24ListingDetail) UnsetIsFinalPrice()`

UnsetIsFinalPrice ensures that no value is present for IsFinalPrice, not even an explicit nil
### GetMedianPrice

`func (o *AutoScout24ListingDetail) GetMedianPrice() float32`

GetMedianPrice returns the MedianPrice field if non-nil, zero value otherwise.

### GetMedianPriceOk

`func (o *AutoScout24ListingDetail) GetMedianPriceOk() (*float32, bool)`

GetMedianPriceOk returns a tuple with the MedianPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMedianPrice

`func (o *AutoScout24ListingDetail) SetMedianPrice(v float32)`

SetMedianPrice sets MedianPrice field to given value.

### HasMedianPrice

`func (o *AutoScout24ListingDetail) HasMedianPrice() bool`

HasMedianPrice returns a boolean if a field has been set.

### SetMedianPriceNil

`func (o *AutoScout24ListingDetail) SetMedianPriceNil(b bool)`

 SetMedianPriceNil sets the value for MedianPrice to be an explicit nil

### UnsetMedianPrice
`func (o *AutoScout24ListingDetail) UnsetMedianPrice()`

UnsetMedianPrice ensures that no value is present for MedianPrice, not even an explicit nil
### GetPriceEvaluation

`func (o *AutoScout24ListingDetail) GetPriceEvaluation() int32`

GetPriceEvaluation returns the PriceEvaluation field if non-nil, zero value otherwise.

### GetPriceEvaluationOk

`func (o *AutoScout24ListingDetail) GetPriceEvaluationOk() (*int32, bool)`

GetPriceEvaluationOk returns a tuple with the PriceEvaluation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceEvaluation

`func (o *AutoScout24ListingDetail) SetPriceEvaluation(v int32)`

SetPriceEvaluation sets PriceEvaluation field to given value.

### HasPriceEvaluation

`func (o *AutoScout24ListingDetail) HasPriceEvaluation() bool`

HasPriceEvaluation returns a boolean if a field has been set.

### SetPriceEvaluationNil

`func (o *AutoScout24ListingDetail) SetPriceEvaluationNil(b bool)`

 SetPriceEvaluationNil sets the value for PriceEvaluation to be an explicit nil

### UnsetPriceEvaluation
`func (o *AutoScout24ListingDetail) UnsetPriceEvaluation()`

UnsetPriceEvaluation ensures that no value is present for PriceEvaluation, not even an explicit nil
### GetPriceDetails

`func (o *AutoScout24ListingDetail) GetPriceDetails() map[string]interface{}`

GetPriceDetails returns the PriceDetails field if non-nil, zero value otherwise.

### GetPriceDetailsOk

`func (o *AutoScout24ListingDetail) GetPriceDetailsOk() (*map[string]interface{}, bool)`

GetPriceDetailsOk returns a tuple with the PriceDetails field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceDetails

`func (o *AutoScout24ListingDetail) SetPriceDetails(v map[string]interface{})`

SetPriceDetails sets PriceDetails field to given value.

### HasPriceDetails

`func (o *AutoScout24ListingDetail) HasPriceDetails() bool`

HasPriceDetails returns a boolean if a field has been set.

### GetPrices

`func (o *AutoScout24ListingDetail) GetPrices() map[string]interface{}`

GetPrices returns the Prices field if non-nil, zero value otherwise.

### GetPricesOk

`func (o *AutoScout24ListingDetail) GetPricesOk() (*map[string]interface{}, bool)`

GetPricesOk returns a tuple with the Prices field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrices

`func (o *AutoScout24ListingDetail) SetPrices(v map[string]interface{})`

SetPrices sets Prices field to given value.

### HasPrices

`func (o *AutoScout24ListingDetail) HasPrices() bool`

HasPrices returns a boolean if a field has been set.

### GetSuperDeal

`func (o *AutoScout24ListingDetail) GetSuperDeal() map[string]interface{}`

GetSuperDeal returns the SuperDeal field if non-nil, zero value otherwise.

### GetSuperDealOk

`func (o *AutoScout24ListingDetail) GetSuperDealOk() (*map[string]interface{}, bool)`

GetSuperDealOk returns a tuple with the SuperDeal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuperDeal

`func (o *AutoScout24ListingDetail) SetSuperDeal(v map[string]interface{})`

SetSuperDeal sets SuperDeal field to given value.

### HasSuperDeal

`func (o *AutoScout24ListingDetail) HasSuperDeal() bool`

HasSuperDeal returns a boolean if a field has been set.

### GetMake

`func (o *AutoScout24ListingDetail) GetMake() string`

GetMake returns the Make field if non-nil, zero value otherwise.

### GetMakeOk

`func (o *AutoScout24ListingDetail) GetMakeOk() (*string, bool)`

GetMakeOk returns a tuple with the Make field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMake

`func (o *AutoScout24ListingDetail) SetMake(v string)`

SetMake sets Make field to given value.

### HasMake

`func (o *AutoScout24ListingDetail) HasMake() bool`

HasMake returns a boolean if a field has been set.

### SetMakeNil

`func (o *AutoScout24ListingDetail) SetMakeNil(b bool)`

 SetMakeNil sets the value for Make to be an explicit nil

### UnsetMake
`func (o *AutoScout24ListingDetail) UnsetMake()`

UnsetMake ensures that no value is present for Make, not even an explicit nil
### GetModel

`func (o *AutoScout24ListingDetail) GetModel() string`

GetModel returns the Model field if non-nil, zero value otherwise.

### GetModelOk

`func (o *AutoScout24ListingDetail) GetModelOk() (*string, bool)`

GetModelOk returns a tuple with the Model field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModel

`func (o *AutoScout24ListingDetail) SetModel(v string)`

SetModel sets Model field to given value.

### HasModel

`func (o *AutoScout24ListingDetail) HasModel() bool`

HasModel returns a boolean if a field has been set.

### SetModelNil

`func (o *AutoScout24ListingDetail) SetModelNil(b bool)`

 SetModelNil sets the value for Model to be an explicit nil

### UnsetModel
`func (o *AutoScout24ListingDetail) UnsetModel()`

UnsetModel ensures that no value is present for Model, not even an explicit nil
### GetVariant

`func (o *AutoScout24ListingDetail) GetVariant() string`

GetVariant returns the Variant field if non-nil, zero value otherwise.

### GetVariantOk

`func (o *AutoScout24ListingDetail) GetVariantOk() (*string, bool)`

GetVariantOk returns a tuple with the Variant field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVariant

`func (o *AutoScout24ListingDetail) SetVariant(v string)`

SetVariant sets Variant field to given value.

### HasVariant

`func (o *AutoScout24ListingDetail) HasVariant() bool`

HasVariant returns a boolean if a field has been set.

### SetVariantNil

`func (o *AutoScout24ListingDetail) SetVariantNil(b bool)`

 SetVariantNil sets the value for Variant to be an explicit nil

### UnsetVariant
`func (o *AutoScout24ListingDetail) UnsetVariant()`

UnsetVariant ensures that no value is present for Variant, not even an explicit nil
### GetVersion

`func (o *AutoScout24ListingDetail) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *AutoScout24ListingDetail) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *AutoScout24ListingDetail) SetVersion(v string)`

SetVersion sets Version field to given value.

### HasVersion

`func (o *AutoScout24ListingDetail) HasVersion() bool`

HasVersion returns a boolean if a field has been set.

### SetVersionNil

`func (o *AutoScout24ListingDetail) SetVersionNil(b bool)`

 SetVersionNil sets the value for Version to be an explicit nil

### UnsetVersion
`func (o *AutoScout24ListingDetail) UnsetVersion()`

UnsetVersion ensures that no value is present for Version, not even an explicit nil
### GetMileageKm

`func (o *AutoScout24ListingDetail) GetMileageKm() int32`

GetMileageKm returns the MileageKm field if non-nil, zero value otherwise.

### GetMileageKmOk

`func (o *AutoScout24ListingDetail) GetMileageKmOk() (*int32, bool)`

GetMileageKmOk returns a tuple with the MileageKm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMileageKm

`func (o *AutoScout24ListingDetail) SetMileageKm(v int32)`

SetMileageKm sets MileageKm field to given value.

### HasMileageKm

`func (o *AutoScout24ListingDetail) HasMileageKm() bool`

HasMileageKm returns a boolean if a field has been set.

### SetMileageKmNil

`func (o *AutoScout24ListingDetail) SetMileageKmNil(b bool)`

 SetMileageKmNil sets the value for MileageKm to be an explicit nil

### UnsetMileageKm
`func (o *AutoScout24ListingDetail) UnsetMileageKm()`

UnsetMileageKm ensures that no value is present for MileageKm, not even an explicit nil
### GetFirstRegistration

`func (o *AutoScout24ListingDetail) GetFirstRegistration() string`

GetFirstRegistration returns the FirstRegistration field if non-nil, zero value otherwise.

### GetFirstRegistrationOk

`func (o *AutoScout24ListingDetail) GetFirstRegistrationOk() (*string, bool)`

GetFirstRegistrationOk returns a tuple with the FirstRegistration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFirstRegistration

`func (o *AutoScout24ListingDetail) SetFirstRegistration(v string)`

SetFirstRegistration sets FirstRegistration field to given value.

### HasFirstRegistration

`func (o *AutoScout24ListingDetail) HasFirstRegistration() bool`

HasFirstRegistration returns a boolean if a field has been set.

### SetFirstRegistrationNil

`func (o *AutoScout24ListingDetail) SetFirstRegistrationNil(b bool)`

 SetFirstRegistrationNil sets the value for FirstRegistration to be an explicit nil

### UnsetFirstRegistration
`func (o *AutoScout24ListingDetail) UnsetFirstRegistration()`

UnsetFirstRegistration ensures that no value is present for FirstRegistration, not even an explicit nil
### GetRegistrationYear

`func (o *AutoScout24ListingDetail) GetRegistrationYear() int32`

GetRegistrationYear returns the RegistrationYear field if non-nil, zero value otherwise.

### GetRegistrationYearOk

`func (o *AutoScout24ListingDetail) GetRegistrationYearOk() (*int32, bool)`

GetRegistrationYearOk returns a tuple with the RegistrationYear field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegistrationYear

`func (o *AutoScout24ListingDetail) SetRegistrationYear(v int32)`

SetRegistrationYear sets RegistrationYear field to given value.

### HasRegistrationYear

`func (o *AutoScout24ListingDetail) HasRegistrationYear() bool`

HasRegistrationYear returns a boolean if a field has been set.

### SetRegistrationYearNil

`func (o *AutoScout24ListingDetail) SetRegistrationYearNil(b bool)`

 SetRegistrationYearNil sets the value for RegistrationYear to be an explicit nil

### UnsetRegistrationYear
`func (o *AutoScout24ListingDetail) UnsetRegistrationYear()`

UnsetRegistrationYear ensures that no value is present for RegistrationYear, not even an explicit nil
### GetRegistrationMonth

`func (o *AutoScout24ListingDetail) GetRegistrationMonth() int32`

GetRegistrationMonth returns the RegistrationMonth field if non-nil, zero value otherwise.

### GetRegistrationMonthOk

`func (o *AutoScout24ListingDetail) GetRegistrationMonthOk() (*int32, bool)`

GetRegistrationMonthOk returns a tuple with the RegistrationMonth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegistrationMonth

`func (o *AutoScout24ListingDetail) SetRegistrationMonth(v int32)`

SetRegistrationMonth sets RegistrationMonth field to given value.

### HasRegistrationMonth

`func (o *AutoScout24ListingDetail) HasRegistrationMonth() bool`

HasRegistrationMonth returns a boolean if a field has been set.

### SetRegistrationMonthNil

`func (o *AutoScout24ListingDetail) SetRegistrationMonthNil(b bool)`

 SetRegistrationMonthNil sets the value for RegistrationMonth to be an explicit nil

### UnsetRegistrationMonth
`func (o *AutoScout24ListingDetail) UnsetRegistrationMonth()`

UnsetRegistrationMonth ensures that no value is present for RegistrationMonth, not even an explicit nil
### GetPowerKw

`func (o *AutoScout24ListingDetail) GetPowerKw() float32`

GetPowerKw returns the PowerKw field if non-nil, zero value otherwise.

### GetPowerKwOk

`func (o *AutoScout24ListingDetail) GetPowerKwOk() (*float32, bool)`

GetPowerKwOk returns a tuple with the PowerKw field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPowerKw

`func (o *AutoScout24ListingDetail) SetPowerKw(v float32)`

SetPowerKw sets PowerKw field to given value.

### HasPowerKw

`func (o *AutoScout24ListingDetail) HasPowerKw() bool`

HasPowerKw returns a boolean if a field has been set.

### SetPowerKwNil

`func (o *AutoScout24ListingDetail) SetPowerKwNil(b bool)`

 SetPowerKwNil sets the value for PowerKw to be an explicit nil

### UnsetPowerKw
`func (o *AutoScout24ListingDetail) UnsetPowerKw()`

UnsetPowerKw ensures that no value is present for PowerKw, not even an explicit nil
### GetPowerHp

`func (o *AutoScout24ListingDetail) GetPowerHp() float32`

GetPowerHp returns the PowerHp field if non-nil, zero value otherwise.

### GetPowerHpOk

`func (o *AutoScout24ListingDetail) GetPowerHpOk() (*float32, bool)`

GetPowerHpOk returns a tuple with the PowerHp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPowerHp

`func (o *AutoScout24ListingDetail) SetPowerHp(v float32)`

SetPowerHp sets PowerHp field to given value.

### HasPowerHp

`func (o *AutoScout24ListingDetail) HasPowerHp() bool`

HasPowerHp returns a boolean if a field has been set.

### SetPowerHpNil

`func (o *AutoScout24ListingDetail) SetPowerHpNil(b bool)`

 SetPowerHpNil sets the value for PowerHp to be an explicit nil

### UnsetPowerHp
`func (o *AutoScout24ListingDetail) UnsetPowerHp()`

UnsetPowerHp ensures that no value is present for PowerHp, not even an explicit nil
### GetDisplacementCc

`func (o *AutoScout24ListingDetail) GetDisplacementCc() int32`

GetDisplacementCc returns the DisplacementCc field if non-nil, zero value otherwise.

### GetDisplacementCcOk

`func (o *AutoScout24ListingDetail) GetDisplacementCcOk() (*int32, bool)`

GetDisplacementCcOk returns a tuple with the DisplacementCc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplacementCc

`func (o *AutoScout24ListingDetail) SetDisplacementCc(v int32)`

SetDisplacementCc sets DisplacementCc field to given value.

### HasDisplacementCc

`func (o *AutoScout24ListingDetail) HasDisplacementCc() bool`

HasDisplacementCc returns a boolean if a field has been set.

### SetDisplacementCcNil

`func (o *AutoScout24ListingDetail) SetDisplacementCcNil(b bool)`

 SetDisplacementCcNil sets the value for DisplacementCc to be an explicit nil

### UnsetDisplacementCc
`func (o *AutoScout24ListingDetail) UnsetDisplacementCc()`

UnsetDisplacementCc ensures that no value is present for DisplacementCc, not even an explicit nil
### GetTransmission

`func (o *AutoScout24ListingDetail) GetTransmission() string`

GetTransmission returns the Transmission field if non-nil, zero value otherwise.

### GetTransmissionOk

`func (o *AutoScout24ListingDetail) GetTransmissionOk() (*string, bool)`

GetTransmissionOk returns a tuple with the Transmission field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransmission

`func (o *AutoScout24ListingDetail) SetTransmission(v string)`

SetTransmission sets Transmission field to given value.

### HasTransmission

`func (o *AutoScout24ListingDetail) HasTransmission() bool`

HasTransmission returns a boolean if a field has been set.

### SetTransmissionNil

`func (o *AutoScout24ListingDetail) SetTransmissionNil(b bool)`

 SetTransmissionNil sets the value for Transmission to be an explicit nil

### UnsetTransmission
`func (o *AutoScout24ListingDetail) UnsetTransmission()`

UnsetTransmission ensures that no value is present for Transmission, not even an explicit nil
### GetBodyType

`func (o *AutoScout24ListingDetail) GetBodyType() string`

GetBodyType returns the BodyType field if non-nil, zero value otherwise.

### GetBodyTypeOk

`func (o *AutoScout24ListingDetail) GetBodyTypeOk() (*string, bool)`

GetBodyTypeOk returns a tuple with the BodyType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBodyType

`func (o *AutoScout24ListingDetail) SetBodyType(v string)`

SetBodyType sets BodyType field to given value.

### HasBodyType

`func (o *AutoScout24ListingDetail) HasBodyType() bool`

HasBodyType returns a boolean if a field has been set.

### SetBodyTypeNil

`func (o *AutoScout24ListingDetail) SetBodyTypeNil(b bool)`

 SetBodyTypeNil sets the value for BodyType to be an explicit nil

### UnsetBodyType
`func (o *AutoScout24ListingDetail) UnsetBodyType()`

UnsetBodyType ensures that no value is present for BodyType, not even an explicit nil
### GetFuel

`func (o *AutoScout24ListingDetail) GetFuel() string`

GetFuel returns the Fuel field if non-nil, zero value otherwise.

### GetFuelOk

`func (o *AutoScout24ListingDetail) GetFuelOk() (*string, bool)`

GetFuelOk returns a tuple with the Fuel field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFuel

`func (o *AutoScout24ListingDetail) SetFuel(v string)`

SetFuel sets Fuel field to given value.

### HasFuel

`func (o *AutoScout24ListingDetail) HasFuel() bool`

HasFuel returns a boolean if a field has been set.

### SetFuelNil

`func (o *AutoScout24ListingDetail) SetFuelNil(b bool)`

 SetFuelNil sets the value for Fuel to be an explicit nil

### UnsetFuel
`func (o *AutoScout24ListingDetail) UnsetFuel()`

UnsetFuel ensures that no value is present for Fuel, not even an explicit nil
### GetFuelType

`func (o *AutoScout24ListingDetail) GetFuelType() string`

GetFuelType returns the FuelType field if non-nil, zero value otherwise.

### GetFuelTypeOk

`func (o *AutoScout24ListingDetail) GetFuelTypeOk() (*string, bool)`

GetFuelTypeOk returns a tuple with the FuelType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFuelType

`func (o *AutoScout24ListingDetail) SetFuelType(v string)`

SetFuelType sets FuelType field to given value.

### HasFuelType

`func (o *AutoScout24ListingDetail) HasFuelType() bool`

HasFuelType returns a boolean if a field has been set.

### SetFuelTypeNil

`func (o *AutoScout24ListingDetail) SetFuelTypeNil(b bool)`

 SetFuelTypeNil sets the value for FuelType to be an explicit nil

### UnsetFuelType
`func (o *AutoScout24ListingDetail) UnsetFuelType()`

UnsetFuelType ensures that no value is present for FuelType, not even an explicit nil
### GetSeats

`func (o *AutoScout24ListingDetail) GetSeats() int32`

GetSeats returns the Seats field if non-nil, zero value otherwise.

### GetSeatsOk

`func (o *AutoScout24ListingDetail) GetSeatsOk() (*int32, bool)`

GetSeatsOk returns a tuple with the Seats field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeats

`func (o *AutoScout24ListingDetail) SetSeats(v int32)`

SetSeats sets Seats field to given value.

### HasSeats

`func (o *AutoScout24ListingDetail) HasSeats() bool`

HasSeats returns a boolean if a field has been set.

### SetSeatsNil

`func (o *AutoScout24ListingDetail) SetSeatsNil(b bool)`

 SetSeatsNil sets the value for Seats to be an explicit nil

### UnsetSeats
`func (o *AutoScout24ListingDetail) UnsetSeats()`

UnsetSeats ensures that no value is present for Seats, not even an explicit nil
### GetDoors

`func (o *AutoScout24ListingDetail) GetDoors() int32`

GetDoors returns the Doors field if non-nil, zero value otherwise.

### GetDoorsOk

`func (o *AutoScout24ListingDetail) GetDoorsOk() (*int32, bool)`

GetDoorsOk returns a tuple with the Doors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDoors

`func (o *AutoScout24ListingDetail) SetDoors(v int32)`

SetDoors sets Doors field to given value.

### HasDoors

`func (o *AutoScout24ListingDetail) HasDoors() bool`

HasDoors returns a boolean if a field has been set.

### SetDoorsNil

`func (o *AutoScout24ListingDetail) SetDoorsNil(b bool)`

 SetDoorsNil sets the value for Doors to be an explicit nil

### UnsetDoors
`func (o *AutoScout24ListingDetail) UnsetDoors()`

UnsetDoors ensures that no value is present for Doors, not even an explicit nil
### GetVehicle

`func (o *AutoScout24ListingDetail) GetVehicle() map[string]interface{}`

GetVehicle returns the Vehicle field if non-nil, zero value otherwise.

### GetVehicleOk

`func (o *AutoScout24ListingDetail) GetVehicleOk() (*map[string]interface{}, bool)`

GetVehicleOk returns a tuple with the Vehicle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVehicle

`func (o *AutoScout24ListingDetail) SetVehicle(v map[string]interface{})`

SetVehicle sets Vehicle field to given value.

### HasVehicle

`func (o *AutoScout24ListingDetail) HasVehicle() bool`

HasVehicle returns a boolean if a field has been set.

### GetEquipment

`func (o *AutoScout24ListingDetail) GetEquipment() map[string][]interface{}`

GetEquipment returns the Equipment field if non-nil, zero value otherwise.

### GetEquipmentOk

`func (o *AutoScout24ListingDetail) GetEquipmentOk() (*map[string][]interface{}, bool)`

GetEquipmentOk returns a tuple with the Equipment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEquipment

`func (o *AutoScout24ListingDetail) SetEquipment(v map[string][]interface{})`

SetEquipment sets Equipment field to given value.

### HasEquipment

`func (o *AutoScout24ListingDetail) HasEquipment() bool`

HasEquipment returns a boolean if a field has been set.

### GetImages

`func (o *AutoScout24ListingDetail) GetImages() []string`

GetImages returns the Images field if non-nil, zero value otherwise.

### GetImagesOk

`func (o *AutoScout24ListingDetail) GetImagesOk() (*[]string, bool)`

GetImagesOk returns a tuple with the Images field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImages

`func (o *AutoScout24ListingDetail) SetImages(v []string)`

SetImages sets Images field to given value.

### HasImages

`func (o *AutoScout24ListingDetail) HasImages() bool`

HasImages returns a boolean if a field has been set.

### GetHeaderImage

`func (o *AutoScout24ListingDetail) GetHeaderImage() string`

GetHeaderImage returns the HeaderImage field if non-nil, zero value otherwise.

### GetHeaderImageOk

`func (o *AutoScout24ListingDetail) GetHeaderImageOk() (*string, bool)`

GetHeaderImageOk returns a tuple with the HeaderImage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeaderImage

`func (o *AutoScout24ListingDetail) SetHeaderImage(v string)`

SetHeaderImage sets HeaderImage field to given value.

### HasHeaderImage

`func (o *AutoScout24ListingDetail) HasHeaderImage() bool`

HasHeaderImage returns a boolean if a field has been set.

### SetHeaderImageNil

`func (o *AutoScout24ListingDetail) SetHeaderImageNil(b bool)`

 SetHeaderImageNil sets the value for HeaderImage to be an explicit nil

### UnsetHeaderImage
`func (o *AutoScout24ListingDetail) UnsetHeaderImage()`

UnsetHeaderImage ensures that no value is present for HeaderImage, not even an explicit nil
### GetImageAltText

`func (o *AutoScout24ListingDetail) GetImageAltText() string`

GetImageAltText returns the ImageAltText field if non-nil, zero value otherwise.

### GetImageAltTextOk

`func (o *AutoScout24ListingDetail) GetImageAltTextOk() (*string, bool)`

GetImageAltTextOk returns a tuple with the ImageAltText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImageAltText

`func (o *AutoScout24ListingDetail) SetImageAltText(v string)`

SetImageAltText sets ImageAltText field to given value.

### HasImageAltText

`func (o *AutoScout24ListingDetail) HasImageAltText() bool`

HasImageAltText returns a boolean if a field has been set.

### SetImageAltTextNil

`func (o *AutoScout24ListingDetail) SetImageAltTextNil(b bool)`

 SetImageAltTextNil sets the value for ImageAltText to be an explicit nil

### UnsetImageAltText
`func (o *AutoScout24ListingDetail) UnsetImageAltText()`

UnsetImageAltText ensures that no value is present for ImageAltText, not even an explicit nil
### GetIsCoverImagePlaceholder

`func (o *AutoScout24ListingDetail) GetIsCoverImagePlaceholder() bool`

GetIsCoverImagePlaceholder returns the IsCoverImagePlaceholder field if non-nil, zero value otherwise.

### GetIsCoverImagePlaceholderOk

`func (o *AutoScout24ListingDetail) GetIsCoverImagePlaceholderOk() (*bool, bool)`

GetIsCoverImagePlaceholderOk returns a tuple with the IsCoverImagePlaceholder field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsCoverImagePlaceholder

`func (o *AutoScout24ListingDetail) SetIsCoverImagePlaceholder(v bool)`

SetIsCoverImagePlaceholder sets IsCoverImagePlaceholder field to given value.

### HasIsCoverImagePlaceholder

`func (o *AutoScout24ListingDetail) HasIsCoverImagePlaceholder() bool`

HasIsCoverImagePlaceholder returns a boolean if a field has been set.

### SetIsCoverImagePlaceholderNil

`func (o *AutoScout24ListingDetail) SetIsCoverImagePlaceholderNil(b bool)`

 SetIsCoverImagePlaceholderNil sets the value for IsCoverImagePlaceholder to be an explicit nil

### UnsetIsCoverImagePlaceholder
`func (o *AutoScout24ListingDetail) UnsetIsCoverImagePlaceholder()`

UnsetIsCoverImagePlaceholder ensures that no value is present for IsCoverImagePlaceholder, not even an explicit nil
### GetCoverImageAttractiveness

`func (o *AutoScout24ListingDetail) GetCoverImageAttractiveness() float32`

GetCoverImageAttractiveness returns the CoverImageAttractiveness field if non-nil, zero value otherwise.

### GetCoverImageAttractivenessOk

`func (o *AutoScout24ListingDetail) GetCoverImageAttractivenessOk() (*float32, bool)`

GetCoverImageAttractivenessOk returns a tuple with the CoverImageAttractiveness field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCoverImageAttractiveness

`func (o *AutoScout24ListingDetail) SetCoverImageAttractiveness(v float32)`

SetCoverImageAttractiveness sets CoverImageAttractiveness field to given value.

### HasCoverImageAttractiveness

`func (o *AutoScout24ListingDetail) HasCoverImageAttractiveness() bool`

HasCoverImageAttractiveness returns a boolean if a field has been set.

### SetCoverImageAttractivenessNil

`func (o *AutoScout24ListingDetail) SetCoverImageAttractivenessNil(b bool)`

 SetCoverImageAttractivenessNil sets the value for CoverImageAttractiveness to be an explicit nil

### UnsetCoverImageAttractiveness
`func (o *AutoScout24ListingDetail) UnsetCoverImageAttractiveness()`

UnsetCoverImageAttractiveness ensures that no value is present for CoverImageAttractiveness, not even an explicit nil
### GetYoutubeLink

`func (o *AutoScout24ListingDetail) GetYoutubeLink() string`

GetYoutubeLink returns the YoutubeLink field if non-nil, zero value otherwise.

### GetYoutubeLinkOk

`func (o *AutoScout24ListingDetail) GetYoutubeLinkOk() (*string, bool)`

GetYoutubeLinkOk returns a tuple with the YoutubeLink field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetYoutubeLink

`func (o *AutoScout24ListingDetail) SetYoutubeLink(v string)`

SetYoutubeLink sets YoutubeLink field to given value.

### HasYoutubeLink

`func (o *AutoScout24ListingDetail) HasYoutubeLink() bool`

HasYoutubeLink returns a boolean if a field has been set.

### SetYoutubeLinkNil

`func (o *AutoScout24ListingDetail) SetYoutubeLinkNil(b bool)`

 SetYoutubeLinkNil sets the value for YoutubeLink to be an explicit nil

### UnsetYoutubeLink
`func (o *AutoScout24ListingDetail) UnsetYoutubeLink()`

UnsetYoutubeLink ensures that no value is present for YoutubeLink, not even an explicit nil
### GetTwinnerUrl

`func (o *AutoScout24ListingDetail) GetTwinnerUrl() string`

GetTwinnerUrl returns the TwinnerUrl field if non-nil, zero value otherwise.

### GetTwinnerUrlOk

`func (o *AutoScout24ListingDetail) GetTwinnerUrlOk() (*string, bool)`

GetTwinnerUrlOk returns a tuple with the TwinnerUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTwinnerUrl

`func (o *AutoScout24ListingDetail) SetTwinnerUrl(v string)`

SetTwinnerUrl sets TwinnerUrl field to given value.

### HasTwinnerUrl

`func (o *AutoScout24ListingDetail) HasTwinnerUrl() bool`

HasTwinnerUrl returns a boolean if a field has been set.

### SetTwinnerUrlNil

`func (o *AutoScout24ListingDetail) SetTwinnerUrlNil(b bool)`

 SetTwinnerUrlNil sets the value for TwinnerUrl to be an explicit nil

### UnsetTwinnerUrl
`func (o *AutoScout24ListingDetail) UnsetTwinnerUrl()`

UnsetTwinnerUrl ensures that no value is present for TwinnerUrl, not even an explicit nil
### GetHas360View

`func (o *AutoScout24ListingDetail) GetHas360View() bool`

GetHas360View returns the Has360View field if non-nil, zero value otherwise.

### GetHas360ViewOk

`func (o *AutoScout24ListingDetail) GetHas360ViewOk() (*bool, bool)`

GetHas360ViewOk returns a tuple with the Has360View field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHas360View

`func (o *AutoScout24ListingDetail) SetHas360View(v bool)`

SetHas360View sets Has360View field to given value.

### HasHas360View

`func (o *AutoScout24ListingDetail) HasHas360View() bool`

HasHas360View returns a boolean if a field has been set.

### SetHas360ViewNil

`func (o *AutoScout24ListingDetail) SetHas360ViewNil(b bool)`

 SetHas360ViewNil sets the value for Has360View to be an explicit nil

### UnsetHas360View
`func (o *AutoScout24ListingDetail) UnsetHas360View()`

UnsetHas360View ensures that no value is present for Has360View, not even an explicit nil
### GetThreeSixty

`func (o *AutoScout24ListingDetail) GetThreeSixty() interface{}`

GetThreeSixty returns the ThreeSixty field if non-nil, zero value otherwise.

### GetThreeSixtyOk

`func (o *AutoScout24ListingDetail) GetThreeSixtyOk() (*interface{}, bool)`

GetThreeSixtyOk returns a tuple with the ThreeSixty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThreeSixty

`func (o *AutoScout24ListingDetail) SetThreeSixty(v interface{})`

SetThreeSixty sets ThreeSixty field to given value.

### HasThreeSixty

`func (o *AutoScout24ListingDetail) HasThreeSixty() bool`

HasThreeSixty returns a boolean if a field has been set.

### SetThreeSixtyNil

`func (o *AutoScout24ListingDetail) SetThreeSixtyNil(b bool)`

 SetThreeSixtyNil sets the value for ThreeSixty to be an explicit nil

### UnsetThreeSixty
`func (o *AutoScout24ListingDetail) UnsetThreeSixty()`

UnsetThreeSixty ensures that no value is present for ThreeSixty, not even an explicit nil
### GetVehicleReport

`func (o *AutoScout24ListingDetail) GetVehicleReport() interface{}`

GetVehicleReport returns the VehicleReport field if non-nil, zero value otherwise.

### GetVehicleReportOk

`func (o *AutoScout24ListingDetail) GetVehicleReportOk() (*interface{}, bool)`

GetVehicleReportOk returns a tuple with the VehicleReport field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVehicleReport

`func (o *AutoScout24ListingDetail) SetVehicleReport(v interface{})`

SetVehicleReport sets VehicleReport field to given value.

### HasVehicleReport

`func (o *AutoScout24ListingDetail) HasVehicleReport() bool`

HasVehicleReport returns a boolean if a field has been set.

### SetVehicleReportNil

`func (o *AutoScout24ListingDetail) SetVehicleReportNil(b bool)`

 SetVehicleReportNil sets the value for VehicleReport to be an explicit nil

### UnsetVehicleReport
`func (o *AutoScout24ListingDetail) UnsetVehicleReport()`

UnsetVehicleReport ensures that no value is present for VehicleReport, not even an explicit nil
### GetPartnerIntegrations

`func (o *AutoScout24ListingDetail) GetPartnerIntegrations() []*map[string]interface{}`

GetPartnerIntegrations returns the PartnerIntegrations field if non-nil, zero value otherwise.

### GetPartnerIntegrationsOk

`func (o *AutoScout24ListingDetail) GetPartnerIntegrationsOk() (*[]*map[string]interface{}, bool)`

GetPartnerIntegrationsOk returns a tuple with the PartnerIntegrations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPartnerIntegrations

`func (o *AutoScout24ListingDetail) SetPartnerIntegrations(v []*map[string]interface{})`

SetPartnerIntegrations sets PartnerIntegrations field to given value.

### HasPartnerIntegrations

`func (o *AutoScout24ListingDetail) HasPartnerIntegrations() bool`

HasPartnerIntegrations returns a boolean if a field has been set.

### GetSeller

`func (o *AutoScout24ListingDetail) GetSeller() map[string]interface{}`

GetSeller returns the Seller field if non-nil, zero value otherwise.

### GetSellerOk

`func (o *AutoScout24ListingDetail) GetSellerOk() (*map[string]interface{}, bool)`

GetSellerOk returns a tuple with the Seller field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeller

`func (o *AutoScout24ListingDetail) SetSeller(v map[string]interface{})`

SetSeller sets Seller field to given value.

### HasSeller

`func (o *AutoScout24ListingDetail) HasSeller() bool`

HasSeller returns a boolean if a field has been set.

### GetLocation

`func (o *AutoScout24ListingDetail) GetLocation() map[string]interface{}`

GetLocation returns the Location field if non-nil, zero value otherwise.

### GetLocationOk

`func (o *AutoScout24ListingDetail) GetLocationOk() (*map[string]interface{}, bool)`

GetLocationOk returns a tuple with the Location field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocation

`func (o *AutoScout24ListingDetail) SetLocation(v map[string]interface{})`

SetLocation sets Location field to given value.

### HasLocation

`func (o *AutoScout24ListingDetail) HasLocation() bool`

HasLocation returns a boolean if a field has been set.

### GetRatings

`func (o *AutoScout24ListingDetail) GetRatings() map[string]interface{}`

GetRatings returns the Ratings field if non-nil, zero value otherwise.

### GetRatingsOk

`func (o *AutoScout24ListingDetail) GetRatingsOk() (*map[string]interface{}, bool)`

GetRatingsOk returns a tuple with the Ratings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRatings

`func (o *AutoScout24ListingDetail) SetRatings(v map[string]interface{})`

SetRatings sets Ratings field to given value.

### HasRatings

`func (o *AutoScout24ListingDetail) HasRatings() bool`

HasRatings returns a boolean if a field has been set.

### GetRating

`func (o *AutoScout24ListingDetail) GetRating() float32`

GetRating returns the Rating field if non-nil, zero value otherwise.

### GetRatingOk

`func (o *AutoScout24ListingDetail) GetRatingOk() (*float32, bool)`

GetRatingOk returns a tuple with the Rating field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRating

`func (o *AutoScout24ListingDetail) SetRating(v float32)`

SetRating sets Rating field to given value.

### HasRating

`func (o *AutoScout24ListingDetail) HasRating() bool`

HasRating returns a boolean if a field has been set.

### SetRatingNil

`func (o *AutoScout24ListingDetail) SetRatingNil(b bool)`

 SetRatingNil sets the value for Rating to be an explicit nil

### UnsetRating
`func (o *AutoScout24ListingDetail) UnsetRating()`

UnsetRating ensures that no value is present for Rating, not even an explicit nil
### GetRatingCount

`func (o *AutoScout24ListingDetail) GetRatingCount() int32`

GetRatingCount returns the RatingCount field if non-nil, zero value otherwise.

### GetRatingCountOk

`func (o *AutoScout24ListingDetail) GetRatingCountOk() (*int32, bool)`

GetRatingCountOk returns a tuple with the RatingCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRatingCount

`func (o *AutoScout24ListingDetail) SetRatingCount(v int32)`

SetRatingCount sets RatingCount field to given value.

### HasRatingCount

`func (o *AutoScout24ListingDetail) HasRatingCount() bool`

HasRatingCount returns a boolean if a field has been set.

### SetRatingCountNil

`func (o *AutoScout24ListingDetail) SetRatingCountNil(b bool)`

 SetRatingCountNil sets the value for RatingCount to be an explicit nil

### UnsetRatingCount
`func (o *AutoScout24ListingDetail) UnsetRatingCount()`

UnsetRatingCount ensures that no value is present for RatingCount, not even an explicit nil
### GetRecommendPercentage

`func (o *AutoScout24ListingDetail) GetRecommendPercentage() float32`

GetRecommendPercentage returns the RecommendPercentage field if non-nil, zero value otherwise.

### GetRecommendPercentageOk

`func (o *AutoScout24ListingDetail) GetRecommendPercentageOk() (*float32, bool)`

GetRecommendPercentageOk returns a tuple with the RecommendPercentage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecommendPercentage

`func (o *AutoScout24ListingDetail) SetRecommendPercentage(v float32)`

SetRecommendPercentage sets RecommendPercentage field to given value.

### HasRecommendPercentage

`func (o *AutoScout24ListingDetail) HasRecommendPercentage() bool`

HasRecommendPercentage returns a boolean if a field has been set.

### SetRecommendPercentageNil

`func (o *AutoScout24ListingDetail) SetRecommendPercentageNil(b bool)`

 SetRecommendPercentageNil sets the value for RecommendPercentage to be an explicit nil

### UnsetRecommendPercentage
`func (o *AutoScout24ListingDetail) UnsetRecommendPercentage()`

UnsetRecommendPercentage ensures that no value is present for RecommendPercentage, not even an explicit nil
### GetWhatsappNumber

`func (o *AutoScout24ListingDetail) GetWhatsappNumber() string`

GetWhatsappNumber returns the WhatsappNumber field if non-nil, zero value otherwise.

### GetWhatsappNumberOk

`func (o *AutoScout24ListingDetail) GetWhatsappNumberOk() (*string, bool)`

GetWhatsappNumberOk returns a tuple with the WhatsappNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWhatsappNumber

`func (o *AutoScout24ListingDetail) SetWhatsappNumber(v string)`

SetWhatsappNumber sets WhatsappNumber field to given value.

### HasWhatsappNumber

`func (o *AutoScout24ListingDetail) HasWhatsappNumber() bool`

HasWhatsappNumber returns a boolean if a field has been set.

### SetWhatsappNumberNil

`func (o *AutoScout24ListingDetail) SetWhatsappNumberNil(b bool)`

 SetWhatsappNumberNil sets the value for WhatsappNumber to be an explicit nil

### UnsetWhatsappNumber
`func (o *AutoScout24ListingDetail) UnsetWhatsappNumber()`

UnsetWhatsappNumber ensures that no value is present for WhatsappNumber, not even an explicit nil
### GetIdentifier

`func (o *AutoScout24ListingDetail) GetIdentifier() map[string]interface{}`

GetIdentifier returns the Identifier field if non-nil, zero value otherwise.

### GetIdentifierOk

`func (o *AutoScout24ListingDetail) GetIdentifierOk() (*map[string]interface{}, bool)`

GetIdentifierOk returns a tuple with the Identifier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIdentifier

`func (o *AutoScout24ListingDetail) SetIdentifier(v map[string]interface{})`

SetIdentifier sets Identifier field to given value.

### HasIdentifier

`func (o *AutoScout24ListingDetail) HasIdentifier() bool`

HasIdentifier returns a boolean if a field has been set.

### GetArticleType

`func (o *AutoScout24ListingDetail) GetArticleType() string`

GetArticleType returns the ArticleType field if non-nil, zero value otherwise.

### GetArticleTypeOk

`func (o *AutoScout24ListingDetail) GetArticleTypeOk() (*string, bool)`

GetArticleTypeOk returns a tuple with the ArticleType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArticleType

`func (o *AutoScout24ListingDetail) SetArticleType(v string)`

SetArticleType sets ArticleType field to given value.

### HasArticleType

`func (o *AutoScout24ListingDetail) HasArticleType() bool`

HasArticleType returns a boolean if a field has been set.

### SetArticleTypeNil

`func (o *AutoScout24ListingDetail) SetArticleTypeNil(b bool)`

 SetArticleTypeNil sets the value for ArticleType to be an explicit nil

### UnsetArticleType
`func (o *AutoScout24ListingDetail) UnsetArticleType()`

UnsetArticleType ensures that no value is present for ArticleType, not even an explicit nil
### GetVehicleType

`func (o *AutoScout24ListingDetail) GetVehicleType() string`

GetVehicleType returns the VehicleType field if non-nil, zero value otherwise.

### GetVehicleTypeOk

`func (o *AutoScout24ListingDetail) GetVehicleTypeOk() (*string, bool)`

GetVehicleTypeOk returns a tuple with the VehicleType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVehicleType

`func (o *AutoScout24ListingDetail) SetVehicleType(v string)`

SetVehicleType sets VehicleType field to given value.

### HasVehicleType

`func (o *AutoScout24ListingDetail) HasVehicleType() bool`

HasVehicleType returns a boolean if a field has been set.

### SetVehicleTypeNil

`func (o *AutoScout24ListingDetail) SetVehicleTypeNil(b bool)`

 SetVehicleTypeNil sets the value for VehicleType to be an explicit nil

### UnsetVehicleType
`func (o *AutoScout24ListingDetail) UnsetVehicleType()`

UnsetVehicleType ensures that no value is present for VehicleType, not even an explicit nil
### GetIsNew

`func (o *AutoScout24ListingDetail) GetIsNew() bool`

GetIsNew returns the IsNew field if non-nil, zero value otherwise.

### GetIsNewOk

`func (o *AutoScout24ListingDetail) GetIsNewOk() (*bool, bool)`

GetIsNewOk returns a tuple with the IsNew field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsNew

`func (o *AutoScout24ListingDetail) SetIsNew(v bool)`

SetIsNew sets IsNew field to given value.

### HasIsNew

`func (o *AutoScout24ListingDetail) HasIsNew() bool`

HasIsNew returns a boolean if a field has been set.

### SetIsNewNil

`func (o *AutoScout24ListingDetail) SetIsNewNil(b bool)`

 SetIsNewNil sets the value for IsNew to be an explicit nil

### UnsetIsNew
`func (o *AutoScout24ListingDetail) UnsetIsNew()`

UnsetIsNew ensures that no value is present for IsNew, not even an explicit nil
### GetIsDeliverable

`func (o *AutoScout24ListingDetail) GetIsDeliverable() bool`

GetIsDeliverable returns the IsDeliverable field if non-nil, zero value otherwise.

### GetIsDeliverableOk

`func (o *AutoScout24ListingDetail) GetIsDeliverableOk() (*bool, bool)`

GetIsDeliverableOk returns a tuple with the IsDeliverable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDeliverable

`func (o *AutoScout24ListingDetail) SetIsDeliverable(v bool)`

SetIsDeliverable sets IsDeliverable field to given value.

### HasIsDeliverable

`func (o *AutoScout24ListingDetail) HasIsDeliverable() bool`

HasIsDeliverable returns a boolean if a field has been set.

### SetIsDeliverableNil

`func (o *AutoScout24ListingDetail) SetIsDeliverableNil(b bool)`

 SetIsDeliverableNil sets the value for IsDeliverable to be an explicit nil

### UnsetIsDeliverable
`func (o *AutoScout24ListingDetail) UnsetIsDeliverable()`

UnsetIsDeliverable ensures that no value is present for IsDeliverable, not even an explicit nil
### GetAvailability

`func (o *AutoScout24ListingDetail) GetAvailability() map[string]interface{}`

GetAvailability returns the Availability field if non-nil, zero value otherwise.

### GetAvailabilityOk

`func (o *AutoScout24ListingDetail) GetAvailabilityOk() (*map[string]interface{}, bool)`

GetAvailabilityOk returns a tuple with the Availability field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAvailability

`func (o *AutoScout24ListingDetail) SetAvailability(v map[string]interface{})`

SetAvailability sets Availability field to given value.

### HasAvailability

`func (o *AutoScout24ListingDetail) HasAvailability() bool`

HasAvailability returns a boolean if a field has been set.

### GetAvailableAt

`func (o *AutoScout24ListingDetail) GetAvailableAt() string`

GetAvailableAt returns the AvailableAt field if non-nil, zero value otherwise.

### GetAvailableAtOk

`func (o *AutoScout24ListingDetail) GetAvailableAtOk() (*string, bool)`

GetAvailableAtOk returns a tuple with the AvailableAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAvailableAt

`func (o *AutoScout24ListingDetail) SetAvailableAt(v string)`

SetAvailableAt sets AvailableAt field to given value.

### HasAvailableAt

`func (o *AutoScout24ListingDetail) HasAvailableAt() bool`

HasAvailableAt returns a boolean if a field has been set.

### SetAvailableAtNil

`func (o *AutoScout24ListingDetail) SetAvailableAtNil(b bool)`

 SetAvailableAtNil sets the value for AvailableAt to be an explicit nil

### UnsetAvailableAt
`func (o *AutoScout24ListingDetail) UnsetAvailableAt()`

UnsetAvailableAt ensures that no value is present for AvailableAt, not even an explicit nil
### GetAvailableUtc

`func (o *AutoScout24ListingDetail) GetAvailableUtc() float32`

GetAvailableUtc returns the AvailableUtc field if non-nil, zero value otherwise.

### GetAvailableUtcOk

`func (o *AutoScout24ListingDetail) GetAvailableUtcOk() (*float32, bool)`

GetAvailableUtcOk returns a tuple with the AvailableUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAvailableUtc

`func (o *AutoScout24ListingDetail) SetAvailableUtc(v float32)`

SetAvailableUtc sets AvailableUtc field to given value.

### HasAvailableUtc

`func (o *AutoScout24ListingDetail) HasAvailableUtc() bool`

HasAvailableUtc returns a boolean if a field has been set.

### SetAvailableUtcNil

`func (o *AutoScout24ListingDetail) SetAvailableUtcNil(b bool)`

 SetAvailableUtcNil sets the value for AvailableUtc to be an explicit nil

### UnsetAvailableUtc
`func (o *AutoScout24ListingDetail) UnsetAvailableUtc()`

UnsetAvailableUtc ensures that no value is present for AvailableUtc, not even an explicit nil
### GetCreatedAt

`func (o *AutoScout24ListingDetail) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *AutoScout24ListingDetail) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *AutoScout24ListingDetail) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *AutoScout24ListingDetail) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### SetCreatedAtNil

`func (o *AutoScout24ListingDetail) SetCreatedAtNil(b bool)`

 SetCreatedAtNil sets the value for CreatedAt to be an explicit nil

### UnsetCreatedAt
`func (o *AutoScout24ListingDetail) UnsetCreatedAt()`

UnsetCreatedAt ensures that no value is present for CreatedAt, not even an explicit nil
### GetCreatedUtc

`func (o *AutoScout24ListingDetail) GetCreatedUtc() float32`

GetCreatedUtc returns the CreatedUtc field if non-nil, zero value otherwise.

### GetCreatedUtcOk

`func (o *AutoScout24ListingDetail) GetCreatedUtcOk() (*float32, bool)`

GetCreatedUtcOk returns a tuple with the CreatedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedUtc

`func (o *AutoScout24ListingDetail) SetCreatedUtc(v float32)`

SetCreatedUtc sets CreatedUtc field to given value.

### HasCreatedUtc

`func (o *AutoScout24ListingDetail) HasCreatedUtc() bool`

HasCreatedUtc returns a boolean if a field has been set.

### SetCreatedUtcNil

`func (o *AutoScout24ListingDetail) SetCreatedUtcNil(b bool)`

 SetCreatedUtcNil sets the value for CreatedUtc to be an explicit nil

### UnsetCreatedUtc
`func (o *AutoScout24ListingDetail) UnsetCreatedUtc()`

UnsetCreatedUtc ensures that no value is present for CreatedUtc, not even an explicit nil
### GetLeasingDetails

`func (o *AutoScout24ListingDetail) GetLeasingDetails() interface{}`

GetLeasingDetails returns the LeasingDetails field if non-nil, zero value otherwise.

### GetLeasingDetailsOk

`func (o *AutoScout24ListingDetail) GetLeasingDetailsOk() (*interface{}, bool)`

GetLeasingDetailsOk returns a tuple with the LeasingDetails field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLeasingDetails

`func (o *AutoScout24ListingDetail) SetLeasingDetails(v interface{})`

SetLeasingDetails sets LeasingDetails field to given value.

### HasLeasingDetails

`func (o *AutoScout24ListingDetail) HasLeasingDetails() bool`

HasLeasingDetails returns a boolean if a field has been set.

### SetLeasingDetailsNil

`func (o *AutoScout24ListingDetail) SetLeasingDetailsNil(b bool)`

 SetLeasingDetailsNil sets the value for LeasingDetails to be an explicit nil

### UnsetLeasingDetails
`func (o *AutoScout24ListingDetail) UnsetLeasingDetails()`

UnsetLeasingDetails ensures that no value is present for LeasingDetails, not even an explicit nil
### GetWarranty

`func (o *AutoScout24ListingDetail) GetWarranty() interface{}`

GetWarranty returns the Warranty field if non-nil, zero value otherwise.

### GetWarrantyOk

`func (o *AutoScout24ListingDetail) GetWarrantyOk() (*interface{}, bool)`

GetWarrantyOk returns a tuple with the Warranty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWarranty

`func (o *AutoScout24ListingDetail) SetWarranty(v interface{})`

SetWarranty sets Warranty field to given value.

### HasWarranty

`func (o *AutoScout24ListingDetail) HasWarranty() bool`

HasWarranty returns a boolean if a field has been set.

### SetWarrantyNil

`func (o *AutoScout24ListingDetail) SetWarrantyNil(b bool)`

 SetWarrantyNil sets the value for Warranty to be an explicit nil

### UnsetWarranty
`func (o *AutoScout24ListingDetail) UnsetWarranty()`

UnsetWarranty ensures that no value is present for Warranty, not even an explicit nil
### GetHasWarranty

`func (o *AutoScout24ListingDetail) GetHasWarranty() bool`

GetHasWarranty returns the HasWarranty field if non-nil, zero value otherwise.

### GetHasWarrantyOk

`func (o *AutoScout24ListingDetail) GetHasWarrantyOk() (*bool, bool)`

GetHasWarrantyOk returns a tuple with the HasWarranty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasWarranty

`func (o *AutoScout24ListingDetail) SetHasWarranty(v bool)`

SetHasWarranty sets HasWarranty field to given value.

### HasHasWarranty

`func (o *AutoScout24ListingDetail) HasHasWarranty() bool`

HasHasWarranty returns a boolean if a field has been set.

### SetHasWarrantyNil

`func (o *AutoScout24ListingDetail) SetHasWarrantyNil(b bool)`

 SetHasWarrantyNil sets the value for HasWarranty to be an explicit nil

### UnsetHasWarranty
`func (o *AutoScout24ListingDetail) UnsetHasWarranty()`

UnsetHasWarranty ensures that no value is present for HasWarranty, not even an explicit nil
### GetFinancingFlags

`func (o *AutoScout24ListingDetail) GetFinancingFlags() interface{}`

GetFinancingFlags returns the FinancingFlags field if non-nil, zero value otherwise.

### GetFinancingFlagsOk

`func (o *AutoScout24ListingDetail) GetFinancingFlagsOk() (*interface{}, bool)`

GetFinancingFlagsOk returns a tuple with the FinancingFlags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFinancingFlags

`func (o *AutoScout24ListingDetail) SetFinancingFlags(v interface{})`

SetFinancingFlags sets FinancingFlags field to given value.

### HasFinancingFlags

`func (o *AutoScout24ListingDetail) HasFinancingFlags() bool`

HasFinancingFlags returns a boolean if a field has been set.

### SetFinancingFlagsNil

`func (o *AutoScout24ListingDetail) SetFinancingFlagsNil(b bool)`

 SetFinancingFlagsNil sets the value for FinancingFlags to be an explicit nil

### UnsetFinancingFlags
`func (o *AutoScout24ListingDetail) UnsetFinancingFlags()`

UnsetFinancingFlags ensures that no value is present for FinancingFlags, not even an explicit nil
### GetFinancingAndInsurance

`func (o *AutoScout24ListingDetail) GetFinancingAndInsurance() interface{}`

GetFinancingAndInsurance returns the FinancingAndInsurance field if non-nil, zero value otherwise.

### GetFinancingAndInsuranceOk

`func (o *AutoScout24ListingDetail) GetFinancingAndInsuranceOk() (*interface{}, bool)`

GetFinancingAndInsuranceOk returns a tuple with the FinancingAndInsurance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFinancingAndInsurance

`func (o *AutoScout24ListingDetail) SetFinancingAndInsurance(v interface{})`

SetFinancingAndInsurance sets FinancingAndInsurance field to given value.

### HasFinancingAndInsurance

`func (o *AutoScout24ListingDetail) HasFinancingAndInsurance() bool`

HasFinancingAndInsurance returns a boolean if a field has been set.

### SetFinancingAndInsuranceNil

`func (o *AutoScout24ListingDetail) SetFinancingAndInsuranceNil(b bool)`

 SetFinancingAndInsuranceNil sets the value for FinancingAndInsurance to be an explicit nil

### UnsetFinancingAndInsurance
`func (o *AutoScout24ListingDetail) UnsetFinancingAndInsurance()`

UnsetFinancingAndInsurance ensures that no value is present for FinancingAndInsurance, not even an explicit nil
### GetOnlinePurchase

`func (o *AutoScout24ListingDetail) GetOnlinePurchase() interface{}`

GetOnlinePurchase returns the OnlinePurchase field if non-nil, zero value otherwise.

### GetOnlinePurchaseOk

`func (o *AutoScout24ListingDetail) GetOnlinePurchaseOk() (*interface{}, bool)`

GetOnlinePurchaseOk returns a tuple with the OnlinePurchase field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOnlinePurchase

`func (o *AutoScout24ListingDetail) SetOnlinePurchase(v interface{})`

SetOnlinePurchase sets OnlinePurchase field to given value.

### HasOnlinePurchase

`func (o *AutoScout24ListingDetail) HasOnlinePurchase() bool`

HasOnlinePurchase returns a boolean if a field has been set.

### SetOnlinePurchaseNil

`func (o *AutoScout24ListingDetail) SetOnlinePurchaseNil(b bool)`

 SetOnlinePurchaseNil sets the value for OnlinePurchase to be an explicit nil

### UnsetOnlinePurchase
`func (o *AutoScout24ListingDetail) UnsetOnlinePurchase()`

UnsetOnlinePurchase ensures that no value is present for OnlinePurchase, not even an explicit nil
### GetSeals

`func (o *AutoScout24ListingDetail) GetSeals() []interface{}`

GetSeals returns the Seals field if non-nil, zero value otherwise.

### GetSealsOk

`func (o *AutoScout24ListingDetail) GetSealsOk() (*[]interface{}, bool)`

GetSealsOk returns a tuple with the Seals field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeals

`func (o *AutoScout24ListingDetail) SetSeals(v []interface{})`

SetSeals sets Seals field to given value.

### HasSeals

`func (o *AutoScout24ListingDetail) HasSeals() bool`

HasSeals returns a boolean if a field has been set.

### GetSpecialConditions

`func (o *AutoScout24ListingDetail) GetSpecialConditions() []interface{}`

GetSpecialConditions returns the SpecialConditions field if non-nil, zero value otherwise.

### GetSpecialConditionsOk

`func (o *AutoScout24ListingDetail) GetSpecialConditionsOk() (*[]interface{}, bool)`

GetSpecialConditionsOk returns a tuple with the SpecialConditions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSpecialConditions

`func (o *AutoScout24ListingDetail) SetSpecialConditions(v []interface{})`

SetSpecialConditions sets SpecialConditions field to given value.

### HasSpecialConditions

`func (o *AutoScout24ListingDetail) HasSpecialConditions() bool`

HasSpecialConditions returns a boolean if a field has been set.

### GetSearchResultType

`func (o *AutoScout24ListingDetail) GetSearchResultType() string`

GetSearchResultType returns the SearchResultType field if non-nil, zero value otherwise.

### GetSearchResultTypeOk

`func (o *AutoScout24ListingDetail) GetSearchResultTypeOk() (*string, bool)`

GetSearchResultTypeOk returns a tuple with the SearchResultType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSearchResultType

`func (o *AutoScout24ListingDetail) SetSearchResultType(v string)`

SetSearchResultType sets SearchResultType field to given value.

### HasSearchResultType

`func (o *AutoScout24ListingDetail) HasSearchResultType() bool`

HasSearchResultType returns a boolean if a field has been set.

### SetSearchResultTypeNil

`func (o *AutoScout24ListingDetail) SetSearchResultTypeNil(b bool)`

 SetSearchResultTypeNil sets the value for SearchResultType to be an explicit nil

### UnsetSearchResultType
`func (o *AutoScout24ListingDetail) UnsetSearchResultType()`

UnsetSearchResultType ensures that no value is present for SearchResultType, not even an explicit nil
### GetAdTier

`func (o *AutoScout24ListingDetail) GetAdTier() string`

GetAdTier returns the AdTier field if non-nil, zero value otherwise.

### GetAdTierOk

`func (o *AutoScout24ListingDetail) GetAdTierOk() (*string, bool)`

GetAdTierOk returns a tuple with the AdTier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdTier

`func (o *AutoScout24ListingDetail) SetAdTier(v string)`

SetAdTier sets AdTier field to given value.

### HasAdTier

`func (o *AutoScout24ListingDetail) HasAdTier() bool`

HasAdTier returns a boolean if a field has been set.

### SetAdTierNil

`func (o *AutoScout24ListingDetail) SetAdTierNil(b bool)`

 SetAdTierNil sets the value for AdTier to be an explicit nil

### UnsetAdTier
`func (o *AutoScout24ListingDetail) UnsetAdTier()`

UnsetAdTier ensures that no value is present for AdTier, not even an explicit nil
### GetAppliedAdTier

`func (o *AutoScout24ListingDetail) GetAppliedAdTier() string`

GetAppliedAdTier returns the AppliedAdTier field if non-nil, zero value otherwise.

### GetAppliedAdTierOk

`func (o *AutoScout24ListingDetail) GetAppliedAdTierOk() (*string, bool)`

GetAppliedAdTierOk returns a tuple with the AppliedAdTier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAppliedAdTier

`func (o *AutoScout24ListingDetail) SetAppliedAdTier(v string)`

SetAppliedAdTier sets AppliedAdTier field to given value.

### HasAppliedAdTier

`func (o *AutoScout24ListingDetail) HasAppliedAdTier() bool`

HasAppliedAdTier returns a boolean if a field has been set.

### SetAppliedAdTierNil

`func (o *AutoScout24ListingDetail) SetAppliedAdTierNil(b bool)`

 SetAppliedAdTierNil sets the value for AppliedAdTier to be an explicit nil

### UnsetAppliedAdTier
`func (o *AutoScout24ListingDetail) UnsetAppliedAdTier()`

UnsetAppliedAdTier ensures that no value is present for AppliedAdTier, not even an explicit nil
### GetHasPremiumListingTreatment

`func (o *AutoScout24ListingDetail) GetHasPremiumListingTreatment() bool`

GetHasPremiumListingTreatment returns the HasPremiumListingTreatment field if non-nil, zero value otherwise.

### GetHasPremiumListingTreatmentOk

`func (o *AutoScout24ListingDetail) GetHasPremiumListingTreatmentOk() (*bool, bool)`

GetHasPremiumListingTreatmentOk returns a tuple with the HasPremiumListingTreatment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasPremiumListingTreatment

`func (o *AutoScout24ListingDetail) SetHasPremiumListingTreatment(v bool)`

SetHasPremiumListingTreatment sets HasPremiumListingTreatment field to given value.

### HasHasPremiumListingTreatment

`func (o *AutoScout24ListingDetail) HasHasPremiumListingTreatment() bool`

HasHasPremiumListingTreatment returns a boolean if a field has been set.

### SetHasPremiumListingTreatmentNil

`func (o *AutoScout24ListingDetail) SetHasPremiumListingTreatmentNil(b bool)`

 SetHasPremiumListingTreatmentNil sets the value for HasPremiumListingTreatment to be an explicit nil

### UnsetHasPremiumListingTreatment
`func (o *AutoScout24ListingDetail) UnsetHasPremiumListingTreatment()`

UnsetHasPremiumListingTreatment ensures that no value is present for HasPremiumListingTreatment, not even an explicit nil
### GetIsTrending

`func (o *AutoScout24ListingDetail) GetIsTrending() bool`

GetIsTrending returns the IsTrending field if non-nil, zero value otherwise.

### GetIsTrendingOk

`func (o *AutoScout24ListingDetail) GetIsTrendingOk() (*bool, bool)`

GetIsTrendingOk returns a tuple with the IsTrending field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsTrending

`func (o *AutoScout24ListingDetail) SetIsTrending(v bool)`

SetIsTrending sets IsTrending field to given value.

### HasIsTrending

`func (o *AutoScout24ListingDetail) HasIsTrending() bool`

HasIsTrending returns a boolean if a field has been set.

### SetIsTrendingNil

`func (o *AutoScout24ListingDetail) SetIsTrendingNil(b bool)`

 SetIsTrendingNil sets the value for IsTrending to be an explicit nil

### UnsetIsTrending
`func (o *AutoScout24ListingDetail) UnsetIsTrending()`

UnsetIsTrending ensures that no value is present for IsTrending, not even an explicit nil
### GetIsListingBoost

`func (o *AutoScout24ListingDetail) GetIsListingBoost() bool`

GetIsListingBoost returns the IsListingBoost field if non-nil, zero value otherwise.

### GetIsListingBoostOk

`func (o *AutoScout24ListingDetail) GetIsListingBoostOk() (*bool, bool)`

GetIsListingBoostOk returns a tuple with the IsListingBoost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsListingBoost

`func (o *AutoScout24ListingDetail) SetIsListingBoost(v bool)`

SetIsListingBoost sets IsListingBoost field to given value.

### HasIsListingBoost

`func (o *AutoScout24ListingDetail) HasIsListingBoost() bool`

HasIsListingBoost returns a boolean if a field has been set.

### SetIsListingBoostNil

`func (o *AutoScout24ListingDetail) SetIsListingBoostNil(b bool)`

 SetIsListingBoostNil sets the value for IsListingBoost to be an explicit nil

### UnsetIsListingBoost
`func (o *AutoScout24ListingDetail) UnsetIsListingBoost()`

UnsetIsListingBoost ensures that no value is present for IsListingBoost, not even an explicit nil
### GetStatistics

`func (o *AutoScout24ListingDetail) GetStatistics() map[string]interface{}`

GetStatistics returns the Statistics field if non-nil, zero value otherwise.

### GetStatisticsOk

`func (o *AutoScout24ListingDetail) GetStatisticsOk() (*map[string]interface{}, bool)`

GetStatisticsOk returns a tuple with the Statistics field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatistics

`func (o *AutoScout24ListingDetail) SetStatistics(v map[string]interface{})`

SetStatistics sets Statistics field to given value.

### HasStatistics

`func (o *AutoScout24ListingDetail) HasStatistics() bool`

HasStatistics returns a boolean if a field has been set.

### GetInteractionStatistics

`func (o *AutoScout24ListingDetail) GetInteractionStatistics() map[string]interface{}`

GetInteractionStatistics returns the InteractionStatistics field if non-nil, zero value otherwise.

### GetInteractionStatisticsOk

`func (o *AutoScout24ListingDetail) GetInteractionStatisticsOk() (*map[string]interface{}, bool)`

GetInteractionStatisticsOk returns a tuple with the InteractionStatistics field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInteractionStatistics

`func (o *AutoScout24ListingDetail) SetInteractionStatistics(v map[string]interface{})`

SetInteractionStatistics sets InteractionStatistics field to given value.

### HasInteractionStatistics

`func (o *AutoScout24ListingDetail) HasInteractionStatistics() bool`

HasInteractionStatistics returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# \AutoScout24API

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Autoscout24CheckAutoscout24Health**](AutoScout24API.md#Autoscout24CheckAutoscout24Health) | **Get** /v1/autoscout24/health | Check AutoScout24 health
[**Autoscout24GetListing**](AutoScout24API.md#Autoscout24GetListing) | **Get** /v1/autoscout24/listing | Get listing
[**Autoscout24ListMarkets**](AutoScout24API.md#Autoscout24ListMarkets) | **Get** /v1/autoscout24/markets | List markets
[**Autoscout24ListSearchFilters**](AutoScout24API.md#Autoscout24ListSearchFilters) | **Get** /v1/autoscout24/filters | List search filters
[**Autoscout24SearchVehicles**](AutoScout24API.md#Autoscout24SearchVehicles) | **Get** /v1/autoscout24/search | Search vehicles



## Autoscout24CheckAutoscout24Health

> interface{} Autoscout24CheckAutoscout24Health(ctx).Execute()

Check AutoScout24 health

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/scrape-badger/scrapebadger-go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutoScout24API.Autoscout24CheckAutoscout24Health(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutoScout24API.Autoscout24CheckAutoscout24Health``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Autoscout24CheckAutoscout24Health`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AutoScout24API.Autoscout24CheckAutoscout24Health`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAutoscout24CheckAutoscout24HealthRequest struct via the builder pattern


### Return type

**interface{}**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## Autoscout24GetListing

> AutoScout24ListingResponse Autoscout24GetListing(ctx).Url(url).ListingId(listingId).Market(market).Execute()

Get listing



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/scrape-badger/scrapebadger-go"
)

func main() {
	url := "url_example" // string | Full HTTPS listing URL from search results. Supply url or listing_id, not both. (optional)
	listingId := "listingId_example" // string | Listing UUID from search results; requires no SEO slug. (optional)
	market := "market_example" // string | Inferred from URL, otherwise de. Explicit market must match the URL host. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutoScout24API.Autoscout24GetListing(context.Background()).Url(url).ListingId(listingId).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutoScout24API.Autoscout24GetListing``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Autoscout24GetListing`: AutoScout24ListingResponse
	fmt.Fprintf(os.Stdout, "Response from `AutoScout24API.Autoscout24GetListing`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAutoscout24GetListingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **url** | **string** | Full HTTPS listing URL from search results. Supply url or listing_id, not both. | 
 **listingId** | **string** | Listing UUID from search results; requires no SEO slug. | 
 **market** | **string** | Inferred from URL, otherwise de. Explicit market must match the URL host. | 

### Return type

[**AutoScout24ListingResponse**](AutoScout24ListingResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## Autoscout24ListMarkets

> AutoScout24MarketsResponse Autoscout24ListMarkets(ctx).Execute()

List markets



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/scrape-badger/scrapebadger-go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutoScout24API.Autoscout24ListMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutoScout24API.Autoscout24ListMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Autoscout24ListMarkets`: AutoScout24MarketsResponse
	fmt.Fprintf(os.Stdout, "Response from `AutoScout24API.Autoscout24ListMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAutoscout24ListMarketsRequest struct via the builder pattern


### Return type

[**AutoScout24MarketsResponse**](AutoScout24MarketsResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## Autoscout24ListSearchFilters

> AutoScout24FiltersResponse Autoscout24ListSearchFilters(ctx).Market(market).Make(make).Execute()

List search filters



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/scrape-badger/scrapebadger-go"
)

func main() {
	market := "market_example" // string |  (optional) (default to "de")
	make := "make_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutoScout24API.Autoscout24ListSearchFilters(context.Background()).Market(market).Make(make).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutoScout24API.Autoscout24ListSearchFilters``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Autoscout24ListSearchFilters`: AutoScout24FiltersResponse
	fmt.Fprintf(os.Stdout, "Response from `AutoScout24API.Autoscout24ListSearchFilters`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAutoscout24ListSearchFiltersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **market** | **string** |  | [default to &quot;de&quot;]
 **make** | **string** |  | 

### Return type

[**AutoScout24FiltersResponse**](AutoScout24FiltersResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## Autoscout24SearchVehicles

> AutoScout24SearchResponse Autoscout24SearchVehicles(ctx).Market(market).Make(make).Model(model).PriceMin(priceMin).PriceMax(priceMax).MileageMin(mileageMin).MileageMax(mileageMax).YearMin(yearMin).YearMax(yearMax).PowerMin(powerMin).PowerMax(powerMax).FuelType(fuelType).Transmission(transmission).BodyType(bodyType).SellerType(sellerType).Condition(condition).Zip(zip).Radius(radius).SortBy(sortBy).Page(page).Execute()

Search vehicles



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/scrape-badger/scrapebadger-go"
)

func main() {
	market := "market_example" // string |  (optional) (default to "de")
	make := "make_example" // string | Native make slug, e.g. volkswagen or bmw. (optional)
	model := "model_example" // string | Native model slug, e.g. golf. Requires make. (optional)
	priceMin := int32(56) // int32 |  (optional)
	priceMax := int32(56) // int32 |  (optional)
	mileageMin := int32(56) // int32 | Kilometres. (optional)
	mileageMax := int32(56) // int32 |  (optional)
	yearMin := int32(56) // int32 |  (optional)
	yearMax := int32(56) // int32 |  (optional)
	powerMin := int32(56) // int32 | Engine power in kW. (optional)
	powerMax := int32(56) // int32 |  (optional)
	fuelType := "fuelType_example" // string |  (optional)
	transmission := "transmission_example" // string |  (optional)
	bodyType := "bodyType_example" // string |  (optional)
	sellerType := "sellerType_example" // string |  (optional)
	condition := "condition_example" // string |  (optional)
	zip := "zip_example" // string | Postal code in the requested market. (optional)
	radius := int32(56) // int32 | Kilometres; requires zip. (optional)
	sortBy := "sortBy_example" // string |  (optional) (default to "best_match")
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutoScout24API.Autoscout24SearchVehicles(context.Background()).Market(market).Make(make).Model(model).PriceMin(priceMin).PriceMax(priceMax).MileageMin(mileageMin).MileageMax(mileageMax).YearMin(yearMin).YearMax(yearMax).PowerMin(powerMin).PowerMax(powerMax).FuelType(fuelType).Transmission(transmission).BodyType(bodyType).SellerType(sellerType).Condition(condition).Zip(zip).Radius(radius).SortBy(sortBy).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutoScout24API.Autoscout24SearchVehicles``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Autoscout24SearchVehicles`: AutoScout24SearchResponse
	fmt.Fprintf(os.Stdout, "Response from `AutoScout24API.Autoscout24SearchVehicles`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAutoscout24SearchVehiclesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **market** | **string** |  | [default to &quot;de&quot;]
 **make** | **string** | Native make slug, e.g. volkswagen or bmw. | 
 **model** | **string** | Native model slug, e.g. golf. Requires make. | 
 **priceMin** | **int32** |  | 
 **priceMax** | **int32** |  | 
 **mileageMin** | **int32** | Kilometres. | 
 **mileageMax** | **int32** |  | 
 **yearMin** | **int32** |  | 
 **yearMax** | **int32** |  | 
 **powerMin** | **int32** | Engine power in kW. | 
 **powerMax** | **int32** |  | 
 **fuelType** | **string** |  | 
 **transmission** | **string** |  | 
 **bodyType** | **string** |  | 
 **sellerType** | **string** |  | 
 **condition** | **string** |  | 
 **zip** | **string** | Postal code in the requested market. | 
 **radius** | **int32** | Kilometres; requires zip. | 
 **sortBy** | **string** |  | [default to &quot;best_match&quot;]
 **page** | **int32** |  | [default to 1]

### Return type

[**AutoScout24SearchResponse**](AutoScout24SearchResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


# \RealtorAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**RealtorGetFullPropertyDetail**](RealtorAPI.md#RealtorGetFullPropertyDetail) | **Get** /v1/realtor/properties/{property_id} | Get full property detail
[**RealtorListMarkets**](RealtorAPI.md#RealtorListMarkets) | **Get** /v1/realtor/markets | List markets
[**RealtorLocationAutocomplete**](RealtorAPI.md#RealtorLocationAutocomplete) | **Get** /v1/realtor/autocomplete | Location autocomplete
[**RealtorRealtorScraperHealthCheck**](RealtorAPI.md#RealtorRealtorScraperHealthCheck) | **Get** /v1/realtor/health | Realtor scraper health check
[**RealtorRealtorScraperHealthCheckHead**](RealtorAPI.md#RealtorRealtorScraperHealthCheckHead) | **Head** /v1/realtor/health | Realtor scraper health check
[**RealtorSearchPropertyListings**](RealtorAPI.md#RealtorSearchPropertyListings) | **Get** /v1/realtor/search | Search property listings



## RealtorGetFullPropertyDetail

> interface{} RealtorGetFullPropertyDetail(ctx, propertyId).Market(market).Execute()

Get full property detail



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
	propertyId := "propertyId_example" // string | 
	market := "market_example" // string | us (realtor.com) | ca (realtor.ca) (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RealtorAPI.RealtorGetFullPropertyDetail(context.Background(), propertyId).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RealtorAPI.RealtorGetFullPropertyDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RealtorGetFullPropertyDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RealtorAPI.RealtorGetFullPropertyDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**propertyId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRealtorGetFullPropertyDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | us (realtor.com) | ca (realtor.ca) | [default to &quot;us&quot;]

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


## RealtorListMarkets

> interface{} RealtorListMarkets(ctx).Execute()

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
	resp, r, err := apiClient.RealtorAPI.RealtorListMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RealtorAPI.RealtorListMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RealtorListMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RealtorAPI.RealtorListMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiRealtorListMarketsRequest struct via the builder pattern


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


## RealtorLocationAutocomplete

> interface{} RealtorLocationAutocomplete(ctx).Query(query).Market(market).Limit(limit).Execute()

Location autocomplete



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
	query := "query_example" // string | Freetext location (city, ZIP/postal, address…)
	market := "market_example" // string | us (realtor.com) | ca (realtor.ca) (optional) (default to "us")
	limit := int32(56) // int32 |  (optional) (default to 10)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RealtorAPI.RealtorLocationAutocomplete(context.Background()).Query(query).Market(market).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RealtorAPI.RealtorLocationAutocomplete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RealtorLocationAutocomplete`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RealtorAPI.RealtorLocationAutocomplete`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRealtorLocationAutocompleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Freetext location (city, ZIP/postal, address…) | 
 **market** | **string** | us (realtor.com) | ca (realtor.ca) | [default to &quot;us&quot;]
 **limit** | **int32** |  | [default to 10]

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


## RealtorRealtorScraperHealthCheck

> interface{} RealtorRealtorScraperHealthCheck(ctx).Execute()

Realtor scraper health check



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
	resp, r, err := apiClient.RealtorAPI.RealtorRealtorScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RealtorAPI.RealtorRealtorScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RealtorRealtorScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RealtorAPI.RealtorRealtorScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiRealtorRealtorScraperHealthCheckRequest struct via the builder pattern


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


## RealtorRealtorScraperHealthCheckHead

> interface{} RealtorRealtorScraperHealthCheckHead(ctx).Execute()

Realtor scraper health check



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
	resp, r, err := apiClient.RealtorAPI.RealtorRealtorScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RealtorAPI.RealtorRealtorScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RealtorRealtorScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RealtorAPI.RealtorRealtorScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiRealtorRealtorScraperHealthCheckHeadRequest struct via the builder pattern


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


## RealtorSearchPropertyListings

> interface{} RealtorSearchPropertyListings(ctx).Location(location).Market(market).Status(status).PriceMin(priceMin).PriceMax(priceMax).BedsMin(bedsMin).BathsMin(bathsMin).SqftMin(sqftMin).SqftMax(sqftMax).PropertyType(propertyType).Sort(sort).Page(page).Limit(limit).LatMin(latMin).LatMax(latMax).LngMin(lngMin).LngMax(lngMax).Execute()

Search property listings



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
	location := "location_example" // string | 'Austin, TX', a ZIP, 'Toronto, ON'… (optional)
	market := "market_example" // string | us (realtor.com) | ca (realtor.ca) (optional) (default to "us")
	status := "status_example" // string | for_sale | for_rent | sold | pending (optional) (default to "for_sale")
	priceMin := float32(8.14) // float32 |  (optional)
	priceMax := float32(8.14) // float32 |  (optional)
	bedsMin := int32(56) // int32 |  (optional)
	bathsMin := int32(56) // int32 |  (optional)
	sqftMin := int32(56) // int32 | US only (optional)
	sqftMax := int32(56) // int32 | US only (optional)
	propertyType := "propertyType_example" // string | US only, CSV of property types (optional)
	sort := "sort_example" // string | relevant | newest | price_low | price_high | photo_count (optional) (default to "relevant")
	page := int32(56) // int32 |  (optional) (default to 1)
	limit := int32(56) // int32 |  (optional)
	latMin := float32(8.14) // float32 | CA bbox south (optional)
	latMax := float32(8.14) // float32 | CA bbox north (optional)
	lngMin := float32(8.14) // float32 | CA bbox west (optional)
	lngMax := float32(8.14) // float32 | CA bbox east (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RealtorAPI.RealtorSearchPropertyListings(context.Background()).Location(location).Market(market).Status(status).PriceMin(priceMin).PriceMax(priceMax).BedsMin(bedsMin).BathsMin(bathsMin).SqftMin(sqftMin).SqftMax(sqftMax).PropertyType(propertyType).Sort(sort).Page(page).Limit(limit).LatMin(latMin).LatMax(latMax).LngMin(lngMin).LngMax(lngMax).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RealtorAPI.RealtorSearchPropertyListings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RealtorSearchPropertyListings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RealtorAPI.RealtorSearchPropertyListings`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRealtorSearchPropertyListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **location** | **string** | &#39;Austin, TX&#39;, a ZIP, &#39;Toronto, ON&#39;… | 
 **market** | **string** | us (realtor.com) | ca (realtor.ca) | [default to &quot;us&quot;]
 **status** | **string** | for_sale | for_rent | sold | pending | [default to &quot;for_sale&quot;]
 **priceMin** | **float32** |  | 
 **priceMax** | **float32** |  | 
 **bedsMin** | **int32** |  | 
 **bathsMin** | **int32** |  | 
 **sqftMin** | **int32** | US only | 
 **sqftMax** | **int32** | US only | 
 **propertyType** | **string** | US only, CSV of property types | 
 **sort** | **string** | relevant | newest | price_low | price_high | photo_count | [default to &quot;relevant&quot;]
 **page** | **int32** |  | [default to 1]
 **limit** | **int32** |  | 
 **latMin** | **float32** | CA bbox south | 
 **latMax** | **float32** | CA bbox north | 
 **lngMin** | **float32** | CA bbox west | 
 **lngMax** | **float32** | CA bbox east | 

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


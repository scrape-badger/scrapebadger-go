# \LoopNetAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**LoopnetGetBrokerProfile**](LoopNetAPI.md#LoopnetGetBrokerProfile) | **Get** /v1/loopnet/brokers/{slug}/{broker_id} | Get broker profile
[**LoopnetGetListingDetail**](LoopNetAPI.md#LoopnetGetListingDetail) | **Get** /v1/loopnet/listings/{listing_id} | Get listing detail
[**LoopnetListCoverageMarkets**](LoopNetAPI.md#LoopnetListCoverageMarkets) | **Get** /v1/loopnet/markets | List coverage markets
[**LoopnetListPropertyTypes**](LoopNetAPI.md#LoopnetListPropertyTypes) | **Get** /v1/loopnet/property-types | List property types
[**LoopnetLoopnetScraperHealthCheck**](LoopNetAPI.md#LoopnetLoopnetScraperHealthCheck) | **Get** /v1/loopnet/health | LoopNet scraper health check
[**LoopnetLoopnetScraperHealthCheckHead**](LoopNetAPI.md#LoopnetLoopnetScraperHealthCheckHead) | **Head** /v1/loopnet/health | LoopNet scraper health check
[**LoopnetSearchCommercialRealEstate**](LoopNetAPI.md#LoopnetSearchCommercialRealEstate) | **Get** /v1/loopnet/search | Search commercial real estate



## LoopnetGetBrokerProfile

> interface{} LoopnetGetBrokerProfile(ctx, slug, brokerId).Market(market).Execute()

Get broker profile



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
	slug := "slug_example" // string | 
	brokerId := "brokerId_example" // string | 
	market := "market_example" // string | us|ca|uk|fr|es (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LoopNetAPI.LoopnetGetBrokerProfile(context.Background(), slug, brokerId).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LoopNetAPI.LoopnetGetBrokerProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LoopnetGetBrokerProfile`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LoopNetAPI.LoopnetGetBrokerProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** |  | 
**brokerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiLoopnetGetBrokerProfileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **market** | **string** | us|ca|uk|fr|es | [default to &quot;us&quot;]

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


## LoopnetGetListingDetail

> interface{} LoopnetGetListingDetail(ctx, listingId).Market(market).Execute()

Get listing detail



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
	listingId := "listingId_example" // string | 
	market := "market_example" // string | us|ca|uk|fr|es (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LoopNetAPI.LoopnetGetListingDetail(context.Background(), listingId).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LoopNetAPI.LoopnetGetListingDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LoopnetGetListingDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LoopNetAPI.LoopnetGetListingDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listingId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiLoopnetGetListingDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | us|ca|uk|fr|es | [default to &quot;us&quot;]

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


## LoopnetListCoverageMarkets

> interface{} LoopnetListCoverageMarkets(ctx).Execute()

List coverage markets



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
	resp, r, err := apiClient.LoopNetAPI.LoopnetListCoverageMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LoopNetAPI.LoopnetListCoverageMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LoopnetListCoverageMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LoopNetAPI.LoopnetListCoverageMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiLoopnetListCoverageMarketsRequest struct via the builder pattern


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


## LoopnetListPropertyTypes

> interface{} LoopnetListPropertyTypes(ctx).Execute()

List property types



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
	resp, r, err := apiClient.LoopNetAPI.LoopnetListPropertyTypes(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LoopNetAPI.LoopnetListPropertyTypes``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LoopnetListPropertyTypes`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LoopNetAPI.LoopnetListPropertyTypes`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiLoopnetListPropertyTypesRequest struct via the builder pattern


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


## LoopnetLoopnetScraperHealthCheck

> interface{} LoopnetLoopnetScraperHealthCheck(ctx).Execute()

LoopNet scraper health check



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
	resp, r, err := apiClient.LoopNetAPI.LoopnetLoopnetScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LoopNetAPI.LoopnetLoopnetScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LoopnetLoopnetScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LoopNetAPI.LoopnetLoopnetScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiLoopnetLoopnetScraperHealthCheckRequest struct via the builder pattern


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


## LoopnetLoopnetScraperHealthCheckHead

> interface{} LoopnetLoopnetScraperHealthCheckHead(ctx).Execute()

LoopNet scraper health check



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
	resp, r, err := apiClient.LoopNetAPI.LoopnetLoopnetScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LoopNetAPI.LoopnetLoopnetScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LoopnetLoopnetScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LoopNetAPI.LoopnetLoopnetScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiLoopnetLoopnetScraperHealthCheckHeadRequest struct via the builder pattern


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


## LoopnetSearchCommercialRealEstate

> interface{} LoopnetSearchCommercialRealEstate(ctx).Location(location).Market(market).ListingType(listingType).PropertyType(propertyType).Page(page).MinPrice(minPrice).MaxPrice(maxPrice).PriceType(priceType).MinSize(minSize).MaxSize(maxSize).Execute()

Search commercial real estate



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
	location := "location_example" // string | City/state, ZIP, state code, or 'usa'
	market := "market_example" // string | us|ca|uk|fr|es (optional) (default to "us")
	listingType := "listingType_example" // string | for-lease|for-sale|auctions (optional) (default to "for-lease")
	propertyType := "propertyType_example" // string | Slug from /property-types (optional)
	page := int32(56) // int32 |  (optional) (default to 1)
	minPrice := int32(56) // int32 |  (optional)
	maxPrice := int32(56) // int32 |  (optional)
	priceType := "priceType_example" // string | unit | sf | acre (optional)
	minSize := int32(56) // int32 |  (optional)
	maxSize := int32(56) // int32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LoopNetAPI.LoopnetSearchCommercialRealEstate(context.Background()).Location(location).Market(market).ListingType(listingType).PropertyType(propertyType).Page(page).MinPrice(minPrice).MaxPrice(maxPrice).PriceType(priceType).MinSize(minSize).MaxSize(maxSize).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LoopNetAPI.LoopnetSearchCommercialRealEstate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LoopnetSearchCommercialRealEstate`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LoopNetAPI.LoopnetSearchCommercialRealEstate`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiLoopnetSearchCommercialRealEstateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **location** | **string** | City/state, ZIP, state code, or &#39;usa&#39; | 
 **market** | **string** | us|ca|uk|fr|es | [default to &quot;us&quot;]
 **listingType** | **string** | for-lease|for-sale|auctions | [default to &quot;for-lease&quot;]
 **propertyType** | **string** | Slug from /property-types | 
 **page** | **int32** |  | [default to 1]
 **minPrice** | **int32** |  | 
 **maxPrice** | **int32** |  | 
 **priceType** | **string** | unit | sf | acre | 
 **minSize** | **int32** |  | 
 **maxSize** | **int32** |  | 

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


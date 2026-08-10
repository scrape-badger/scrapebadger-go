# \IdealistaAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**IdealistaAgencyByPhone**](IdealistaAPI.md#IdealistaAgencyByPhone) | **Get** /v1/idealista/agency/by-phone/{phone} | Agency by phone
[**IdealistaAgencyProfileListings**](IdealistaAPI.md#IdealistaAgencyProfileListings) | **Get** /v1/idealista/agency/{short_name} | Agency profile + listings
[**IdealistaGetListingEngagementStats**](IdealistaAPI.md#IdealistaGetListingEngagementStats) | **Get** /v1/idealista/properties/{property_code}/stats | Get listing engagement stats
[**IdealistaGetPropertyDetail**](IdealistaAPI.md#IdealistaGetPropertyDetail) | **Get** /v1/idealista/properties/{property_code} | Get property detail
[**IdealistaIdealistaScraperHealthCheck**](IdealistaAPI.md#IdealistaIdealistaScraperHealthCheck) | **Get** /v1/idealista/health | Idealista scraper health check
[**IdealistaIdealistaScraperHealthCheckHead**](IdealistaAPI.md#IdealistaIdealistaScraperHealthCheckHead) | **Head** /v1/idealista/health | Idealista scraper health check
[**IdealistaListMarkets**](IdealistaAPI.md#IdealistaListMarkets) | **Get** /v1/idealista/markets | List markets
[**IdealistaResolveLocations**](IdealistaAPI.md#IdealistaResolveLocations) | **Get** /v1/idealista/suggest | Resolve locations
[**IdealistaSearchAllBeatsResultCap**](IdealistaAPI.md#IdealistaSearchAllBeatsResultCap) | **Get** /v1/idealista/search/all | Search all (beats result cap)
[**IdealistaSearchListings**](IdealistaAPI.md#IdealistaSearchListings) | **Get** /v1/idealista/search | Search listings



## IdealistaAgencyByPhone

> interface{} IdealistaAgencyByPhone(ctx, phone).Market(market).Operation(operation).PropertyType(propertyType).Page(page).MaxItems(maxItems).IncludeListings(includeListings).Execute()

Agency by phone



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
	phone := "phone_example" // string | 
	market := "market_example" // string | es|it|pt (optional) (default to "es")
	operation := "operation_example" // string | sale|rent (optional)
	propertyType := "propertyType_example" // string | homes|offices|premises|garages|newDevelopments|lands|storageRooms|buildings|bedrooms (optional)
	page := int32(56) // int32 |  (optional) (default to 1)
	maxItems := int32(56) // int32 |  (optional) (default to 30)
	includeListings := true // bool |  (optional) (default to true)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IdealistaAPI.IdealistaAgencyByPhone(context.Background(), phone).Market(market).Operation(operation).PropertyType(propertyType).Page(page).MaxItems(maxItems).IncludeListings(includeListings).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IdealistaAPI.IdealistaAgencyByPhone``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `IdealistaAgencyByPhone`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `IdealistaAPI.IdealistaAgencyByPhone`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**phone** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiIdealistaAgencyByPhoneRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | es|it|pt | [default to &quot;es&quot;]
 **operation** | **string** | sale|rent | 
 **propertyType** | **string** | homes|offices|premises|garages|newDevelopments|lands|storageRooms|buildings|bedrooms | 
 **page** | **int32** |  | [default to 1]
 **maxItems** | **int32** |  | [default to 30]
 **includeListings** | **bool** |  | [default to true]

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


## IdealistaAgencyProfileListings

> interface{} IdealistaAgencyProfileListings(ctx, shortName).Market(market).Operation(operation).PropertyType(propertyType).Page(page).MaxItems(maxItems).IncludeListings(includeListings).Execute()

Agency profile + listings



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
	shortName := "shortName_example" // string | 
	market := "market_example" // string | es|it|pt (optional) (default to "es")
	operation := "operation_example" // string | sale|rent (optional)
	propertyType := "propertyType_example" // string | homes|offices|premises|garages|newDevelopments|lands|storageRooms|buildings|bedrooms (optional)
	page := int32(56) // int32 |  (optional) (default to 1)
	maxItems := int32(56) // int32 |  (optional) (default to 30)
	includeListings := true // bool |  (optional) (default to true)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IdealistaAPI.IdealistaAgencyProfileListings(context.Background(), shortName).Market(market).Operation(operation).PropertyType(propertyType).Page(page).MaxItems(maxItems).IncludeListings(includeListings).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IdealistaAPI.IdealistaAgencyProfileListings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `IdealistaAgencyProfileListings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `IdealistaAPI.IdealistaAgencyProfileListings`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shortName** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiIdealistaAgencyProfileListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | es|it|pt | [default to &quot;es&quot;]
 **operation** | **string** | sale|rent | 
 **propertyType** | **string** | homes|offices|premises|garages|newDevelopments|lands|storageRooms|buildings|bedrooms | 
 **page** | **int32** |  | [default to 1]
 **maxItems** | **int32** |  | [default to 30]
 **includeListings** | **bool** |  | [default to true]

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


## IdealistaGetListingEngagementStats

> interface{} IdealistaGetListingEngagementStats(ctx, propertyCode).Market(market).Locale(locale).Execute()

Get listing engagement stats



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
	propertyCode := "propertyCode_example" // string | 
	market := "market_example" // string | es|it|pt (optional) (default to "es")
	locale := "locale_example" // string | Language for stat labels (optional) (default to "en")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IdealistaAPI.IdealistaGetListingEngagementStats(context.Background(), propertyCode).Market(market).Locale(locale).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IdealistaAPI.IdealistaGetListingEngagementStats``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `IdealistaGetListingEngagementStats`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `IdealistaAPI.IdealistaGetListingEngagementStats`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**propertyCode** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiIdealistaGetListingEngagementStatsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | es|it|pt | [default to &quot;es&quot;]
 **locale** | **string** | Language for stat labels | [default to &quot;en&quot;]

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


## IdealistaGetPropertyDetail

> interface{} IdealistaGetPropertyDetail(ctx, propertyCode).Market(market).Locale(locale).Execute()

Get property detail



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
	propertyCode := "propertyCode_example" // string | 
	market := "market_example" // string | es|it|pt (optional) (default to "es")
	locale := "locale_example" // string | Response language (en, es, it, pt) (optional) (default to "en")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IdealistaAPI.IdealistaGetPropertyDetail(context.Background(), propertyCode).Market(market).Locale(locale).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IdealistaAPI.IdealistaGetPropertyDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `IdealistaGetPropertyDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `IdealistaAPI.IdealistaGetPropertyDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**propertyCode** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiIdealistaGetPropertyDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | es|it|pt | [default to &quot;es&quot;]
 **locale** | **string** | Response language (en, es, it, pt) | [default to &quot;en&quot;]

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


## IdealistaIdealistaScraperHealthCheck

> interface{} IdealistaIdealistaScraperHealthCheck(ctx).Execute()

Idealista scraper health check



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
	resp, r, err := apiClient.IdealistaAPI.IdealistaIdealistaScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IdealistaAPI.IdealistaIdealistaScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `IdealistaIdealistaScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `IdealistaAPI.IdealistaIdealistaScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiIdealistaIdealistaScraperHealthCheckRequest struct via the builder pattern


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


## IdealistaIdealistaScraperHealthCheckHead

> interface{} IdealistaIdealistaScraperHealthCheckHead(ctx).Execute()

Idealista scraper health check



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
	resp, r, err := apiClient.IdealistaAPI.IdealistaIdealistaScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IdealistaAPI.IdealistaIdealistaScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `IdealistaIdealistaScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `IdealistaAPI.IdealistaIdealistaScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiIdealistaIdealistaScraperHealthCheckHeadRequest struct via the builder pattern


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


## IdealistaListMarkets

> interface{} IdealistaListMarkets(ctx).Execute()

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
	resp, r, err := apiClient.IdealistaAPI.IdealistaListMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IdealistaAPI.IdealistaListMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `IdealistaListMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `IdealistaAPI.IdealistaListMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiIdealistaListMarketsRequest struct via the builder pattern


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


## IdealistaResolveLocations

> interface{} IdealistaResolveLocations(ctx).Query(query).Operation(operation).PropertyType(propertyType).Market(market).Locale(locale).Execute()

Resolve locations



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
	query := "query_example" // string | Free-text location, e.g. 'sagrada familia'
	operation := "operation_example" // string | sale|rent (optional) (default to "sale")
	propertyType := "propertyType_example" // string | homes|offices|premises|garages|newDevelopments|lands|storageRooms|buildings|bedrooms (optional) (default to "homes")
	market := "market_example" // string | es|it|pt (optional) (default to "es")
	locale := "locale_example" // string | Response language (en, es, it, pt) (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IdealistaAPI.IdealistaResolveLocations(context.Background()).Query(query).Operation(operation).PropertyType(propertyType).Market(market).Locale(locale).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IdealistaAPI.IdealistaResolveLocations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `IdealistaResolveLocations`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `IdealistaAPI.IdealistaResolveLocations`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiIdealistaResolveLocationsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Free-text location, e.g. &#39;sagrada familia&#39; | 
 **operation** | **string** | sale|rent | [default to &quot;sale&quot;]
 **propertyType** | **string** | homes|offices|premises|garages|newDevelopments|lands|storageRooms|buildings|bedrooms | [default to &quot;homes&quot;]
 **market** | **string** | es|it|pt | [default to &quot;es&quot;]
 **locale** | **string** | Response language (en, es, it, pt) | 

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


## IdealistaSearchAllBeatsResultCap

> interface{} IdealistaSearchAllBeatsResultCap(ctx).Location(location).Operation(operation).PropertyType(propertyType).Market(market).MaxResults(maxResults).MinPrice(minPrice).MaxPrice(maxPrice).MinSize(minSize).MaxSize(maxSize).MinRooms(minRooms).MaxRooms(maxRooms).Locale(locale).Execute()

Search all (beats result cap)



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
	location := "location_example" // string | Idealista location code (from /suggest)
	operation := "operation_example" // string | sale|rent (optional) (default to "sale")
	propertyType := "propertyType_example" // string | homes|offices|premises|garages|newDevelopments|lands|storageRooms|buildings|bedrooms (optional) (default to "homes")
	market := "market_example" // string | es|it|pt (optional) (default to "es")
	maxResults := int32(56) // int32 |  (optional) (default to 500)
	minPrice := float32(8.14) // float32 |  (optional)
	maxPrice := float32(8.14) // float32 |  (optional)
	minSize := float32(8.14) // float32 |  (optional)
	maxSize := float32(8.14) // float32 |  (optional)
	minRooms := int32(56) // int32 |  (optional)
	maxRooms := int32(56) // int32 |  (optional)
	locale := "locale_example" // string | Response language (en, es, it, pt) (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IdealistaAPI.IdealistaSearchAllBeatsResultCap(context.Background()).Location(location).Operation(operation).PropertyType(propertyType).Market(market).MaxResults(maxResults).MinPrice(minPrice).MaxPrice(maxPrice).MinSize(minSize).MaxSize(maxSize).MinRooms(minRooms).MaxRooms(maxRooms).Locale(locale).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IdealistaAPI.IdealistaSearchAllBeatsResultCap``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `IdealistaSearchAllBeatsResultCap`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `IdealistaAPI.IdealistaSearchAllBeatsResultCap`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiIdealistaSearchAllBeatsResultCapRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **location** | **string** | Idealista location code (from /suggest) | 
 **operation** | **string** | sale|rent | [default to &quot;sale&quot;]
 **propertyType** | **string** | homes|offices|premises|garages|newDevelopments|lands|storageRooms|buildings|bedrooms | [default to &quot;homes&quot;]
 **market** | **string** | es|it|pt | [default to &quot;es&quot;]
 **maxResults** | **int32** |  | [default to 500]
 **minPrice** | **float32** |  | 
 **maxPrice** | **float32** |  | 
 **minSize** | **float32** |  | 
 **maxSize** | **float32** |  | 
 **minRooms** | **int32** |  | 
 **maxRooms** | **int32** |  | 
 **locale** | **string** | Response language (en, es, it, pt) | 

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


## IdealistaSearchListings

> interface{} IdealistaSearchListings(ctx).Location(location).Operation(operation).PropertyType(propertyType).Market(market).Page(page).MaxItems(maxItems).SortBy(sortBy).SortOrder(sortOrder).MinPrice(minPrice).MaxPrice(maxPrice).MinSize(minSize).MaxSize(maxSize).MinRooms(minRooms).MaxRooms(maxRooms).Locale(locale).Execute()

Search listings



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
	location := "location_example" // string | Idealista location code (from /suggest)
	operation := "operation_example" // string | sale|rent (optional) (default to "sale")
	propertyType := "propertyType_example" // string | homes|offices|premises|garages|newDevelopments|lands|storageRooms|buildings|bedrooms (optional) (default to "homes")
	market := "market_example" // string | es|it|pt (optional) (default to "es")
	page := int32(56) // int32 |  (optional) (default to 1)
	maxItems := int32(56) // int32 |  (optional) (default to 30)
	sortBy := "sortBy_example" // string | distance|size|rooms|floor|ratioeurm2|price|street|photos|modificationDate|publicationDate|weigh|priceDown|preservationTypeAndPrice|privateAds (optional)
	sortOrder := "sortOrder_example" // string | asc|desc (optional) (default to "desc")
	minPrice := float32(8.14) // float32 |  (optional)
	maxPrice := float32(8.14) // float32 |  (optional)
	minSize := float32(8.14) // float32 |  (optional)
	maxSize := float32(8.14) // float32 |  (optional)
	minRooms := int32(56) // int32 |  (optional)
	maxRooms := int32(56) // int32 |  (optional)
	locale := "locale_example" // string | Response language (en, es, it, pt) (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IdealistaAPI.IdealistaSearchListings(context.Background()).Location(location).Operation(operation).PropertyType(propertyType).Market(market).Page(page).MaxItems(maxItems).SortBy(sortBy).SortOrder(sortOrder).MinPrice(minPrice).MaxPrice(maxPrice).MinSize(minSize).MaxSize(maxSize).MinRooms(minRooms).MaxRooms(maxRooms).Locale(locale).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IdealistaAPI.IdealistaSearchListings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `IdealistaSearchListings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `IdealistaAPI.IdealistaSearchListings`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiIdealistaSearchListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **location** | **string** | Idealista location code (from /suggest) | 
 **operation** | **string** | sale|rent | [default to &quot;sale&quot;]
 **propertyType** | **string** | homes|offices|premises|garages|newDevelopments|lands|storageRooms|buildings|bedrooms | [default to &quot;homes&quot;]
 **market** | **string** | es|it|pt | [default to &quot;es&quot;]
 **page** | **int32** |  | [default to 1]
 **maxItems** | **int32** |  | [default to 30]
 **sortBy** | **string** | distance|size|rooms|floor|ratioeurm2|price|street|photos|modificationDate|publicationDate|weigh|priceDown|preservationTypeAndPrice|privateAds | 
 **sortOrder** | **string** | asc|desc | [default to &quot;desc&quot;]
 **minPrice** | **float32** |  | 
 **maxPrice** | **float32** |  | 
 **minSize** | **float32** |  | 
 **maxSize** | **float32** |  | 
 **minRooms** | **int32** |  | 
 **maxRooms** | **int32** |  | 
 **locale** | **string** | Response language (en, es, it, pt) | 

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


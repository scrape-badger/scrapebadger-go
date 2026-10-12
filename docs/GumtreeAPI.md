# \GumtreeAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GumtreeGetListing**](GumtreeAPI.md#GumtreeGetListing) | **Get** /v1/gumtree/listings/{listing_id} | Get listing
[**GumtreeGetSearchFilters**](GumtreeAPI.md#GumtreeGetSearchFilters) | **Get** /v1/gumtree/search/filters | Get search filters
[**GumtreeGetSellerListings**](GumtreeAPI.md#GumtreeGetSellerListings) | **Get** /v1/gumtree/listings/{listing_id}/seller-listings | Get seller listings
[**GumtreeGumtreeScraperHealthCheck**](GumtreeAPI.md#GumtreeGumtreeScraperHealthCheck) | **Get** /v1/gumtree/health | Gumtree scraper health check
[**GumtreeGumtreeScraperHealthCheckHead**](GumtreeAPI.md#GumtreeGumtreeScraperHealthCheckHead) | **Head** /v1/gumtree/health | Gumtree scraper health check
[**GumtreeListCategories**](GumtreeAPI.md#GumtreeListCategories) | **Get** /v1/gumtree/categories | List categories
[**GumtreeListLocations**](GumtreeAPI.md#GumtreeListLocations) | **Get** /v1/gumtree/locations | List locations
[**GumtreeListMarkets**](GumtreeAPI.md#GumtreeListMarkets) | **Get** /v1/gumtree/markets | List markets
[**GumtreeLocationSuggestions**](GumtreeAPI.md#GumtreeLocationSuggestions) | **Get** /v1/gumtree/locations/autocomplete | Location suggestions
[**GumtreeSearchListings**](GumtreeAPI.md#GumtreeSearchListings) | **Get** /v1/gumtree/search | Search listings
[**GumtreeSearchSuggestions**](GumtreeAPI.md#GumtreeSearchSuggestions) | **Get** /v1/gumtree/autocomplete | Search suggestions



## GumtreeGetListing

> interface{} GumtreeGetListing(ctx, listingId).Market(market).Execute()

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
	listingId := "listingId_example" // string | Gumtree listing id — the number at the end of the listing URL (uk/au: ~10 digits; za: the full 26-digit ad id, not the short one)
	market := "market_example" // string | Which Gumtree: 'uk' (gumtree.com, GBP), 'au' (gumtree.com.au, AUD) or 'za' (gumtree.co.za, ZAR). Separate sites — ids from one market mean nothing in another. (optional) (default to "uk")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GumtreeAPI.GumtreeGetListing(context.Background(), listingId).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GumtreeAPI.GumtreeGetListing``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GumtreeGetListing`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GumtreeAPI.GumtreeGetListing`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listingId** | **string** | Gumtree listing id — the number at the end of the listing URL (uk/au: ~10 digits; za: the full 26-digit ad id, not the short one) | 

### Other Parameters

Other parameters are passed through a pointer to a apiGumtreeGetListingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | Which Gumtree: &#39;uk&#39; (gumtree.com, GBP), &#39;au&#39; (gumtree.com.au, AUD) or &#39;za&#39; (gumtree.co.za, ZAR). Separate sites — ids from one market mean nothing in another. | [default to &quot;uk&quot;]

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


## GumtreeGetSearchFilters

> interface{} GumtreeGetSearchFilters(ctx).Category(category).Location(location).Query(query).Filters(filters).Market(market).Execute()

Get search filters



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
	category := "category_example" // string | uk: category slug, e.g. 'cars', 'for-sale', 'property-to-rent', 'jobs', 'bicycles'. au/za: numeric category id, e.g. '18320' (au cars) or '9077' (za cars). Use /categories to browse the tree. Default 'all'. (optional) (default to "all")
	location := "location_example" // string | uk: location slug ('london'), town name or UK postcode ('SW1A 1AA'). au/za: numeric location id, e.g. '3003435' (au Sydney) or '3100003' (za Gauteng). Use /locations/autocomplete to resolve one. Default: the whole country. (optional)
	query := "query_example" // string | Optional keywords to scope the counts (optional)
	filters := "filters_example" // string | za only: filters already applied (e.g. 'ma:toyota' to list Toyota models) (optional)
	market := "market_example" // string | Which Gumtree: 'uk' (gumtree.com, GBP), 'au' (gumtree.com.au, AUD) or 'za' (gumtree.co.za, ZAR). Separate sites — ids from one market mean nothing in another. (optional) (default to "uk")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GumtreeAPI.GumtreeGetSearchFilters(context.Background()).Category(category).Location(location).Query(query).Filters(filters).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GumtreeAPI.GumtreeGetSearchFilters``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GumtreeGetSearchFilters`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GumtreeAPI.GumtreeGetSearchFilters`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGumtreeGetSearchFiltersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **category** | **string** | uk: category slug, e.g. &#39;cars&#39;, &#39;for-sale&#39;, &#39;property-to-rent&#39;, &#39;jobs&#39;, &#39;bicycles&#39;. au/za: numeric category id, e.g. &#39;18320&#39; (au cars) or &#39;9077&#39; (za cars). Use /categories to browse the tree. Default &#39;all&#39;. | [default to &quot;all&quot;]
 **location** | **string** | uk: location slug (&#39;london&#39;), town name or UK postcode (&#39;SW1A 1AA&#39;). au/za: numeric location id, e.g. &#39;3003435&#39; (au Sydney) or &#39;3100003&#39; (za Gauteng). Use /locations/autocomplete to resolve one. Default: the whole country. | 
 **query** | **string** | Optional keywords to scope the counts | 
 **filters** | **string** | za only: filters already applied (e.g. &#39;ma:toyota&#39; to list Toyota models) | 
 **market** | **string** | Which Gumtree: &#39;uk&#39; (gumtree.com, GBP), &#39;au&#39; (gumtree.com.au, AUD) or &#39;za&#39; (gumtree.co.za, ZAR). Separate sites — ids from one market mean nothing in another. | [default to &quot;uk&quot;]

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


## GumtreeGetSellerListings

> interface{} GumtreeGetSellerListings(ctx, listingId).Page(page).Market(market).Execute()

Get seller listings



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
	listingId := "listingId_example" // string | Gumtree listing id — the number at the end of the listing URL (uk/au: ~10 digits; za: the full 26-digit ad id, not the short one)
	page := int32(56) // int32 |  (optional) (default to 1)
	market := "market_example" // string | Which Gumtree: 'uk' (gumtree.com, GBP), 'au' (gumtree.com.au, AUD) or 'za' (gumtree.co.za, ZAR). Separate sites — ids from one market mean nothing in another. (optional) (default to "uk")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GumtreeAPI.GumtreeGetSellerListings(context.Background(), listingId).Page(page).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GumtreeAPI.GumtreeGetSellerListings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GumtreeGetSellerListings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GumtreeAPI.GumtreeGetSellerListings`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listingId** | **string** | Gumtree listing id — the number at the end of the listing URL (uk/au: ~10 digits; za: the full 26-digit ad id, not the short one) | 

### Other Parameters

Other parameters are passed through a pointer to a apiGumtreeGetSellerListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** |  | [default to 1]
 **market** | **string** | Which Gumtree: &#39;uk&#39; (gumtree.com, GBP), &#39;au&#39; (gumtree.com.au, AUD) or &#39;za&#39; (gumtree.co.za, ZAR). Separate sites — ids from one market mean nothing in another. | [default to &quot;uk&quot;]

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


## GumtreeGumtreeScraperHealthCheck

> interface{} GumtreeGumtreeScraperHealthCheck(ctx).Execute()

Gumtree scraper health check



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
	resp, r, err := apiClient.GumtreeAPI.GumtreeGumtreeScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GumtreeAPI.GumtreeGumtreeScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GumtreeGumtreeScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GumtreeAPI.GumtreeGumtreeScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGumtreeGumtreeScraperHealthCheckRequest struct via the builder pattern


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


## GumtreeGumtreeScraperHealthCheckHead

> interface{} GumtreeGumtreeScraperHealthCheckHead(ctx).Execute()

Gumtree scraper health check



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
	resp, r, err := apiClient.GumtreeAPI.GumtreeGumtreeScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GumtreeAPI.GumtreeGumtreeScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GumtreeGumtreeScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GumtreeAPI.GumtreeGumtreeScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGumtreeGumtreeScraperHealthCheckHeadRequest struct via the builder pattern


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


## GumtreeListCategories

> interface{} GumtreeListCategories(ctx).ParentId(parentId).Market(market).Execute()

List categories



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
	parentId := int32(56) // int32 | Category id to list the children of (default: all) (optional)
	market := "market_example" // string | Which Gumtree: 'uk' (gumtree.com, GBP), 'au' (gumtree.com.au, AUD) or 'za' (gumtree.co.za, ZAR). Separate sites — ids from one market mean nothing in another. (optional) (default to "uk")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GumtreeAPI.GumtreeListCategories(context.Background()).ParentId(parentId).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GumtreeAPI.GumtreeListCategories``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GumtreeListCategories`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GumtreeAPI.GumtreeListCategories`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGumtreeListCategoriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **parentId** | **int32** | Category id to list the children of (default: all) | 
 **market** | **string** | Which Gumtree: &#39;uk&#39; (gumtree.com, GBP), &#39;au&#39; (gumtree.com.au, AUD) or &#39;za&#39; (gumtree.co.za, ZAR). Separate sites — ids from one market mean nothing in another. | [default to &quot;uk&quot;]

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


## GumtreeListLocations

> interface{} GumtreeListLocations(ctx).ParentId(parentId).Market(market).Execute()

List locations



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
	parentId := int32(56) // int32 | Location id to list the children of (default: the whole country) (optional)
	market := "market_example" // string | Which Gumtree: 'uk' (gumtree.com, GBP), 'au' (gumtree.com.au, AUD) or 'za' (gumtree.co.za, ZAR). Separate sites — ids from one market mean nothing in another. (optional) (default to "uk")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GumtreeAPI.GumtreeListLocations(context.Background()).ParentId(parentId).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GumtreeAPI.GumtreeListLocations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GumtreeListLocations`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GumtreeAPI.GumtreeListLocations`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGumtreeListLocationsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **parentId** | **int32** | Location id to list the children of (default: the whole country) | 
 **market** | **string** | Which Gumtree: &#39;uk&#39; (gumtree.com, GBP), &#39;au&#39; (gumtree.com.au, AUD) or &#39;za&#39; (gumtree.co.za, ZAR). Separate sites — ids from one market mean nothing in another. | [default to &quot;uk&quot;]

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


## GumtreeListMarkets

> interface{} GumtreeListMarkets(ctx).Execute()

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
	resp, r, err := apiClient.GumtreeAPI.GumtreeListMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GumtreeAPI.GumtreeListMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GumtreeListMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GumtreeAPI.GumtreeListMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGumtreeListMarketsRequest struct via the builder pattern


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


## GumtreeLocationSuggestions

> interface{} GumtreeLocationSuggestions(ctx).Query(query).Market(market).Execute()

Location suggestions



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
	query := "query_example" // string | Town, area or postcode prefix, e.g. 'manch' or 'SW1A'
	market := "market_example" // string | Which Gumtree: 'uk' (gumtree.com, GBP), 'au' (gumtree.com.au, AUD) or 'za' (gumtree.co.za, ZAR). Separate sites — ids from one market mean nothing in another. (optional) (default to "uk")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GumtreeAPI.GumtreeLocationSuggestions(context.Background()).Query(query).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GumtreeAPI.GumtreeLocationSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GumtreeLocationSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GumtreeAPI.GumtreeLocationSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGumtreeLocationSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Town, area or postcode prefix, e.g. &#39;manch&#39; or &#39;SW1A&#39; | 
 **market** | **string** | Which Gumtree: &#39;uk&#39; (gumtree.com, GBP), &#39;au&#39; (gumtree.com.au, AUD) or &#39;za&#39; (gumtree.co.za, ZAR). Separate sites — ids from one market mean nothing in another. | [default to &quot;uk&quot;]

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


## GumtreeSearchListings

> interface{} GumtreeSearchListings(ctx).Query(query).Category(category).Location(location).Distance(distance).MinPrice(minPrice).MaxPrice(maxPrice).Sort(sort).SellerType(sellerType).UrgentOnly(urgentOnly).WithPhotos(withPhotos).Filters(filters).Page(page).Market(market).Execute()

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
	query := "query_example" // string | Search keywords, e.g. 'mountain bike' (optional)
	category := "category_example" // string | uk: category slug, e.g. 'cars', 'for-sale', 'property-to-rent', 'jobs', 'bicycles'. au/za: numeric category id, e.g. '18320' (au cars) or '9077' (za cars). Use /categories to browse the tree. Default 'all'. (optional) (default to "all")
	location := "location_example" // string | uk: location slug ('london'), town name or UK postcode ('SW1A 1AA'). au/za: numeric location id, e.g. '3003435' (au Sydney) or '3100003' (za Gauteng). Use /locations/autocomplete to resolve one. Default: the whole country. (optional)
	distance := float32(8.14) // float32 | Radius around `location`: miles (uk) or km (au). Not offered by za. (optional)
	minPrice := int32(56) // int32 | Minimum price in the market's currency (uk: needs a category, not 'all') (optional)
	maxPrice := int32(56) // int32 | Maximum price in the market's currency (uk: needs a category, not 'all') (optional)
	sort := "sort_example" // string | Result ordering (default relevance). 'distance' needs uk, or au with a location. (optional)
	sellerType := "sellerType_example" // string | uk/za: 'trade' covers dealers, agencies and recruiters. au: not supported — use a category filter such as 'cars.forsaleby_s:ownr'. (optional)
	urgentOnly := true // bool | uk only: only ads marked urgent (optional) (default to false)
	withPhotos := true // bool | uk only: only ads with photos (optional) (default to false)
	filters := "filters_example" // string | Category-specific filters as comma-separated key:value pairs, e.g. 'vehicle_make:bmw,vehicle_fuel_type:petrol,min_vehicle_mileage:10000' (uk), 'cars.carmake_s:toyota,cars.forsaleby_s:ownr' (au) or 'ma:toyota,fu:petrol,max_km:100000' (za). Range filters take min_<key>/max_<key>. Discover keys and values with /search/filters for the same market. (optional)
	page := int32(56) // int32 |  (optional) (default to 1)
	market := "market_example" // string | Which Gumtree: 'uk' (gumtree.com, GBP), 'au' (gumtree.com.au, AUD) or 'za' (gumtree.co.za, ZAR). Separate sites — ids from one market mean nothing in another. (optional) (default to "uk")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GumtreeAPI.GumtreeSearchListings(context.Background()).Query(query).Category(category).Location(location).Distance(distance).MinPrice(minPrice).MaxPrice(maxPrice).Sort(sort).SellerType(sellerType).UrgentOnly(urgentOnly).WithPhotos(withPhotos).Filters(filters).Page(page).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GumtreeAPI.GumtreeSearchListings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GumtreeSearchListings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GumtreeAPI.GumtreeSearchListings`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGumtreeSearchListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords, e.g. &#39;mountain bike&#39; | 
 **category** | **string** | uk: category slug, e.g. &#39;cars&#39;, &#39;for-sale&#39;, &#39;property-to-rent&#39;, &#39;jobs&#39;, &#39;bicycles&#39;. au/za: numeric category id, e.g. &#39;18320&#39; (au cars) or &#39;9077&#39; (za cars). Use /categories to browse the tree. Default &#39;all&#39;. | [default to &quot;all&quot;]
 **location** | **string** | uk: location slug (&#39;london&#39;), town name or UK postcode (&#39;SW1A 1AA&#39;). au/za: numeric location id, e.g. &#39;3003435&#39; (au Sydney) or &#39;3100003&#39; (za Gauteng). Use /locations/autocomplete to resolve one. Default: the whole country. | 
 **distance** | **float32** | Radius around &#x60;location&#x60;: miles (uk) or km (au). Not offered by za. | 
 **minPrice** | **int32** | Minimum price in the market&#39;s currency (uk: needs a category, not &#39;all&#39;) | 
 **maxPrice** | **int32** | Maximum price in the market&#39;s currency (uk: needs a category, not &#39;all&#39;) | 
 **sort** | **string** | Result ordering (default relevance). &#39;distance&#39; needs uk, or au with a location. | 
 **sellerType** | **string** | uk/za: &#39;trade&#39; covers dealers, agencies and recruiters. au: not supported — use a category filter such as &#39;cars.forsaleby_s:ownr&#39;. | 
 **urgentOnly** | **bool** | uk only: only ads marked urgent | [default to false]
 **withPhotos** | **bool** | uk only: only ads with photos | [default to false]
 **filters** | **string** | Category-specific filters as comma-separated key:value pairs, e.g. &#39;vehicle_make:bmw,vehicle_fuel_type:petrol,min_vehicle_mileage:10000&#39; (uk), &#39;cars.carmake_s:toyota,cars.forsaleby_s:ownr&#39; (au) or &#39;ma:toyota,fu:petrol,max_km:100000&#39; (za). Range filters take min_&lt;key&gt;/max_&lt;key&gt;. Discover keys and values with /search/filters for the same market. | 
 **page** | **int32** |  | [default to 1]
 **market** | **string** | Which Gumtree: &#39;uk&#39; (gumtree.com, GBP), &#39;au&#39; (gumtree.com.au, AUD) or &#39;za&#39; (gumtree.co.za, ZAR). Separate sites — ids from one market mean nothing in another. | [default to &quot;uk&quot;]

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


## GumtreeSearchSuggestions

> interface{} GumtreeSearchSuggestions(ctx).Query(query).Market(market).Execute()

Search suggestions



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
	query := "query_example" // string | Partial search term, e.g. 'iph'
	market := "market_example" // string | Which Gumtree: 'uk' (gumtree.com, GBP), 'au' (gumtree.com.au, AUD) or 'za' (gumtree.co.za, ZAR). Separate sites — ids from one market mean nothing in another. (optional) (default to "uk")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GumtreeAPI.GumtreeSearchSuggestions(context.Background()).Query(query).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GumtreeAPI.GumtreeSearchSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GumtreeSearchSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GumtreeAPI.GumtreeSearchSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGumtreeSearchSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Partial search term, e.g. &#39;iph&#39; | 
 **market** | **string** | Which Gumtree: &#39;uk&#39; (gumtree.com, GBP), &#39;au&#39; (gumtree.com.au, AUD) or &#39;za&#39; (gumtree.co.za, ZAR). Separate sites — ids from one market mean nothing in another. | [default to &quot;uk&quot;]

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


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
[**GumtreeLocationSuggestions**](GumtreeAPI.md#GumtreeLocationSuggestions) | **Get** /v1/gumtree/locations/autocomplete | Location suggestions
[**GumtreeSearchListings**](GumtreeAPI.md#GumtreeSearchListings) | **Get** /v1/gumtree/search | Search listings
[**GumtreeSearchSuggestions**](GumtreeAPI.md#GumtreeSearchSuggestions) | **Get** /v1/gumtree/autocomplete | Search suggestions



## GumtreeGetListing

> interface{} GumtreeGetListing(ctx, listingId).Execute()

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
	listingId := "listingId_example" // string | Gumtree listing id — the number at the end of a gumtree.com/p/... URL

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GumtreeAPI.GumtreeGetListing(context.Background(), listingId).Execute()
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
**listingId** | **string** | Gumtree listing id — the number at the end of a gumtree.com/p/... URL | 

### Other Parameters

Other parameters are passed through a pointer to a apiGumtreeGetListingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


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

> interface{} GumtreeGetSearchFilters(ctx).Category(category).Location(location).Query(query).Execute()

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
	category := "category_example" // string | Category slug, e.g. 'cars', 'for-sale', 'property-to-rent', 'jobs'. Default 'all'. (optional) (default to "all")
	location := "location_example" // string | Location slug ('london'), town name or UK postcode ('SW1A 1AA'). Default 'uk'. (optional) (default to "uk")
	query := "query_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GumtreeAPI.GumtreeGetSearchFilters(context.Background()).Category(category).Location(location).Query(query).Execute()
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
 **category** | **string** | Category slug, e.g. &#39;cars&#39;, &#39;for-sale&#39;, &#39;property-to-rent&#39;, &#39;jobs&#39;. Default &#39;all&#39;. | [default to &quot;all&quot;]
 **location** | **string** | Location slug (&#39;london&#39;), town name or UK postcode (&#39;SW1A 1AA&#39;). Default &#39;uk&#39;. | [default to &quot;uk&quot;]
 **query** | **string** |  | 

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

> interface{} GumtreeGetSellerListings(ctx, listingId).Page(page).Execute()

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
	listingId := "listingId_example" // string | Gumtree listing id — the number at the end of a gumtree.com/p/... URL
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GumtreeAPI.GumtreeGetSellerListings(context.Background(), listingId).Page(page).Execute()
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
**listingId** | **string** | Gumtree listing id — the number at the end of a gumtree.com/p/... URL | 

### Other Parameters

Other parameters are passed through a pointer to a apiGumtreeGetSellerListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** |  | [default to 1]

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

> interface{} GumtreeListCategories(ctx).ParentId(parentId).Execute()

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
	parentId := int32(56) // int32 | Parent category id (default: all) (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GumtreeAPI.GumtreeListCategories(context.Background()).ParentId(parentId).Execute()
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
 **parentId** | **int32** | Parent category id (default: all) | [default to 1]

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

> interface{} GumtreeListLocations(ctx).ParentId(parentId).Execute()

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
	parentId := int32(56) // int32 | Parent location id (default: UK) (optional) (default to 10000392)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GumtreeAPI.GumtreeListLocations(context.Background()).ParentId(parentId).Execute()
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
 **parentId** | **int32** | Parent location id (default: UK) | [default to 10000392]

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

> interface{} GumtreeLocationSuggestions(ctx).Query(query).Execute()

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
	query := "query_example" // string | Town or postcode prefix, e.g. 'manch'

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GumtreeAPI.GumtreeLocationSuggestions(context.Background()).Query(query).Execute()
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
 **query** | **string** | Town or postcode prefix, e.g. &#39;manch&#39; | 

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

> interface{} GumtreeSearchListings(ctx).Query(query).Category(category).Location(location).Distance(distance).MinPrice(minPrice).MaxPrice(maxPrice).Sort(sort).SellerType(sellerType).UrgentOnly(urgentOnly).WithPhotos(withPhotos).Filters(filters).Page(page).Execute()

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
	category := "category_example" // string | Category slug, e.g. 'cars', 'for-sale', 'property-to-rent', 'jobs'. Default 'all'. (optional) (default to "all")
	location := "location_example" // string | Location slug ('london'), town name or UK postcode ('SW1A 1AA'). Default 'uk'. (optional) (default to "uk")
	distance := float32(8.14) // float32 | Radius in miles (optional)
	minPrice := int32(56) // int32 | GBP; needs a category (optional)
	maxPrice := int32(56) // int32 | GBP; needs a category (optional)
	sort := "sort_example" // string |  (optional)
	sellerType := "sellerType_example" // string |  (optional)
	urgentOnly := true // bool |  (optional) (default to false)
	withPhotos := true // bool |  (optional) (default to false)
	filters := "filters_example" // string | Category filters as key:value pairs, e.g. 'vehicle_make:bmw,vehicle_fuel_type:petrol' (optional)
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GumtreeAPI.GumtreeSearchListings(context.Background()).Query(query).Category(category).Location(location).Distance(distance).MinPrice(minPrice).MaxPrice(maxPrice).Sort(sort).SellerType(sellerType).UrgentOnly(urgentOnly).WithPhotos(withPhotos).Filters(filters).Page(page).Execute()
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
 **category** | **string** | Category slug, e.g. &#39;cars&#39;, &#39;for-sale&#39;, &#39;property-to-rent&#39;, &#39;jobs&#39;. Default &#39;all&#39;. | [default to &quot;all&quot;]
 **location** | **string** | Location slug (&#39;london&#39;), town name or UK postcode (&#39;SW1A 1AA&#39;). Default &#39;uk&#39;. | [default to &quot;uk&quot;]
 **distance** | **float32** | Radius in miles | 
 **minPrice** | **int32** | GBP; needs a category | 
 **maxPrice** | **int32** | GBP; needs a category | 
 **sort** | **string** |  | 
 **sellerType** | **string** |  | 
 **urgentOnly** | **bool** |  | [default to false]
 **withPhotos** | **bool** |  | [default to false]
 **filters** | **string** | Category filters as key:value pairs, e.g. &#39;vehicle_make:bmw,vehicle_fuel_type:petrol&#39; | 
 **page** | **int32** |  | [default to 1]

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

> interface{} GumtreeSearchSuggestions(ctx).Query(query).Execute()

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GumtreeAPI.GumtreeSearchSuggestions(context.Background()).Query(query).Execute()
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


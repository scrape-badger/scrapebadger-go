# \WalmartAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**WalmartBrowseACategory**](WalmartAPI.md#WalmartBrowseACategory) | **Get** /v1/walmart/category | Browse a category
[**WalmartDealsRollbacksAndClearance**](WalmartAPI.md#WalmartDealsRollbacksAndClearance) | **Get** /v1/walmart/deals | Deals, rollbacks and clearance
[**WalmartGetASellerSCatalogue**](WalmartAPI.md#WalmartGetASellerSCatalogue) | **Get** /v1/walmart/sellers/{seller_id}/products | Get a seller&#39;s catalogue
[**WalmartGetProductDetail**](WalmartAPI.md#WalmartGetProductDetail) | **Get** /v1/walmart/products/{item_id} | Get product detail
[**WalmartGetProductReviews**](WalmartAPI.md#WalmartGetProductReviews) | **Get** /v1/walmart/products/{item_id}/reviews | Get product reviews
[**WalmartGetSellerProfile**](WalmartAPI.md#WalmartGetSellerProfile) | **Get** /v1/walmart/sellers/{seller_id} | Get seller profile
[**WalmartGetStoreNearbyStores**](WalmartAPI.md#WalmartGetStoreNearbyStores) | **Get** /v1/walmart/stores/{store_id} | Get store + nearby stores
[**WalmartListSupportedMarkets**](WalmartAPI.md#WalmartListSupportedMarkets) | **Get** /v1/walmart/markets | List supported markets
[**WalmartSearchProducts**](WalmartAPI.md#WalmartSearchProducts) | **Get** /v1/walmart/search | Search products
[**WalmartSearchSuggestions**](WalmartAPI.md#WalmartSearchSuggestions) | **Get** /v1/walmart/autocomplete | Search suggestions
[**WalmartWalmartScraperHealthCheck**](WalmartAPI.md#WalmartWalmartScraperHealthCheck) | **Get** /v1/walmart/health | Walmart scraper health check
[**WalmartWalmartScraperHealthCheckHead**](WalmartAPI.md#WalmartWalmartScraperHealthCheckHead) | **Head** /v1/walmart/health | Walmart scraper health check



## WalmartBrowseACategory

> interface{} WalmartBrowseACategory(ctx).Path(path).Page(page).MinPrice(minPrice).MaxPrice(maxPrice).Facet(facet).Execute()

Browse a category



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
	path := "path_example" // string | Browse path, e.g. 'electronics/3944', or a '/cp/...' path
	page := int32(56) // int32 |  (optional) (default to 1)
	minPrice := float32(8.14) // float32 |  (optional)
	maxPrice := float32(8.14) // float32 |  (optional)
	facet := "facet_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalmartAPI.WalmartBrowseACategory(context.Background()).Path(path).Page(page).MinPrice(minPrice).MaxPrice(maxPrice).Facet(facet).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalmartAPI.WalmartBrowseACategory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalmartBrowseACategory`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WalmartAPI.WalmartBrowseACategory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWalmartBrowseACategoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **path** | **string** | Browse path, e.g. &#39;electronics/3944&#39;, or a &#39;/cp/...&#39; path | 
 **page** | **int32** |  | [default to 1]
 **minPrice** | **float32** |  | 
 **maxPrice** | **float32** |  | 
 **facet** | **string** |  | 

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


## WalmartDealsRollbacksAndClearance

> interface{} WalmartDealsRollbacksAndClearance(ctx).Page(page).MinPrice(minPrice).MaxPrice(maxPrice).Execute()

Deals, rollbacks and clearance



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
	page := int32(56) // int32 |  (optional) (default to 1)
	minPrice := float32(8.14) // float32 |  (optional)
	maxPrice := float32(8.14) // float32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalmartAPI.WalmartDealsRollbacksAndClearance(context.Background()).Page(page).MinPrice(minPrice).MaxPrice(maxPrice).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalmartAPI.WalmartDealsRollbacksAndClearance``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalmartDealsRollbacksAndClearance`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WalmartAPI.WalmartDealsRollbacksAndClearance`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWalmartDealsRollbacksAndClearanceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int32** |  | [default to 1]
 **minPrice** | **float32** |  | 
 **maxPrice** | **float32** |  | 

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


## WalmartGetASellerSCatalogue

> interface{} WalmartGetASellerSCatalogue(ctx, sellerId).Query(query).Page(page).Sort(sort).Execute()

Get a seller's catalogue



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
	sellerId := "sellerId_example" // string | Numeric catalog seller id, e.g. '101040442' — the `catalog_seller_id` on a product, NOT the 32-char hex `seller_id` (which 404s).
	query := "query_example" // string | Required — Walmart returns nothing for a seller facet alone
	page := int32(56) // int32 |  (optional) (default to 1)
	sort := "sort_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalmartAPI.WalmartGetASellerSCatalogue(context.Background(), sellerId).Query(query).Page(page).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalmartAPI.WalmartGetASellerSCatalogue``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalmartGetASellerSCatalogue`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WalmartAPI.WalmartGetASellerSCatalogue`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sellerId** | **string** | Numeric catalog seller id, e.g. &#39;101040442&#39; — the &#x60;catalog_seller_id&#x60; on a product, NOT the 32-char hex &#x60;seller_id&#x60; (which 404s). | 

### Other Parameters

Other parameters are passed through a pointer to a apiWalmartGetASellerSCatalogueRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **query** | **string** | Required — Walmart returns nothing for a seller facet alone | 
 **page** | **int32** |  | [default to 1]
 **sort** | **string** |  | 

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


## WalmartGetProductDetail

> interface{} WalmartGetProductDetail(ctx, itemId).Execute()

Get product detail



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
	itemId := "itemId_example" // string | Walmart usItemId, e.g. '5689919121'

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalmartAPI.WalmartGetProductDetail(context.Background(), itemId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalmartAPI.WalmartGetProductDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalmartGetProductDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WalmartAPI.WalmartGetProductDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**itemId** | **string** | Walmart usItemId, e.g. &#39;5689919121&#39; | 

### Other Parameters

Other parameters are passed through a pointer to a apiWalmartGetProductDetailRequest struct via the builder pattern


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


## WalmartGetProductReviews

> interface{} WalmartGetProductReviews(ctx, itemId).Page(page).Sort(sort).Execute()

Get product reviews



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
	itemId := "itemId_example" // string | Walmart usItemId, e.g. '5689919121'
	page := int32(56) // int32 |  (optional) (default to 1)
	sort := "sort_example" // string | relevancy | submission-desc | submission-asc | rating-desc | rating-asc | helpful (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalmartAPI.WalmartGetProductReviews(context.Background(), itemId).Page(page).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalmartAPI.WalmartGetProductReviews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalmartGetProductReviews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WalmartAPI.WalmartGetProductReviews`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**itemId** | **string** | Walmart usItemId, e.g. &#39;5689919121&#39; | 

### Other Parameters

Other parameters are passed through a pointer to a apiWalmartGetProductReviewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** |  | [default to 1]
 **sort** | **string** | relevancy | submission-desc | submission-asc | rating-desc | rating-asc | helpful | 

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


## WalmartGetSellerProfile

> interface{} WalmartGetSellerProfile(ctx, sellerId).Execute()

Get seller profile



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
	sellerId := "sellerId_example" // string | Numeric catalog seller id, e.g. '101040442' — the `catalog_seller_id` on a product, NOT the 32-char hex `seller_id` (which 404s).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalmartAPI.WalmartGetSellerProfile(context.Background(), sellerId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalmartAPI.WalmartGetSellerProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalmartGetSellerProfile`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WalmartAPI.WalmartGetSellerProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sellerId** | **string** | Numeric catalog seller id, e.g. &#39;101040442&#39; — the &#x60;catalog_seller_id&#x60; on a product, NOT the 32-char hex &#x60;seller_id&#x60; (which 404s). | 

### Other Parameters

Other parameters are passed through a pointer to a apiWalmartGetSellerProfileRequest struct via the builder pattern


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


## WalmartGetStoreNearbyStores

> interface{} WalmartGetStoreNearbyStores(ctx, storeId).Execute()

Get store + nearby stores



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
	storeId := "storeId_example" // string | Walmart store number, e.g. '100'

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalmartAPI.WalmartGetStoreNearbyStores(context.Background(), storeId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalmartAPI.WalmartGetStoreNearbyStores``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalmartGetStoreNearbyStores`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WalmartAPI.WalmartGetStoreNearbyStores`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**storeId** | **string** | Walmart store number, e.g. &#39;100&#39; | 

### Other Parameters

Other parameters are passed through a pointer to a apiWalmartGetStoreNearbyStoresRequest struct via the builder pattern


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


## WalmartListSupportedMarkets

> interface{} WalmartListSupportedMarkets(ctx).Execute()

List supported markets



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
	resp, r, err := apiClient.WalmartAPI.WalmartListSupportedMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalmartAPI.WalmartListSupportedMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalmartListSupportedMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WalmartAPI.WalmartListSupportedMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiWalmartListSupportedMarketsRequest struct via the builder pattern


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


## WalmartSearchProducts

> interface{} WalmartSearchProducts(ctx).Query(query).Page(page).Sort(sort).MinPrice(minPrice).MaxPrice(maxPrice).Facet(facet).Execute()

Search products



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
	query := "query_example" // string | Search keywords, e.g. 'laptop'
	page := int32(56) // int32 | Results dry up after page 10 (optional) (default to 1)
	sort := "sort_example" // string | best_match | best_seller | price_low | price_high | rating_high | new (optional)
	minPrice := float32(8.14) // float32 |  (optional)
	maxPrice := float32(8.14) // float32 |  (optional)
	facet := "facet_example" // string | Facet filter, e.g. 'brand:HP' (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalmartAPI.WalmartSearchProducts(context.Background()).Query(query).Page(page).Sort(sort).MinPrice(minPrice).MaxPrice(maxPrice).Facet(facet).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalmartAPI.WalmartSearchProducts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalmartSearchProducts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WalmartAPI.WalmartSearchProducts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWalmartSearchProductsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords, e.g. &#39;laptop&#39; | 
 **page** | **int32** | Results dry up after page 10 | [default to 1]
 **sort** | **string** | best_match | best_seller | price_low | price_high | rating_high | new | 
 **minPrice** | **float32** |  | 
 **maxPrice** | **float32** |  | 
 **facet** | **string** | Facet filter, e.g. &#39;brand:HP&#39; | 

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


## WalmartSearchSuggestions

> interface{} WalmartSearchSuggestions(ctx).Query(query).Execute()

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
	query := "query_example" // string | Partial search term, e.g. 'lapt'

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WalmartAPI.WalmartSearchSuggestions(context.Background()).Query(query).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalmartAPI.WalmartSearchSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalmartSearchSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WalmartAPI.WalmartSearchSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWalmartSearchSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Partial search term, e.g. &#39;lapt&#39; | 

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


## WalmartWalmartScraperHealthCheck

> interface{} WalmartWalmartScraperHealthCheck(ctx).Execute()

Walmart scraper health check



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
	resp, r, err := apiClient.WalmartAPI.WalmartWalmartScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalmartAPI.WalmartWalmartScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalmartWalmartScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WalmartAPI.WalmartWalmartScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiWalmartWalmartScraperHealthCheckRequest struct via the builder pattern


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


## WalmartWalmartScraperHealthCheckHead

> interface{} WalmartWalmartScraperHealthCheckHead(ctx).Execute()

Walmart scraper health check



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
	resp, r, err := apiClient.WalmartAPI.WalmartWalmartScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WalmartAPI.WalmartWalmartScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WalmartWalmartScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WalmartAPI.WalmartWalmartScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiWalmartWalmartScraperHealthCheckHeadRequest struct via the builder pattern


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


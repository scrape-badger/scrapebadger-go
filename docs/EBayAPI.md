# \EBayAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**EbayBrowseACategory**](EBayAPI.md#EbayBrowseACategory) | **Get** /v1/ebay/categories/{category_id}/items | Browse a category
[**EbayCompletedSoldListings**](EBayAPI.md#EbayCompletedSoldListings) | **Get** /v1/ebay/completed | Completed / sold listings
[**EbayEbayScraperHealthCheck**](EBayAPI.md#EbayEbayScraperHealthCheck) | **Get** /v1/ebay/health | eBay scraper health check
[**EbayEbayScraperHealthCheckHead**](EBayAPI.md#EbayEbayScraperHealthCheckHead) | **Head** /v1/ebay/health | eBay scraper health check
[**EbayGetItemDetail**](EBayAPI.md#EbayGetItemDetail) | **Get** /v1/ebay/items/{item_id} | Get item detail
[**EbayGetItemReviews**](EBayAPI.md#EbayGetItemReviews) | **Get** /v1/ebay/items/{item_id}/reviews | Get item reviews
[**EbayGetSellerFeedback**](EBayAPI.md#EbayGetSellerFeedback) | **Get** /v1/ebay/sellers/{username}/feedback | Get seller feedback
[**EbayGetSellerListings**](EBayAPI.md#EbayGetSellerListings) | **Get** /v1/ebay/sellers/{username}/items | Get seller listings
[**EbayGetSellerProfile**](EBayAPI.md#EbayGetSellerProfile) | **Get** /v1/ebay/sellers/{username} | Get seller profile
[**EbayKeywordSuggestions**](EBayAPI.md#EbayKeywordSuggestions) | **Get** /v1/ebay/autocomplete | Keyword suggestions
[**EbayListCategories**](EBayAPI.md#EbayListCategories) | **Get** /v1/ebay/categories | List categories
[**EbayListMarkets**](EBayAPI.md#EbayListMarkets) | **Get** /v1/ebay/markets | List markets
[**EbaySearchByImage**](EBayAPI.md#EbaySearchByImage) | **Post** /v1/ebay/search/by-image | Search by image
[**EbaySearchListings**](EBayAPI.md#EbaySearchListings) | **Get** /v1/ebay/search | Search listings



## EbayBrowseACategory

> interface{} EbayBrowseACategory(ctx, categoryId).Domain(domain).Page(page).PerPage(perPage).SortBy(sortBy).MinPrice(minPrice).MaxPrice(maxPrice).Execute()

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
	categoryId := "categoryId_example" // string | 
	domain := "domain_example" // string |  (optional) (default to "com")
	page := int32(56) // int32 |  (optional) (default to 1)
	perPage := int32(56) // int32 |  (optional)
	sortBy := "sortBy_example" // string | best_match|ending_soonest|newly_listed|price_low_to_high|price_high_to_low (optional) (default to "best_match")
	minPrice := float32(8.14) // float32 |  (optional)
	maxPrice := float32(8.14) // float32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EBayAPI.EbayBrowseACategory(context.Background(), categoryId).Domain(domain).Page(page).PerPage(perPage).SortBy(sortBy).MinPrice(minPrice).MaxPrice(maxPrice).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EBayAPI.EbayBrowseACategory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EbayBrowseACategory`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EBayAPI.EbayBrowseACategory`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**categoryId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiEbayBrowseACategoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **domain** | **string** |  | [default to &quot;com&quot;]
 **page** | **int32** |  | [default to 1]
 **perPage** | **int32** |  | 
 **sortBy** | **string** | best_match|ending_soonest|newly_listed|price_low_to_high|price_high_to_low | [default to &quot;best_match&quot;]
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


## EbayCompletedSoldListings

> interface{} EbayCompletedSoldListings(ctx).Query(query).Domain(domain).CategoryId(categoryId).Page(page).PerPage(perPage).SortBy(sortBy).Condition(condition).MinPrice(minPrice).MaxPrice(maxPrice).Location(location).Language(language).Execute()

Completed / sold listings



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
	query := "query_example" // string | Search keywords
	domain := "domain_example" // string | Marketplace domain (com, co.uk, de …) (optional) (default to "com")
	categoryId := "categoryId_example" // string | Restrict to a category id (optional)
	page := int32(56) // int32 |  (optional) (default to 1)
	perPage := int32(56) // int32 | 60, 120 or 240 (optional)
	sortBy := "sortBy_example" // string | best_match|ending_soonest|newly_listed|price_low_to_high|price_high_to_low (optional) (default to "best_match")
	condition := "condition_example" // string | new|open_box|refurbished|used|for_parts|graded|ungraded (optional)
	minPrice := float32(8.14) // float32 |  (optional)
	maxPrice := float32(8.14) // float32 |  (optional)
	location := "location_example" // string | domestic|worldwide (optional)
	language := "language_example" // string | english|japanese|chinese|korean (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EBayAPI.EbayCompletedSoldListings(context.Background()).Query(query).Domain(domain).CategoryId(categoryId).Page(page).PerPage(perPage).SortBy(sortBy).Condition(condition).MinPrice(minPrice).MaxPrice(maxPrice).Location(location).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EBayAPI.EbayCompletedSoldListings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EbayCompletedSoldListings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EBayAPI.EbayCompletedSoldListings`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiEbayCompletedSoldListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords | 
 **domain** | **string** | Marketplace domain (com, co.uk, de …) | [default to &quot;com&quot;]
 **categoryId** | **string** | Restrict to a category id | 
 **page** | **int32** |  | [default to 1]
 **perPage** | **int32** | 60, 120 or 240 | 
 **sortBy** | **string** | best_match|ending_soonest|newly_listed|price_low_to_high|price_high_to_low | [default to &quot;best_match&quot;]
 **condition** | **string** | new|open_box|refurbished|used|for_parts|graded|ungraded | 
 **minPrice** | **float32** |  | 
 **maxPrice** | **float32** |  | 
 **location** | **string** | domestic|worldwide | 
 **language** | **string** | english|japanese|chinese|korean | 

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


## EbayEbayScraperHealthCheck

> interface{} EbayEbayScraperHealthCheck(ctx).Execute()

eBay scraper health check



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
	resp, r, err := apiClient.EBayAPI.EbayEbayScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EBayAPI.EbayEbayScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EbayEbayScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EBayAPI.EbayEbayScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiEbayEbayScraperHealthCheckRequest struct via the builder pattern


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


## EbayEbayScraperHealthCheckHead

> interface{} EbayEbayScraperHealthCheckHead(ctx).Execute()

eBay scraper health check



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
	resp, r, err := apiClient.EBayAPI.EbayEbayScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EBayAPI.EbayEbayScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EbayEbayScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EBayAPI.EbayEbayScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiEbayEbayScraperHealthCheckHeadRequest struct via the builder pattern


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


## EbayGetItemDetail

> interface{} EbayGetItemDetail(ctx, itemId).Domain(domain).Execute()

Get item detail



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
	itemId := "itemId_example" // string | 
	domain := "domain_example" // string |  (optional) (default to "com")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EBayAPI.EbayGetItemDetail(context.Background(), itemId).Domain(domain).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EBayAPI.EbayGetItemDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EbayGetItemDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EBayAPI.EbayGetItemDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**itemId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiEbayGetItemDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **domain** | **string** |  | [default to &quot;com&quot;]

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


## EbayGetItemReviews

> interface{} EbayGetItemReviews(ctx, itemId).Domain(domain).Page(page).Execute()

Get item reviews



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
	itemId := "itemId_example" // string | 
	domain := "domain_example" // string |  (optional) (default to "com")
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EBayAPI.EbayGetItemReviews(context.Background(), itemId).Domain(domain).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EBayAPI.EbayGetItemReviews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EbayGetItemReviews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EBayAPI.EbayGetItemReviews`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**itemId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiEbayGetItemReviewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **domain** | **string** |  | [default to &quot;com&quot;]
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


## EbayGetSellerFeedback

> interface{} EbayGetSellerFeedback(ctx, username).Domain(domain).Page(page).Execute()

Get seller feedback



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
	username := "username_example" // string | 
	domain := "domain_example" // string |  (optional) (default to "com")
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EBayAPI.EbayGetSellerFeedback(context.Background(), username).Domain(domain).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EBayAPI.EbayGetSellerFeedback``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EbayGetSellerFeedback`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EBayAPI.EbayGetSellerFeedback`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiEbayGetSellerFeedbackRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **domain** | **string** |  | [default to &quot;com&quot;]
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


## EbayGetSellerListings

> interface{} EbayGetSellerListings(ctx, username).Domain(domain).Query(query).Page(page).PerPage(perPage).Execute()

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
	username := "username_example" // string | 
	domain := "domain_example" // string |  (optional) (default to "com")
	query := "query_example" // string |  (optional)
	page := int32(56) // int32 |  (optional) (default to 1)
	perPage := int32(56) // int32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EBayAPI.EbayGetSellerListings(context.Background(), username).Domain(domain).Query(query).Page(page).PerPage(perPage).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EBayAPI.EbayGetSellerListings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EbayGetSellerListings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EBayAPI.EbayGetSellerListings`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiEbayGetSellerListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **domain** | **string** |  | [default to &quot;com&quot;]
 **query** | **string** |  | 
 **page** | **int32** |  | [default to 1]
 **perPage** | **int32** |  | 

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


## EbayGetSellerProfile

> interface{} EbayGetSellerProfile(ctx, username).Domain(domain).Execute()

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
	username := "username_example" // string | 
	domain := "domain_example" // string |  (optional) (default to "com")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EBayAPI.EbayGetSellerProfile(context.Background(), username).Domain(domain).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EBayAPI.EbayGetSellerProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EbayGetSellerProfile`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EBayAPI.EbayGetSellerProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiEbayGetSellerProfileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **domain** | **string** |  | [default to &quot;com&quot;]

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


## EbayKeywordSuggestions

> interface{} EbayKeywordSuggestions(ctx).Query(query).Domain(domain).Execute()

Keyword suggestions



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
	query := "query_example" // string | Partial query prefix
	domain := "domain_example" // string |  (optional) (default to "com")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EBayAPI.EbayKeywordSuggestions(context.Background()).Query(query).Domain(domain).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EBayAPI.EbayKeywordSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EbayKeywordSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EBayAPI.EbayKeywordSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiEbayKeywordSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Partial query prefix | 
 **domain** | **string** |  | [default to &quot;com&quot;]

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


## EbayListCategories

> interface{} EbayListCategories(ctx).Execute()

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EBayAPI.EbayListCategories(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EBayAPI.EbayListCategories``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EbayListCategories`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EBayAPI.EbayListCategories`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiEbayListCategoriesRequest struct via the builder pattern


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


## EbayListMarkets

> interface{} EbayListMarkets(ctx).Execute()

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
	resp, r, err := apiClient.EBayAPI.EbayListMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EBayAPI.EbayListMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EbayListMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EBayAPI.EbayListMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiEbayListMarketsRequest struct via the builder pattern


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


## EbaySearchByImage

> interface{} EbaySearchByImage(ctx).RequestBody(requestBody).Execute()

Search by image



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
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EBayAPI.EbaySearchByImage(context.Background()).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EBayAPI.EbaySearchByImage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EbaySearchByImage`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EBayAPI.EbaySearchByImage`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiEbaySearchByImageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **requestBody** | **map[string]interface{}** |  | 

### Return type

**interface{}**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## EbaySearchListings

> interface{} EbaySearchListings(ctx).Query(query).Domain(domain).CategoryId(categoryId).Page(page).PerPage(perPage).SortBy(sortBy).Condition(condition).BuyingFormat(buyingFormat).MinPrice(minPrice).MaxPrice(maxPrice).FreeShipping(freeShipping).Location(location).Language(language).Execute()

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
	query := "query_example" // string | Search keywords
	domain := "domain_example" // string | Marketplace domain (com, co.uk, de …) (optional) (default to "com")
	categoryId := "categoryId_example" // string | Restrict to a category id (optional)
	page := int32(56) // int32 |  (optional) (default to 1)
	perPage := int32(56) // int32 | 60, 120 or 240 (optional)
	sortBy := "sortBy_example" // string | best_match|ending_soonest|newly_listed|price_low_to_high|price_high_to_low (optional) (default to "best_match")
	condition := "condition_example" // string | new|open_box|refurbished|used|for_parts|graded|ungraded (optional)
	buyingFormat := "buyingFormat_example" // string | auction|buy_it_now|best_offer (optional)
	minPrice := float32(8.14) // float32 |  (optional)
	maxPrice := float32(8.14) // float32 |  (optional)
	freeShipping := true // bool |  (optional) (default to false)
	location := "location_example" // string | domestic|worldwide (optional)
	language := "language_example" // string | english|japanese|chinese|korean (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EBayAPI.EbaySearchListings(context.Background()).Query(query).Domain(domain).CategoryId(categoryId).Page(page).PerPage(perPage).SortBy(sortBy).Condition(condition).BuyingFormat(buyingFormat).MinPrice(minPrice).MaxPrice(maxPrice).FreeShipping(freeShipping).Location(location).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EBayAPI.EbaySearchListings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EbaySearchListings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EBayAPI.EbaySearchListings`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiEbaySearchListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords | 
 **domain** | **string** | Marketplace domain (com, co.uk, de …) | [default to &quot;com&quot;]
 **categoryId** | **string** | Restrict to a category id | 
 **page** | **int32** |  | [default to 1]
 **perPage** | **int32** | 60, 120 or 240 | 
 **sortBy** | **string** | best_match|ending_soonest|newly_listed|price_low_to_high|price_high_to_low | [default to &quot;best_match&quot;]
 **condition** | **string** | new|open_box|refurbished|used|for_parts|graded|ungraded | 
 **buyingFormat** | **string** | auction|buy_it_now|best_offer | 
 **minPrice** | **float32** |  | 
 **maxPrice** | **float32** |  | 
 **freeShipping** | **bool** |  | [default to false]
 **location** | **string** | domestic|worldwide | 
 **language** | **string** | english|japanese|chinese|korean | 

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


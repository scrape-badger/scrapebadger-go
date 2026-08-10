# \AmazonAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AmazonAmazonScraperHealthCheck**](AmazonAPI.md#AmazonAmazonScraperHealthCheck) | **Get** /v1/amazon/health | Amazon scraper health check
[**AmazonAmazonScraperHealthCheckHead**](AmazonAPI.md#AmazonAmazonScraperHealthCheckHead) | **Head** /v1/amazon/health | Amazon scraper health check
[**AmazonBestsellersByCategory**](AmazonAPI.md#AmazonBestsellersByCategory) | **Get** /v1/amazon/bestsellers | Bestsellers by category
[**AmazonBrowseNodeCategoryListing**](AmazonAPI.md#AmazonBrowseNodeCategoryListing) | **Get** /v1/amazon/category | Browse-node category listing
[**AmazonGetAllSellerOffersBuybox**](AmazonAPI.md#AmazonGetAllSellerOffersBuybox) | **Get** /v1/amazon/products/{asin}/offers | Get all seller offers (buybox)
[**AmazonGetProductDetail**](AmazonAPI.md#AmazonGetProductDetail) | **Get** /v1/amazon/products/{asin} | Get product detail
[**AmazonGetProductReviews**](AmazonAPI.md#AmazonGetProductReviews) | **Get** /v1/amazon/products/{asin}/reviews | Get product reviews
[**AmazonGetSellerFeedback**](AmazonAPI.md#AmazonGetSellerFeedback) | **Get** /v1/amazon/sellers/{seller_id}/feedback | Get seller feedback
[**AmazonGetSellerProfile**](AmazonAPI.md#AmazonGetSellerProfile) | **Get** /v1/amazon/sellers/{seller_id} | Get seller profile
[**AmazonGetSellerStorefrontProducts**](AmazonAPI.md#AmazonGetSellerStorefrontProducts) | **Get** /v1/amazon/sellers/{seller_id}/products | Get seller storefront products
[**AmazonKeywordSuggestions**](AmazonAPI.md#AmazonKeywordSuggestions) | **Get** /v1/amazon/autocomplete | Keyword suggestions
[**AmazonListCategoryAliases**](AmazonAPI.md#AmazonListCategoryAliases) | **Get** /v1/amazon/categories | List category aliases
[**AmazonListMarketplaces**](AmazonAPI.md#AmazonListMarketplaces) | **Get** /v1/amazon/markets | List marketplaces
[**AmazonNewReleasesByCategory**](AmazonAPI.md#AmazonNewReleasesByCategory) | **Get** /v1/amazon/new-releases | New releases by category
[**AmazonSearchAmazonProducts**](AmazonAPI.md#AmazonSearchAmazonProducts) | **Get** /v1/amazon/search | Search Amazon products
[**AmazonTodaySDeals**](AmazonAPI.md#AmazonTodaySDeals) | **Get** /v1/amazon/deals | Today&#39;s deals



## AmazonAmazonScraperHealthCheck

> interface{} AmazonAmazonScraperHealthCheck(ctx).Execute()

Amazon scraper health check



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
	resp, r, err := apiClient.AmazonAPI.AmazonAmazonScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AmazonAPI.AmazonAmazonScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AmazonAmazonScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AmazonAPI.AmazonAmazonScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAmazonAmazonScraperHealthCheckRequest struct via the builder pattern


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


## AmazonAmazonScraperHealthCheckHead

> interface{} AmazonAmazonScraperHealthCheckHead(ctx).Execute()

Amazon scraper health check



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
	resp, r, err := apiClient.AmazonAPI.AmazonAmazonScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AmazonAPI.AmazonAmazonScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AmazonAmazonScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AmazonAPI.AmazonAmazonScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAmazonAmazonScraperHealthCheckHeadRequest struct via the builder pattern


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


## AmazonBestsellersByCategory

> interface{} AmazonBestsellersByCategory(ctx).Domain(domain).Category(category).Page(page).Execute()

Bestsellers by category



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
	domain := "domain_example" // string |  (optional) (default to "com")
	category := "category_example" // string | Bestsellers node id or slug (optional)
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AmazonAPI.AmazonBestsellersByCategory(context.Background()).Domain(domain).Category(category).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AmazonAPI.AmazonBestsellersByCategory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AmazonBestsellersByCategory`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AmazonAPI.AmazonBestsellersByCategory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAmazonBestsellersByCategoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domain** | **string** |  | [default to &quot;com&quot;]
 **category** | **string** | Bestsellers node id or slug | 
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


## AmazonBrowseNodeCategoryListing

> interface{} AmazonBrowseNodeCategoryListing(ctx).Node(node).Domain(domain).Page(page).SortBy(sortBy).Execute()

Browse-node category listing



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
	node := "node_example" // string | Amazon browse-node id
	domain := "domain_example" // string |  (optional) (default to "com")
	page := int32(56) // int32 |  (optional) (default to 1)
	sortBy := "sortBy_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AmazonAPI.AmazonBrowseNodeCategoryListing(context.Background()).Node(node).Domain(domain).Page(page).SortBy(sortBy).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AmazonAPI.AmazonBrowseNodeCategoryListing``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AmazonBrowseNodeCategoryListing`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AmazonAPI.AmazonBrowseNodeCategoryListing`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAmazonBrowseNodeCategoryListingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **node** | **string** | Amazon browse-node id | 
 **domain** | **string** |  | [default to &quot;com&quot;]
 **page** | **int32** |  | [default to 1]
 **sortBy** | **string** |  | 

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


## AmazonGetAllSellerOffersBuybox

> interface{} AmazonGetAllSellerOffersBuybox(ctx, asin).Domain(domain).Zip(zip).Execute()

Get all seller offers (buybox)



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
	asin := "asin_example" // string | 
	domain := "domain_example" // string |  (optional) (default to "com")
	zip := "zip_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AmazonAPI.AmazonGetAllSellerOffersBuybox(context.Background(), asin).Domain(domain).Zip(zip).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AmazonAPI.AmazonGetAllSellerOffersBuybox``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AmazonGetAllSellerOffersBuybox`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AmazonAPI.AmazonGetAllSellerOffersBuybox`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**asin** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAmazonGetAllSellerOffersBuyboxRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **domain** | **string** |  | [default to &quot;com&quot;]
 **zip** | **string** |  | 

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


## AmazonGetProductDetail

> interface{} AmazonGetProductDetail(ctx, asin).Domain(domain).Zip(zip).Language(language).Execute()

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
	asin := "asin_example" // string | 
	domain := "domain_example" // string |  (optional) (default to "com")
	zip := "zip_example" // string | Delivery postal/zip for localized buybox (optional)
	language := "language_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AmazonAPI.AmazonGetProductDetail(context.Background(), asin).Domain(domain).Zip(zip).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AmazonAPI.AmazonGetProductDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AmazonGetProductDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AmazonAPI.AmazonGetProductDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**asin** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAmazonGetProductDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **domain** | **string** |  | [default to &quot;com&quot;]
 **zip** | **string** | Delivery postal/zip for localized buybox | 
 **language** | **string** |  | 

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


## AmazonGetProductReviews

> interface{} AmazonGetProductReviews(ctx, asin).Domain(domain).Page(page).SortBy(sortBy).Star(star).VerifiedOnly(verifiedOnly).MediaOnly(mediaOnly).Execute()

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
	asin := "asin_example" // string | 
	domain := "domain_example" // string |  (optional) (default to "com")
	page := int32(56) // int32 | Review page (1-100, ~10 reviews/page) (optional) (default to 1)
	sortBy := "sortBy_example" // string | helpful | recent (optional) (default to "helpful")
	star := "star_example" // string | one_star..five_star | positive | critical (optional)
	verifiedOnly := true // bool |  (optional) (default to false)
	mediaOnly := true // bool |  (optional) (default to false)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AmazonAPI.AmazonGetProductReviews(context.Background(), asin).Domain(domain).Page(page).SortBy(sortBy).Star(star).VerifiedOnly(verifiedOnly).MediaOnly(mediaOnly).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AmazonAPI.AmazonGetProductReviews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AmazonGetProductReviews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AmazonAPI.AmazonGetProductReviews`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**asin** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAmazonGetProductReviewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **domain** | **string** |  | [default to &quot;com&quot;]
 **page** | **int32** | Review page (1-100, ~10 reviews/page) | [default to 1]
 **sortBy** | **string** | helpful | recent | [default to &quot;helpful&quot;]
 **star** | **string** | one_star..five_star | positive | critical | 
 **verifiedOnly** | **bool** |  | [default to false]
 **mediaOnly** | **bool** |  | [default to false]

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


## AmazonGetSellerFeedback

> interface{} AmazonGetSellerFeedback(ctx, sellerId).Domain(domain).Page(page).Execute()

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
	sellerId := "sellerId_example" // string | 
	domain := "domain_example" // string |  (optional) (default to "com")
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AmazonAPI.AmazonGetSellerFeedback(context.Background(), sellerId).Domain(domain).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AmazonAPI.AmazonGetSellerFeedback``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AmazonGetSellerFeedback`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AmazonAPI.AmazonGetSellerFeedback`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sellerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAmazonGetSellerFeedbackRequest struct via the builder pattern


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


## AmazonGetSellerProfile

> interface{} AmazonGetSellerProfile(ctx, sellerId).Domain(domain).Execute()

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
	sellerId := "sellerId_example" // string | 
	domain := "domain_example" // string |  (optional) (default to "com")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AmazonAPI.AmazonGetSellerProfile(context.Background(), sellerId).Domain(domain).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AmazonAPI.AmazonGetSellerProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AmazonGetSellerProfile`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AmazonAPI.AmazonGetSellerProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sellerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAmazonGetSellerProfileRequest struct via the builder pattern


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


## AmazonGetSellerStorefrontProducts

> interface{} AmazonGetSellerStorefrontProducts(ctx, sellerId).Domain(domain).Page(page).Execute()

Get seller storefront products



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
	sellerId := "sellerId_example" // string | 
	domain := "domain_example" // string |  (optional) (default to "com")
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AmazonAPI.AmazonGetSellerStorefrontProducts(context.Background(), sellerId).Domain(domain).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AmazonAPI.AmazonGetSellerStorefrontProducts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AmazonGetSellerStorefrontProducts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AmazonAPI.AmazonGetSellerStorefrontProducts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sellerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAmazonGetSellerStorefrontProductsRequest struct via the builder pattern


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


## AmazonKeywordSuggestions

> interface{} AmazonKeywordSuggestions(ctx).Query(query).Domain(domain).Execute()

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
	query := "query_example" // string | Partial search term
	domain := "domain_example" // string |  (optional) (default to "com")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AmazonAPI.AmazonKeywordSuggestions(context.Background()).Query(query).Domain(domain).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AmazonAPI.AmazonKeywordSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AmazonKeywordSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AmazonAPI.AmazonKeywordSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAmazonKeywordSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Partial search term | 
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


## AmazonListCategoryAliases

> interface{} AmazonListCategoryAliases(ctx).Domain(domain).Execute()

List category aliases



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
	domain := "domain_example" // string |  (optional) (default to "com")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AmazonAPI.AmazonListCategoryAliases(context.Background()).Domain(domain).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AmazonAPI.AmazonListCategoryAliases``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AmazonListCategoryAliases`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AmazonAPI.AmazonListCategoryAliases`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAmazonListCategoryAliasesRequest struct via the builder pattern


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


## AmazonListMarketplaces

> interface{} AmazonListMarketplaces(ctx).Execute()

List marketplaces



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
	resp, r, err := apiClient.AmazonAPI.AmazonListMarketplaces(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AmazonAPI.AmazonListMarketplaces``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AmazonListMarketplaces`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AmazonAPI.AmazonListMarketplaces`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAmazonListMarketplacesRequest struct via the builder pattern


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


## AmazonNewReleasesByCategory

> interface{} AmazonNewReleasesByCategory(ctx).Domain(domain).Category(category).Page(page).Execute()

New releases by category



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
	domain := "domain_example" // string |  (optional) (default to "com")
	category := "category_example" // string |  (optional)
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AmazonAPI.AmazonNewReleasesByCategory(context.Background()).Domain(domain).Category(category).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AmazonAPI.AmazonNewReleasesByCategory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AmazonNewReleasesByCategory`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AmazonAPI.AmazonNewReleasesByCategory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAmazonNewReleasesByCategoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domain** | **string** |  | [default to &quot;com&quot;]
 **category** | **string** |  | 
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


## AmazonSearchAmazonProducts

> interface{} AmazonSearchAmazonProducts(ctx).Query(query).Domain(domain).Page(page).SortBy(sortBy).Category(category).MinPrice(minPrice).MaxPrice(maxPrice).Zip(zip).Language(language).Execute()

Search Amazon products



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
	domain := "domain_example" // string | Amazon marketplace TLD or code (com, co.uk, de…) (optional) (default to "com")
	page := int32(56) // int32 |  (optional) (default to 1)
	sortBy := "sortBy_example" // string | relevance | price_low_to_high | price_high_to_low | avg_review | newest (optional)
	category := "category_example" // string | Department/category alias (i= param) (optional)
	minPrice := float32(8.14) // float32 |  (optional)
	maxPrice := float32(8.14) // float32 |  (optional)
	zip := "zip_example" // string | Delivery postal/zip code for localized pricing (optional)
	language := "language_example" // string | Locale for results, e.g. en_US, fr_FR (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AmazonAPI.AmazonSearchAmazonProducts(context.Background()).Query(query).Domain(domain).Page(page).SortBy(sortBy).Category(category).MinPrice(minPrice).MaxPrice(maxPrice).Zip(zip).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AmazonAPI.AmazonSearchAmazonProducts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AmazonSearchAmazonProducts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AmazonAPI.AmazonSearchAmazonProducts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAmazonSearchAmazonProductsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords | 
 **domain** | **string** | Amazon marketplace TLD or code (com, co.uk, de…) | [default to &quot;com&quot;]
 **page** | **int32** |  | [default to 1]
 **sortBy** | **string** | relevance | price_low_to_high | price_high_to_low | avg_review | newest | 
 **category** | **string** | Department/category alias (i&#x3D; param) | 
 **minPrice** | **float32** |  | 
 **maxPrice** | **float32** |  | 
 **zip** | **string** | Delivery postal/zip code for localized pricing | 
 **language** | **string** | Locale for results, e.g. en_US, fr_FR | 

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


## AmazonTodaySDeals

> interface{} AmazonTodaySDeals(ctx).Domain(domain).Category(category).Page(page).Execute()

Today's deals



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
	domain := "domain_example" // string |  (optional) (default to "com")
	category := "category_example" // string |  (optional)
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AmazonAPI.AmazonTodaySDeals(context.Background()).Domain(domain).Category(category).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AmazonAPI.AmazonTodaySDeals``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AmazonTodaySDeals`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AmazonAPI.AmazonTodaySDeals`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAmazonTodaySDealsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domain** | **string** |  | [default to &quot;com&quot;]
 **category** | **string** |  | 
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


# \DepopAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DepopDepopScraperHealthCheck**](DepopAPI.md#DepopDepopScraperHealthCheck) | **Get** /v1/depop/health | Depop scraper health check
[**DepopDepopScraperHealthCheckHead**](DepopAPI.md#DepopDepopScraperHealthCheckHead) | **Head** /v1/depop/health | Depop scraper health check
[**DepopGetAUserSProducts**](DepopAPI.md#DepopGetAUserSProducts) | **Get** /v1/depop/users/{username}/products | Get a user&#39;s products
[**DepopGetProductDetail**](DepopAPI.md#DepopGetProductDetail) | **Get** /v1/depop/products/{product_id} | Get product detail
[**DepopGetShopUserProfile**](DepopAPI.md#DepopGetShopUserProfile) | **Get** /v1/depop/users/{username} | Get shop/user profile
[**DepopListMarkets**](DepopAPI.md#DepopListMarkets) | **Get** /v1/depop/markets | List markets
[**DepopSearchDepopProducts**](DepopAPI.md#DepopSearchDepopProducts) | **Get** /v1/depop/search | Search Depop products



## DepopDepopScraperHealthCheck

> interface{} DepopDepopScraperHealthCheck(ctx).Execute()

Depop scraper health check



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
	resp, r, err := apiClient.DepopAPI.DepopDepopScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DepopAPI.DepopDepopScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DepopDepopScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DepopAPI.DepopDepopScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiDepopDepopScraperHealthCheckRequest struct via the builder pattern


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


## DepopDepopScraperHealthCheckHead

> interface{} DepopDepopScraperHealthCheckHead(ctx).Execute()

Depop scraper health check



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
	resp, r, err := apiClient.DepopAPI.DepopDepopScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DepopAPI.DepopDepopScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DepopDepopScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DepopAPI.DepopDepopScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiDepopDepopScraperHealthCheckHeadRequest struct via the builder pattern


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


## DepopGetAUserSProducts

> interface{} DepopGetAUserSProducts(ctx, username).Market(market).PerPage(perPage).Cursor(cursor).Execute()

Get a user's products



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
	market := "market_example" // string | Market code (optional) (default to "us")
	perPage := int32(56) // int32 |  (optional) (default to 24)
	cursor := "cursor_example" // string | Pagination cursor (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DepopAPI.DepopGetAUserSProducts(context.Background(), username).Market(market).PerPage(perPage).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DepopAPI.DepopGetAUserSProducts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DepopGetAUserSProducts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DepopAPI.DepopGetAUserSProducts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDepopGetAUserSProductsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | Market code | [default to &quot;us&quot;]
 **perPage** | **int32** |  | [default to 24]
 **cursor** | **string** | Pagination cursor | 

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


## DepopGetProductDetail

> interface{} DepopGetProductDetail(ctx, productId).Market(market).Execute()

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
	productId := "productId_example" // string | 
	market := "market_example" // string | Market code (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DepopAPI.DepopGetProductDetail(context.Background(), productId).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DepopAPI.DepopGetProductDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DepopGetProductDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DepopAPI.DepopGetProductDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**productId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDepopGetProductDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | Market code | [default to &quot;us&quot;]

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


## DepopGetShopUserProfile

> interface{} DepopGetShopUserProfile(ctx, username).Market(market).Execute()

Get shop/user profile



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
	market := "market_example" // string | Market code (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DepopAPI.DepopGetShopUserProfile(context.Background(), username).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DepopAPI.DepopGetShopUserProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DepopGetShopUserProfile`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DepopAPI.DepopGetShopUserProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDepopGetShopUserProfileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | Market code | [default to &quot;us&quot;]

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


## DepopListMarkets

> interface{} DepopListMarkets(ctx).Execute()

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
	resp, r, err := apiClient.DepopAPI.DepopListMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DepopAPI.DepopListMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DepopListMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DepopAPI.DepopListMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiDepopListMarketsRequest struct via the builder pattern


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


## DepopSearchDepopProducts

> interface{} DepopSearchDepopProducts(ctx).Query(query).Market(market).PerPage(perPage).Cursor(cursor).PriceMin(priceMin).PriceMax(priceMax).Brands(brands).Categories(categories).Sizes(sizes).Conditions(conditions).Gender(gender).Sort(sort).Execute()

Search Depop products



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
	query := "query_example" // string | Search text, e.g. 'nike vintage'
	market := "market_example" // string | Market code (us, gb, au, it, fr, ...) (optional) (default to "us")
	perPage := int32(56) // int32 | Results per page (optional) (default to 24)
	cursor := "cursor_example" // string | Pagination cursor (from previous page) (optional)
	priceMin := float32(8.14) // float32 | Minimum price (optional)
	priceMax := float32(8.14) // float32 | Maximum price (optional)
	brands := "brands_example" // string | Comma-separated brand IDs (optional)
	categories := "categories_example" // string | Comma-separated category IDs (optional)
	sizes := "sizes_example" // string | Comma-separated size IDs (optional)
	conditions := "conditions_example" // string | Comma-separated condition slugs (brand_new, used_excellent, ...) (optional)
	gender := "gender_example" // string | male | female (optional)
	sort := "sort_example" // string | relevance | newlyListed | priceAscending | priceDescending (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DepopAPI.DepopSearchDepopProducts(context.Background()).Query(query).Market(market).PerPage(perPage).Cursor(cursor).PriceMin(priceMin).PriceMax(priceMax).Brands(brands).Categories(categories).Sizes(sizes).Conditions(conditions).Gender(gender).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DepopAPI.DepopSearchDepopProducts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DepopSearchDepopProducts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DepopAPI.DepopSearchDepopProducts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiDepopSearchDepopProductsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search text, e.g. &#39;nike vintage&#39; | 
 **market** | **string** | Market code (us, gb, au, it, fr, ...) | [default to &quot;us&quot;]
 **perPage** | **int32** | Results per page | [default to 24]
 **cursor** | **string** | Pagination cursor (from previous page) | 
 **priceMin** | **float32** | Minimum price | 
 **priceMax** | **float32** | Maximum price | 
 **brands** | **string** | Comma-separated brand IDs | 
 **categories** | **string** | Comma-separated category IDs | 
 **sizes** | **string** | Comma-separated size IDs | 
 **conditions** | **string** | Comma-separated condition slugs (brand_new, used_excellent, ...) | 
 **gender** | **string** | male | female | 
 **sort** | **string** | relevance | newlyListed | priceAscending | priceDescending | 

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


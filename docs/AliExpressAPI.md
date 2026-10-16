# \AliExpressAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AliexpressGetCategoryNavigation**](AliExpressAPI.md#AliexpressGetCategoryNavigation) | **Get** /v1/aliexpress/categories | Get category navigation
[**AliexpressGetProductDetail**](AliExpressAPI.md#AliexpressGetProductDetail) | **Get** /v1/aliexpress/products/{product_id} | Get product detail
[**AliexpressGetProductReviews**](AliExpressAPI.md#AliexpressGetProductReviews) | **Get** /v1/aliexpress/products/{product_id}/reviews | Get product reviews
[**AliexpressGetSearchSuggestions**](AliExpressAPI.md#AliexpressGetSearchSuggestions) | **Get** /v1/aliexpress/autocomplete | Get search suggestions
[**AliexpressGetStoreProductCategories**](AliExpressAPI.md#AliexpressGetStoreProductCategories) | **Get** /v1/aliexpress/stores/{store_id}/categories | Get store product categories
[**AliexpressGetStoreProducts**](AliExpressAPI.md#AliexpressGetStoreProducts) | **Get** /v1/aliexpress/stores/{store_id}/products | Get store products
[**AliexpressGetStoreProfile**](AliExpressAPI.md#AliexpressGetStoreProfile) | **Get** /v1/aliexpress/stores/{store_id} | Get store profile
[**AliexpressSearchProducts**](AliExpressAPI.md#AliexpressSearchProducts) | **Get** /v1/aliexpress/search | Search products



## AliexpressGetCategoryNavigation

> interface{} AliexpressGetCategoryNavigation(ctx).Execute()

Get category navigation

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
	resp, r, err := apiClient.AliExpressAPI.AliexpressGetCategoryNavigation(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AliExpressAPI.AliexpressGetCategoryNavigation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AliexpressGetCategoryNavigation`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AliExpressAPI.AliexpressGetCategoryNavigation`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAliexpressGetCategoryNavigationRequest struct via the builder pattern


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


## AliexpressGetProductDetail

> interface{} AliexpressGetProductDetail(ctx, productId).Country(country).Currency(currency).Language(language).Execute()

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
	country := "country_example" // string |  (optional) (default to "US")
	currency := "currency_example" // string |  (optional) (default to "USD")
	language := "language_example" // string |  (optional) (default to "en_US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AliExpressAPI.AliexpressGetProductDetail(context.Background(), productId).Country(country).Currency(currency).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AliExpressAPI.AliexpressGetProductDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AliexpressGetProductDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AliExpressAPI.AliexpressGetProductDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**productId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAliexpressGetProductDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** |  | [default to &quot;US&quot;]
 **currency** | **string** |  | [default to &quot;USD&quot;]
 **language** | **string** |  | [default to &quot;en_US&quot;]

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


## AliexpressGetProductReviews

> interface{} AliexpressGetProductReviews(ctx, productId).Page(page).PageSize(pageSize).Sort(sort).Execute()

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
	productId := "productId_example" // string | 
	page := int32(56) // int32 |  (optional) (default to 1)
	pageSize := int32(56) // int32 |  (optional) (default to 10)
	sort := "sort_example" // string |  (optional) (default to "complex_default")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AliExpressAPI.AliexpressGetProductReviews(context.Background(), productId).Page(page).PageSize(pageSize).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AliExpressAPI.AliexpressGetProductReviews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AliexpressGetProductReviews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AliExpressAPI.AliexpressGetProductReviews`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**productId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAliexpressGetProductReviewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** |  | [default to 1]
 **pageSize** | **int32** |  | [default to 10]
 **sort** | **string** |  | [default to &quot;complex_default&quot;]

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


## AliexpressGetSearchSuggestions

> interface{} AliexpressGetSearchSuggestions(ctx).Query(query).Country(country).Language(language).Execute()

Get search suggestions

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
	query := "query_example" // string | 
	country := "country_example" // string |  (optional) (default to "US")
	language := "language_example" // string |  (optional) (default to "en")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AliExpressAPI.AliexpressGetSearchSuggestions(context.Background()).Query(query).Country(country).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AliExpressAPI.AliexpressGetSearchSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AliexpressGetSearchSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AliExpressAPI.AliexpressGetSearchSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAliexpressGetSearchSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 
 **country** | **string** |  | [default to &quot;US&quot;]
 **language** | **string** |  | [default to &quot;en&quot;]

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


## AliexpressGetStoreProductCategories

> interface{} AliexpressGetStoreProductCategories(ctx, storeId).Country(country).Execute()

Get store product categories

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
	storeId := "storeId_example" // string | 
	country := "country_example" // string |  (optional) (default to "US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AliExpressAPI.AliexpressGetStoreProductCategories(context.Background(), storeId).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AliExpressAPI.AliexpressGetStoreProductCategories``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AliexpressGetStoreProductCategories`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AliExpressAPI.AliexpressGetStoreProductCategories`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**storeId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAliexpressGetStoreProductCategoriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** |  | [default to &quot;US&quot;]

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


## AliexpressGetStoreProducts

> interface{} AliexpressGetStoreProducts(ctx, storeId).Page(page).PageSize(pageSize).Country(country).Currency(currency).Language(language).Query(query).Sort(sort).Execute()

Get store products

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
	storeId := "storeId_example" // string | 
	page := int32(56) // int32 |  (optional) (default to 1)
	pageSize := int32(56) // int32 |  (optional) (default to 24)
	country := "country_example" // string |  (optional) (default to "US")
	currency := "currency_example" // string |  (optional) (default to "USD")
	language := "language_example" // string |  (optional) (default to "en")
	query := "query_example" // string |  (optional) (default to "")
	sort := "sort_example" // string |  (optional) (default to "bestmatch_sort")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AliExpressAPI.AliexpressGetStoreProducts(context.Background(), storeId).Page(page).PageSize(pageSize).Country(country).Currency(currency).Language(language).Query(query).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AliExpressAPI.AliexpressGetStoreProducts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AliexpressGetStoreProducts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AliExpressAPI.AliexpressGetStoreProducts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**storeId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAliexpressGetStoreProductsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** |  | [default to 1]
 **pageSize** | **int32** |  | [default to 24]
 **country** | **string** |  | [default to &quot;US&quot;]
 **currency** | **string** |  | [default to &quot;USD&quot;]
 **language** | **string** |  | [default to &quot;en&quot;]
 **query** | **string** |  | [default to &quot;&quot;]
 **sort** | **string** |  | [default to &quot;bestmatch_sort&quot;]

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


## AliexpressGetStoreProfile

> interface{} AliexpressGetStoreProfile(ctx, storeId).Country(country).Currency(currency).Language(language).Execute()

Get store profile

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
	storeId := "storeId_example" // string | 
	country := "country_example" // string |  (optional) (default to "US")
	currency := "currency_example" // string |  (optional) (default to "USD")
	language := "language_example" // string |  (optional) (default to "en")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AliExpressAPI.AliexpressGetStoreProfile(context.Background(), storeId).Country(country).Currency(currency).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AliExpressAPI.AliexpressGetStoreProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AliexpressGetStoreProfile`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AliExpressAPI.AliexpressGetStoreProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**storeId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAliexpressGetStoreProfileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** |  | [default to &quot;US&quot;]
 **currency** | **string** |  | [default to &quot;USD&quot;]
 **language** | **string** |  | [default to &quot;en&quot;]

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


## AliexpressSearchProducts

> interface{} AliexpressSearchProducts(ctx).Query(query).Page(page).Country(country).Currency(currency).Language(language).Sort(sort).MinPrice(minPrice).MaxPrice(maxPrice).Execute()

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
	query := "query_example" // string | 
	page := int32(56) // int32 |  (optional) (default to 1)
	country := "country_example" // string |  (optional) (default to "US")
	currency := "currency_example" // string |  (optional) (default to "USD")
	language := "language_example" // string |  (optional) (default to "en")
	sort := "sort_example" // string |  (optional) (default to "default")
	minPrice := float32(8.14) // float32 |  (optional)
	maxPrice := float32(8.14) // float32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AliExpressAPI.AliexpressSearchProducts(context.Background()).Query(query).Page(page).Country(country).Currency(currency).Language(language).Sort(sort).MinPrice(minPrice).MaxPrice(maxPrice).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AliExpressAPI.AliexpressSearchProducts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AliexpressSearchProducts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AliExpressAPI.AliexpressSearchProducts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAliexpressSearchProductsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 
 **page** | **int32** |  | [default to 1]
 **country** | **string** |  | [default to &quot;US&quot;]
 **currency** | **string** |  | [default to &quot;USD&quot;]
 **language** | **string** |  | [default to &quot;en&quot;]
 **sort** | **string** |  | [default to &quot;default&quot;]
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


# \BestBuyAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**BestbuyBrowseACategory**](BestBuyAPI.md#BestbuyBrowseACategory) | **Get** /v1/bestbuy/category | Browse a category
[**BestbuyGetCategories**](BestBuyAPI.md#BestbuyGetCategories) | **Get** /v1/bestbuy/categories | Get categories
[**BestbuyGetLaptopAndComputerDeals**](BestBuyAPI.md#BestbuyGetLaptopAndComputerDeals) | **Get** /v1/bestbuy/deals | Get laptop and computer deals
[**BestbuyGetProductAvailability**](BestBuyAPI.md#BestbuyGetProductAvailability) | **Get** /v1/bestbuy/products/{sku}/availability | Get product availability
[**BestbuyGetProductDetail**](BestBuyAPI.md#BestbuyGetProductDetail) | **Get** /v1/bestbuy/products/{sku} | Get product detail
[**BestbuyGetProductQuestions**](BestBuyAPI.md#BestbuyGetProductQuestions) | **Get** /v1/bestbuy/products/{sku}/questions | Get product questions
[**BestbuyGetProductReviews**](BestBuyAPI.md#BestbuyGetProductReviews) | **Get** /v1/bestbuy/products/{sku}/reviews | Get product reviews
[**BestbuyGetSearchSuggestions**](BestBuyAPI.md#BestbuyGetSearchSuggestions) | **Get** /v1/bestbuy/autocomplete | Get search suggestions
[**BestbuyListSupportedMarkets**](BestBuyAPI.md#BestbuyListSupportedMarkets) | **Get** /v1/bestbuy/markets | List supported markets
[**BestbuySearchProducts**](BestBuyAPI.md#BestbuySearchProducts) | **Get** /v1/bestbuy/search | Search products



## BestbuyBrowseACategory

> interface{} BestbuyBrowseACategory(ctx).CategoryId(categoryId).Page(page).Execute()

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
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BestBuyAPI.BestbuyBrowseACategory(context.Background()).CategoryId(categoryId).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BestBuyAPI.BestbuyBrowseACategory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BestbuyBrowseACategory`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BestBuyAPI.BestbuyBrowseACategory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBestbuyBrowseACategoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **categoryId** | **string** |  | 
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


## BestbuyGetCategories

> interface{} BestbuyGetCategories(ctx).Query(query).Execute()

Get categories

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
	query := "query_example" // string |  (optional) (default to "laptop")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BestBuyAPI.BestbuyGetCategories(context.Background()).Query(query).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BestBuyAPI.BestbuyGetCategories``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BestbuyGetCategories`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BestBuyAPI.BestbuyGetCategories`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBestbuyGetCategoriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | [default to &quot;laptop&quot;]

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


## BestbuyGetLaptopAndComputerDeals

> interface{} BestbuyGetLaptopAndComputerDeals(ctx).Page(page).Execute()

Get laptop and computer deals

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BestBuyAPI.BestbuyGetLaptopAndComputerDeals(context.Background()).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BestBuyAPI.BestbuyGetLaptopAndComputerDeals``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BestbuyGetLaptopAndComputerDeals`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BestBuyAPI.BestbuyGetLaptopAndComputerDeals`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBestbuyGetLaptopAndComputerDealsRequest struct via the builder pattern


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


## BestbuyGetProductAvailability

> interface{} BestbuyGetProductAvailability(ctx, sku).ZipCode(zipCode).StoreId(storeId).Execute()

Get product availability

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
	sku := "sku_example" // string | 
	zipCode := "zipCode_example" // string | 
	storeId := "storeId_example" // string |  (optional) (default to "7")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BestBuyAPI.BestbuyGetProductAvailability(context.Background(), sku).ZipCode(zipCode).StoreId(storeId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BestBuyAPI.BestbuyGetProductAvailability``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BestbuyGetProductAvailability`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BestBuyAPI.BestbuyGetProductAvailability`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sku** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiBestbuyGetProductAvailabilityRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **zipCode** | **string** |  | 
 **storeId** | **string** |  | [default to &quot;7&quot;]

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


## BestbuyGetProductDetail

> interface{} BestbuyGetProductDetail(ctx, sku).Execute()

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
	sku := "sku_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BestBuyAPI.BestbuyGetProductDetail(context.Background(), sku).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BestBuyAPI.BestbuyGetProductDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BestbuyGetProductDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BestBuyAPI.BestbuyGetProductDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sku** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiBestbuyGetProductDetailRequest struct via the builder pattern


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


## BestbuyGetProductQuestions

> interface{} BestbuyGetProductQuestions(ctx, sku).Page(page).PageSize(pageSize).Query(query).Execute()

Get product questions

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
	sku := "sku_example" // string | 
	page := int32(56) // int32 |  (optional) (default to 1)
	pageSize := int32(56) // int32 |  (optional) (default to 10)
	query := "query_example" // string |  (optional) (default to "")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BestBuyAPI.BestbuyGetProductQuestions(context.Background(), sku).Page(page).PageSize(pageSize).Query(query).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BestBuyAPI.BestbuyGetProductQuestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BestbuyGetProductQuestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BestBuyAPI.BestbuyGetProductQuestions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sku** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiBestbuyGetProductQuestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** |  | [default to 1]
 **pageSize** | **int32** |  | [default to 10]
 **query** | **string** |  | [default to &quot;&quot;]

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


## BestbuyGetProductReviews

> interface{} BestbuyGetProductReviews(ctx, sku).Page(page).PageSize(pageSize).Sort(sort).Execute()

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
	sku := "sku_example" // string | 
	page := int32(56) // int32 |  (optional) (default to 1)
	pageSize := int32(56) // int32 |  (optional) (default to 10)
	sort := "sort_example" // string |  (optional) (default to "MOST_RECENT")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BestBuyAPI.BestbuyGetProductReviews(context.Background(), sku).Page(page).PageSize(pageSize).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BestBuyAPI.BestbuyGetProductReviews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BestbuyGetProductReviews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BestBuyAPI.BestbuyGetProductReviews`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**sku** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiBestbuyGetProductReviewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** |  | [default to 1]
 **pageSize** | **int32** |  | [default to 10]
 **sort** | **string** |  | [default to &quot;MOST_RECENT&quot;]

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


## BestbuyGetSearchSuggestions

> interface{} BestbuyGetSearchSuggestions(ctx).Query(query).Execute()

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BestBuyAPI.BestbuyGetSearchSuggestions(context.Background()).Query(query).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BestBuyAPI.BestbuyGetSearchSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BestbuyGetSearchSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BestBuyAPI.BestbuyGetSearchSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBestbuyGetSearchSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
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


## BestbuyListSupportedMarkets

> interface{} BestbuyListSupportedMarkets(ctx).Execute()

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
	resp, r, err := apiClient.BestBuyAPI.BestbuyListSupportedMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BestBuyAPI.BestbuyListSupportedMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BestbuyListSupportedMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BestBuyAPI.BestbuyListSupportedMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiBestbuyListSupportedMarketsRequest struct via the builder pattern


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


## BestbuySearchProducts

> interface{} BestbuySearchProducts(ctx).Query(query).Page(page).Sort(sort).Execute()

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
	sort := "sort_example" // string |  (optional) (default to "best_match")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BestBuyAPI.BestbuySearchProducts(context.Background()).Query(query).Page(page).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BestBuyAPI.BestbuySearchProducts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BestbuySearchProducts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BestBuyAPI.BestbuySearchProducts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBestbuySearchProductsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 
 **page** | **int32** |  | [default to 1]
 **sort** | **string** |  | [default to &quot;best_match&quot;]

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


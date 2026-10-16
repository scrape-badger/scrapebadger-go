# \TargetAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**TargetBrowseACategory**](TargetAPI.md#TargetBrowseACategory) | **Get** /v1/target/category | Browse a category
[**TargetFindNearbyStores**](TargetAPI.md#TargetFindNearbyStores) | **Get** /v1/target/stores | Find nearby stores
[**TargetGetCategories**](TargetAPI.md#TargetGetCategories) | **Get** /v1/target/categories | Get categories
[**TargetGetProductAvailability**](TargetAPI.md#TargetGetProductAvailability) | **Get** /v1/target/products/{tcin}/availability | Get product availability
[**TargetGetProductDetail**](TargetAPI.md#TargetGetProductDetail) | **Get** /v1/target/products/{tcin} | Get product detail
[**TargetGetProductQuestions**](TargetAPI.md#TargetGetProductQuestions) | **Get** /v1/target/products/{tcin}/questions | Get product questions
[**TargetGetProductReviews**](TargetAPI.md#TargetGetProductReviews) | **Get** /v1/target/products/{tcin}/reviews | Get product reviews
[**TargetGetSearchSuggestions**](TargetAPI.md#TargetGetSearchSuggestions) | **Get** /v1/target/autocomplete | Get search suggestions
[**TargetGetStoreDetail**](TargetAPI.md#TargetGetStoreDetail) | **Get** /v1/target/stores/{store_id} | Get store detail
[**TargetListSupportedMarkets**](TargetAPI.md#TargetListSupportedMarkets) | **Get** /v1/target/markets | List supported markets
[**TargetSearchProducts**](TargetAPI.md#TargetSearchProducts) | **Get** /v1/target/search | Search products



## TargetBrowseACategory

> interface{} TargetBrowseACategory(ctx).CategoryId(categoryId).Page(page).PageSize(pageSize).StoreId(storeId).ZipCode(zipCode).Execute()

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
	pageSize := int32(56) // int32 |  (optional) (default to 24)
	storeId := "storeId_example" // string |  (optional) (default to "1375")
	zipCode := "zipCode_example" // string |  (optional) (default to "55403")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TargetAPI.TargetBrowseACategory(context.Background()).CategoryId(categoryId).Page(page).PageSize(pageSize).StoreId(storeId).ZipCode(zipCode).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TargetAPI.TargetBrowseACategory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TargetBrowseACategory`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TargetAPI.TargetBrowseACategory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTargetBrowseACategoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **categoryId** | **string** |  | 
 **page** | **int32** |  | [default to 1]
 **pageSize** | **int32** |  | [default to 24]
 **storeId** | **string** |  | [default to &quot;1375&quot;]
 **zipCode** | **string** |  | [default to &quot;55403&quot;]

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


## TargetFindNearbyStores

> interface{} TargetFindNearbyStores(ctx).ZipCode(zipCode).Limit(limit).Execute()

Find nearby stores

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
	zipCode := "zipCode_example" // string | 
	limit := int32(56) // int32 |  (optional) (default to 10)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TargetAPI.TargetFindNearbyStores(context.Background()).ZipCode(zipCode).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TargetAPI.TargetFindNearbyStores``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TargetFindNearbyStores`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TargetAPI.TargetFindNearbyStores`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTargetFindNearbyStoresRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **zipCode** | **string** |  | 
 **limit** | **int32** |  | [default to 10]

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


## TargetGetCategories

> interface{} TargetGetCategories(ctx).CategoryId(categoryId).Execute()

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
	categoryId := "categoryId_example" // string |  (optional) (default to "5xtly")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TargetAPI.TargetGetCategories(context.Background()).CategoryId(categoryId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TargetAPI.TargetGetCategories``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TargetGetCategories`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TargetAPI.TargetGetCategories`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTargetGetCategoriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **categoryId** | **string** |  | [default to &quot;5xtly&quot;]

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


## TargetGetProductAvailability

> interface{} TargetGetProductAvailability(ctx, tcin).ZipCode(zipCode).Limit(limit).Execute()

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
	tcin := "tcin_example" // string | 
	zipCode := "zipCode_example" // string | 
	limit := int32(56) // int32 |  (optional) (default to 10)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TargetAPI.TargetGetProductAvailability(context.Background(), tcin).ZipCode(zipCode).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TargetAPI.TargetGetProductAvailability``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TargetGetProductAvailability`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TargetAPI.TargetGetProductAvailability`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tcin** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTargetGetProductAvailabilityRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **zipCode** | **string** |  | 
 **limit** | **int32** |  | [default to 10]

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


## TargetGetProductDetail

> interface{} TargetGetProductDetail(ctx, tcin).StoreId(storeId).ZipCode(zipCode).Execute()

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
	tcin := "tcin_example" // string | 
	storeId := "storeId_example" // string |  (optional) (default to "1375")
	zipCode := "zipCode_example" // string |  (optional) (default to "55403")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TargetAPI.TargetGetProductDetail(context.Background(), tcin).StoreId(storeId).ZipCode(zipCode).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TargetAPI.TargetGetProductDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TargetGetProductDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TargetAPI.TargetGetProductDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tcin** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTargetGetProductDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **storeId** | **string** |  | [default to &quot;1375&quot;]
 **zipCode** | **string** |  | [default to &quot;55403&quot;]

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


## TargetGetProductQuestions

> interface{} TargetGetProductQuestions(ctx, tcin).Page(page).PageSize(pageSize).Execute()

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
	tcin := "tcin_example" // string | 
	page := int32(56) // int32 |  (optional) (default to 1)
	pageSize := int32(56) // int32 |  (optional) (default to 10)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TargetAPI.TargetGetProductQuestions(context.Background(), tcin).Page(page).PageSize(pageSize).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TargetAPI.TargetGetProductQuestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TargetGetProductQuestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TargetAPI.TargetGetProductQuestions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tcin** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTargetGetProductQuestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** |  | [default to 1]
 **pageSize** | **int32** |  | [default to 10]

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


## TargetGetProductReviews

> interface{} TargetGetProductReviews(ctx, tcin).Page(page).PageSize(pageSize).Sort(sort).Execute()

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
	tcin := "tcin_example" // string | 
	page := int32(56) // int32 |  (optional) (default to 1)
	pageSize := int32(56) // int32 |  (optional) (default to 10)
	sort := "sort_example" // string |  (optional) (default to "most_recent")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TargetAPI.TargetGetProductReviews(context.Background(), tcin).Page(page).PageSize(pageSize).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TargetAPI.TargetGetProductReviews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TargetGetProductReviews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TargetAPI.TargetGetProductReviews`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tcin** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTargetGetProductReviewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** |  | [default to 1]
 **pageSize** | **int32** |  | [default to 10]
 **sort** | **string** |  | [default to &quot;most_recent&quot;]

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


## TargetGetSearchSuggestions

> interface{} TargetGetSearchSuggestions(ctx).Query(query).Execute()

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
	resp, r, err := apiClient.TargetAPI.TargetGetSearchSuggestions(context.Background()).Query(query).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TargetAPI.TargetGetSearchSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TargetGetSearchSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TargetAPI.TargetGetSearchSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTargetGetSearchSuggestionsRequest struct via the builder pattern


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


## TargetGetStoreDetail

> interface{} TargetGetStoreDetail(ctx, storeId).Execute()

Get store detail

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TargetAPI.TargetGetStoreDetail(context.Background(), storeId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TargetAPI.TargetGetStoreDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TargetGetStoreDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TargetAPI.TargetGetStoreDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**storeId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTargetGetStoreDetailRequest struct via the builder pattern


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


## TargetListSupportedMarkets

> interface{} TargetListSupportedMarkets(ctx).Execute()

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
	resp, r, err := apiClient.TargetAPI.TargetListSupportedMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TargetAPI.TargetListSupportedMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TargetListSupportedMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TargetAPI.TargetListSupportedMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiTargetListSupportedMarketsRequest struct via the builder pattern


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


## TargetSearchProducts

> interface{} TargetSearchProducts(ctx).Query(query).Page(page).PageSize(pageSize).StoreId(storeId).ZipCode(zipCode).Sort(sort).Execute()

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
	pageSize := int32(56) // int32 |  (optional) (default to 24)
	storeId := "storeId_example" // string |  (optional) (default to "1375")
	zipCode := "zipCode_example" // string |  (optional) (default to "55403")
	sort := "sort_example" // string |  (optional) (default to "relevance")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TargetAPI.TargetSearchProducts(context.Background()).Query(query).Page(page).PageSize(pageSize).StoreId(storeId).ZipCode(zipCode).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TargetAPI.TargetSearchProducts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TargetSearchProducts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TargetAPI.TargetSearchProducts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTargetSearchProductsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 
 **page** | **int32** |  | [default to 1]
 **pageSize** | **int32** |  | [default to 24]
 **storeId** | **string** |  | [default to &quot;1375&quot;]
 **zipCode** | **string** |  | [default to &quot;55403&quot;]
 **sort** | **string** |  | [default to &quot;relevance&quot;]

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


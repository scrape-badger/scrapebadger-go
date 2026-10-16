# \ASOSAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AsosGetProductDetail**](ASOSAPI.md#AsosGetProductDetail) | **Get** /v1/asos/products/{product_id} | Get product detail
[**AsosGetStockAndPrices**](ASOSAPI.md#AsosGetStockAndPrices) | **Get** /v1/asos/stock-price | Get stock and prices
[**AsosListCategories**](ASOSAPI.md#AsosListCategories) | **Get** /v1/asos/categories | List categories
[**AsosListMarkets**](ASOSAPI.md#AsosListMarkets) | **Get** /v1/asos/markets | List markets
[**AsosListSearchFilters**](ASOSAPI.md#AsosListSearchFilters) | **Get** /v1/asos/filters | List search filters
[**AsosSearchProducts**](ASOSAPI.md#AsosSearchProducts) | **Get** /v1/asos/search | Search products
[**AsosSearchSuggestions**](ASOSAPI.md#AsosSearchSuggestions) | **Get** /v1/asos/autocomplete | Search suggestions



## AsosGetProductDetail

> ProductResponse AsosGetProductDetail(ctx, productId).Market(market).Store(store).Country(country).Currency(currency).Language(language).Execute()

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
	productId := int32(56) // int32 | 
	market := "market_example" // string | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl (optional) (default to "uk")
	store := "store_example" // string | Override store, e.g. COM or US (optional)
	country := "country_example" // string | ISO country override (optional)
	currency := "currency_example" // string | Currency override (optional)
	language := "language_example" // string | Locale override, e.g. en-GB (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ASOSAPI.AsosGetProductDetail(context.Background(), productId).Market(market).Store(store).Country(country).Currency(currency).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ASOSAPI.AsosGetProductDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AsosGetProductDetail`: ProductResponse
	fmt.Fprintf(os.Stdout, "Response from `ASOSAPI.AsosGetProductDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**productId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAsosGetProductDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl | [default to &quot;uk&quot;]
 **store** | **string** | Override store, e.g. COM or US | 
 **country** | **string** | ISO country override | 
 **currency** | **string** | Currency override | 
 **language** | **string** | Locale override, e.g. en-GB | 

### Return type

[**ProductResponse**](ProductResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AsosGetStockAndPrices

> StockResponse AsosGetStockAndPrices(ctx).ProductIds(productIds).Market(market).Store(store).Country(country).Currency(currency).Language(language).Execute()

Get stock and prices



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
	productIds := "productIds_example" // string | 1–50 comma-separated product ids
	market := "market_example" // string | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl (optional) (default to "uk")
	store := "store_example" // string | Override store, e.g. COM or US (optional)
	country := "country_example" // string | ISO country override (optional)
	currency := "currency_example" // string | Currency override (optional)
	language := "language_example" // string | Locale override, e.g. en-GB (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ASOSAPI.AsosGetStockAndPrices(context.Background()).ProductIds(productIds).Market(market).Store(store).Country(country).Currency(currency).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ASOSAPI.AsosGetStockAndPrices``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AsosGetStockAndPrices`: StockResponse
	fmt.Fprintf(os.Stdout, "Response from `ASOSAPI.AsosGetStockAndPrices`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAsosGetStockAndPricesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productIds** | **string** | 1–50 comma-separated product ids | 
 **market** | **string** | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl | [default to &quot;uk&quot;]
 **store** | **string** | Override store, e.g. COM or US | 
 **country** | **string** | ISO country override | 
 **currency** | **string** | Currency override | 
 **language** | **string** | Locale override, e.g. en-GB | 

### Return type

[**StockResponse**](StockResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AsosListCategories

> interface{} AsosListCategories(ctx).Gender(gender).Market(market).Store(store).Country(country).Currency(currency).Language(language).Execute()

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
	gender := "gender_example" // string |  (optional) (default to "men")
	market := "market_example" // string | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl (optional) (default to "uk")
	store := "store_example" // string | Override store, e.g. COM or US (optional)
	country := "country_example" // string | ISO country override (optional)
	currency := "currency_example" // string | Currency override (optional)
	language := "language_example" // string | Locale override, e.g. en-GB (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ASOSAPI.AsosListCategories(context.Background()).Gender(gender).Market(market).Store(store).Country(country).Currency(currency).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ASOSAPI.AsosListCategories``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AsosListCategories`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ASOSAPI.AsosListCategories`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAsosListCategoriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gender** | **string** |  | [default to &quot;men&quot;]
 **market** | **string** | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl | [default to &quot;uk&quot;]
 **store** | **string** | Override store, e.g. COM or US | 
 **country** | **string** | ISO country override | 
 **currency** | **string** | Currency override | 
 **language** | **string** | Locale override, e.g. en-GB | 

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


## AsosListMarkets

> interface{} AsosListMarkets(ctx).Execute()

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
	resp, r, err := apiClient.ASOSAPI.AsosListMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ASOSAPI.AsosListMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AsosListMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ASOSAPI.AsosListMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAsosListMarketsRequest struct via the builder pattern


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


## AsosListSearchFilters

> interface{} AsosListSearchFilters(ctx).Query(query).CategoryId(categoryId).Market(market).Store(store).Country(country).Currency(currency).Language(language).Execute()

List search filters



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
	query := "query_example" // string |  (optional)
	categoryId := int32(56) // int32 |  (optional)
	market := "market_example" // string | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl (optional) (default to "uk")
	store := "store_example" // string | Override store, e.g. COM or US (optional)
	country := "country_example" // string | ISO country override (optional)
	currency := "currency_example" // string | Currency override (optional)
	language := "language_example" // string | Locale override, e.g. en-GB (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ASOSAPI.AsosListSearchFilters(context.Background()).Query(query).CategoryId(categoryId).Market(market).Store(store).Country(country).Currency(currency).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ASOSAPI.AsosListSearchFilters``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AsosListSearchFilters`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ASOSAPI.AsosListSearchFilters`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAsosListSearchFiltersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 
 **categoryId** | **int32** |  | 
 **market** | **string** | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl | [default to &quot;uk&quot;]
 **store** | **string** | Override store, e.g. COM or US | 
 **country** | **string** | ISO country override | 
 **currency** | **string** | Currency override | 
 **language** | **string** | Locale override, e.g. en-GB | 

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


## AsosSearchProducts

> PortalApiRoutersV1AsosSearchResponse AsosSearchProducts(ctx).Query(query).CategoryId(categoryId).Offset(offset).Limit(limit).Sort(sort).Brand(brand).Colour(colour).Size(size).MinPrice(minPrice).MaxPrice(maxPrice).Market(market).Store(store).Country(country).Currency(currency).Language(language).Execute()

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
	query := "query_example" // string | Keyword, e.g. shoes (optional)
	categoryId := int32(56) // int32 | Category id from navigation (optional)
	offset := int32(56) // int32 |  (optional) (default to 0)
	limit := int32(56) // int32 |  (optional) (default to 48)
	sort := "sort_example" // string |  (optional) (default to "recommended")
	brand := "brand_example" // string | Comma-separated brand facet ids (optional)
	colour := "colour_example" // string | Comma-separated colour facet ids (optional)
	size := "size_example" // string | Comma-separated size facet ids (optional)
	minPrice := float32(8.14) // float32 |  (optional)
	maxPrice := float32(8.14) // float32 |  (optional)
	market := "market_example" // string | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl (optional) (default to "uk")
	store := "store_example" // string | Override store, e.g. COM or US (optional)
	country := "country_example" // string | ISO country override (optional)
	currency := "currency_example" // string | Currency override (optional)
	language := "language_example" // string | Locale override, e.g. en-GB (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ASOSAPI.AsosSearchProducts(context.Background()).Query(query).CategoryId(categoryId).Offset(offset).Limit(limit).Sort(sort).Brand(brand).Colour(colour).Size(size).MinPrice(minPrice).MaxPrice(maxPrice).Market(market).Store(store).Country(country).Currency(currency).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ASOSAPI.AsosSearchProducts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AsosSearchProducts`: PortalApiRoutersV1AsosSearchResponse
	fmt.Fprintf(os.Stdout, "Response from `ASOSAPI.AsosSearchProducts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAsosSearchProductsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Keyword, e.g. shoes | 
 **categoryId** | **int32** | Category id from navigation | 
 **offset** | **int32** |  | [default to 0]
 **limit** | **int32** |  | [default to 48]
 **sort** | **string** |  | [default to &quot;recommended&quot;]
 **brand** | **string** | Comma-separated brand facet ids | 
 **colour** | **string** | Comma-separated colour facet ids | 
 **size** | **string** | Comma-separated size facet ids | 
 **minPrice** | **float32** |  | 
 **maxPrice** | **float32** |  | 
 **market** | **string** | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl | [default to &quot;uk&quot;]
 **store** | **string** | Override store, e.g. COM or US | 
 **country** | **string** | ISO country override | 
 **currency** | **string** | Currency override | 
 **language** | **string** | Locale override, e.g. en-GB | 

### Return type

[**PortalApiRoutersV1AsosSearchResponse**](PortalApiRoutersV1AsosSearchResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AsosSearchSuggestions

> interface{} AsosSearchSuggestions(ctx).Query(query).Market(market).Store(store).Country(country).Currency(currency).Language(language).Execute()

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
	query := "query_example" // string | 
	market := "market_example" // string | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl (optional) (default to "uk")
	store := "store_example" // string | Override store, e.g. COM or US (optional)
	country := "country_example" // string | ISO country override (optional)
	currency := "currency_example" // string | Currency override (optional)
	language := "language_example" // string | Locale override, e.g. en-GB (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ASOSAPI.AsosSearchSuggestions(context.Background()).Query(query).Market(market).Store(store).Country(country).Currency(currency).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ASOSAPI.AsosSearchSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AsosSearchSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ASOSAPI.AsosSearchSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAsosSearchSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 
 **market** | **string** | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl | [default to &quot;uk&quot;]
 **store** | **string** | Override store, e.g. COM or US | 
 **country** | **string** | ISO country override | 
 **currency** | **string** | Currency override | 
 **language** | **string** | Locale override, e.g. en-GB | 

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


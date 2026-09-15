# \VintedAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**VintedGetItemDetails**](VintedAPI.md#VintedGetItemDetails) | **Get** /v1/vinted/items/{item_id} | Get item details
[**VintedGetUserProfile**](VintedAPI.md#VintedGetUserProfile) | **Get** /v1/vinted/users/{user_id} | Get user profile
[**VintedGetUserSListedItems**](VintedAPI.md#VintedGetUserSListedItems) | **Get** /v1/vinted/users/{user_id}/items | Get user&#39;s listed items
[**VintedListColors**](VintedAPI.md#VintedListColors) | **Get** /v1/vinted/colors | List colors
[**VintedListItemConditions**](VintedAPI.md#VintedListItemConditions) | **Get** /v1/vinted/statuses | List item conditions
[**VintedListMarkets**](VintedAPI.md#VintedListMarkets) | **Get** /v1/vinted/markets | List markets
[**VintedListPublicVintedMobileOperations**](VintedAPI.md#VintedListPublicVintedMobileOperations) | **Get** /v1/vinted/mobile/operations | List public Vinted mobile operations
[**VintedReadVintedMobileData**](VintedAPI.md#VintedReadVintedMobileData) | **Post** /v1/vinted/mobile/{operation} | Read Vinted mobile data
[**VintedSearchBrands**](VintedAPI.md#VintedSearchBrands) | **Get** /v1/vinted/brands | Search brands
[**VintedSearchByImage**](VintedAPI.md#VintedSearchByImage) | **Post** /v1/vinted/search_by_image | Search by image
[**VintedSearchVintedItems**](VintedAPI.md#VintedSearchVintedItems) | **Get** /v1/vinted/search | Search Vinted items
[**VintedVintedScraperHealthCheck**](VintedAPI.md#VintedVintedScraperHealthCheck) | **Get** /v1/vinted/health | Vinted scraper health check
[**VintedVintedScraperHealthCheckHead**](VintedAPI.md#VintedVintedScraperHealthCheckHead) | **Head** /v1/vinted/health | Vinted scraper health check



## VintedGetItemDetails

> interface{} VintedGetItemDetails(ctx, itemId).Market(market).Execute()

Get item details



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
	itemId := int32(56) // int32 | 
	market := "market_example" // string |  (optional) (default to "fr")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VintedAPI.VintedGetItemDetails(context.Background(), itemId).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VintedAPI.VintedGetItemDetails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VintedGetItemDetails`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `VintedAPI.VintedGetItemDetails`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**itemId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiVintedGetItemDetailsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** |  | [default to &quot;fr&quot;]

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


## VintedGetUserProfile

> interface{} VintedGetUserProfile(ctx, userId).Market(market).Execute()

Get user profile



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
	userId := int32(56) // int32 | 
	market := "market_example" // string |  (optional) (default to "fr")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VintedAPI.VintedGetUserProfile(context.Background(), userId).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VintedAPI.VintedGetUserProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VintedGetUserProfile`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `VintedAPI.VintedGetUserProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiVintedGetUserProfileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** |  | [default to &quot;fr&quot;]

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


## VintedGetUserSListedItems

> interface{} VintedGetUserSListedItems(ctx, userId).Market(market).Page(page).PerPage(perPage).Execute()

Get user's listed items



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
	userId := int32(56) // int32 | 
	market := "market_example" // string |  (optional) (default to "fr")
	page := int32(56) // int32 |  (optional) (default to 1)
	perPage := int32(56) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VintedAPI.VintedGetUserSListedItems(context.Background(), userId).Market(market).Page(page).PerPage(perPage).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VintedAPI.VintedGetUserSListedItems``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VintedGetUserSListedItems`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `VintedAPI.VintedGetUserSListedItems`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiVintedGetUserSListedItemsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** |  | [default to &quot;fr&quot;]
 **page** | **int32** |  | [default to 1]
 **perPage** | **int32** |  | [default to 20]

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


## VintedListColors

> interface{} VintedListColors(ctx).Market(market).Execute()

List colors



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
	market := "market_example" // string |  (optional) (default to "fr")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VintedAPI.VintedListColors(context.Background()).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VintedAPI.VintedListColors``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VintedListColors`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `VintedAPI.VintedListColors`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiVintedListColorsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **market** | **string** |  | [default to &quot;fr&quot;]

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


## VintedListItemConditions

> interface{} VintedListItemConditions(ctx).Market(market).Execute()

List item conditions



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
	market := "market_example" // string |  (optional) (default to "fr")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VintedAPI.VintedListItemConditions(context.Background()).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VintedAPI.VintedListItemConditions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VintedListItemConditions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `VintedAPI.VintedListItemConditions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiVintedListItemConditionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **market** | **string** |  | [default to &quot;fr&quot;]

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


## VintedListMarkets

> interface{} VintedListMarkets(ctx).Execute()

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
	resp, r, err := apiClient.VintedAPI.VintedListMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VintedAPI.VintedListMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VintedListMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `VintedAPI.VintedListMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiVintedListMarketsRequest struct via the builder pattern


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


## VintedListPublicVintedMobileOperations

> interface{} VintedListPublicVintedMobileOperations(ctx).Execute()

List public Vinted mobile operations



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
	resp, r, err := apiClient.VintedAPI.VintedListPublicVintedMobileOperations(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VintedAPI.VintedListPublicVintedMobileOperations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VintedListPublicVintedMobileOperations`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `VintedAPI.VintedListPublicVintedMobileOperations`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiVintedListPublicVintedMobileOperationsRequest struct via the builder pattern


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


## VintedReadVintedMobileData

> interface{} VintedReadVintedMobileData(ctx, operation).VintedMobileReadRequest(vintedMobileReadRequest).Execute()

Read Vinted mobile data



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
	operation := "operation_example" // string | 
	vintedMobileReadRequest := *openapiclient.NewVintedMobileReadRequest() // VintedMobileReadRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VintedAPI.VintedReadVintedMobileData(context.Background(), operation).VintedMobileReadRequest(vintedMobileReadRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VintedAPI.VintedReadVintedMobileData``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VintedReadVintedMobileData`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `VintedAPI.VintedReadVintedMobileData`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**operation** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiVintedReadVintedMobileDataRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **vintedMobileReadRequest** | [**VintedMobileReadRequest**](VintedMobileReadRequest.md) |  | 

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


## VintedSearchBrands

> interface{} VintedSearchBrands(ctx).Keyword(keyword).Market(market).Execute()

Search brands



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
	keyword := "keyword_example" // string | Brand search keyword
	market := "market_example" // string |  (optional) (default to "fr")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VintedAPI.VintedSearchBrands(context.Background()).Keyword(keyword).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VintedAPI.VintedSearchBrands``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VintedSearchBrands`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `VintedAPI.VintedSearchBrands`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiVintedSearchBrandsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **keyword** | **string** | Brand search keyword | 
 **market** | **string** |  | [default to &quot;fr&quot;]

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


## VintedSearchByImage

> interface{} VintedSearchByImage(ctx).VintedImageSearchRequest(vintedImageSearchRequest).Execute()

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
	vintedImageSearchRequest := *openapiclient.NewVintedImageSearchRequest() // VintedImageSearchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VintedAPI.VintedSearchByImage(context.Background()).VintedImageSearchRequest(vintedImageSearchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VintedAPI.VintedSearchByImage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VintedSearchByImage`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `VintedAPI.VintedSearchByImage`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiVintedSearchByImageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vintedImageSearchRequest** | [**VintedImageSearchRequest**](VintedImageSearchRequest.md) |  | 

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


## VintedSearchVintedItems

> interface{} VintedSearchVintedItems(ctx).Query(query).Market(market).SellerCountry(sellerCountry).Page(page).PerPage(perPage).PriceFrom(priceFrom).PriceTo(priceTo).BrandIds(brandIds).CatalogIds(catalogIds).ColorIds(colorIds).SizeIds(sizeIds).MaterialIds(materialIds).Time(time).SearchSessionId(searchSessionId).StatusIds(statusIds).Order(order).Execute()

Search Vinted items



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
	query := "query_example" // string | Search text
	market := "market_example" // string | Market code (optional) (default to "fr")
	sellerCountry := "sellerCountry_example" // string | Filter to items whose seller is physically located in one of these comma-separated ISO-2 country codes (e.g. 'fr' or 'fr,be'). Market domains federate cross-border EU listings and Vinted has no native country filter, so each item is enriched with its seller's country and non-matching ones are dropped. Adds 1 credit per uncached seller looked up (cached for 7 days). (optional)
	page := int32(56) // int32 |  (optional) (default to 1)
	perPage := int32(56) // int32 |  (optional) (default to 20)
	priceFrom := float32(8.14) // float32 |  (optional)
	priceTo := float32(8.14) // float32 |  (optional)
	brandIds := "brandIds_example" // string |  (optional)
	catalogIds := "catalogIds_example" // string | Comma-separated Vinted catalog (category) IDs to restrict the search to, e.g. '1904' or '1904,79'. Vinted applies this before searching, so pagination totals reflect the filtered set. A catalog ID is the `catalog[]` value in a Vinted category URL (vinted.fr/catalog?catalog[]=1904). (optional)
	colorIds := "colorIds_example" // string | Comma-separated color IDs (optional)
	sizeIds := "sizeIds_example" // string | Comma-separated size IDs (optional)
	materialIds := "materialIds_example" // string | Comma-separated material IDs (optional)
	time := int32(56) // int32 | Pagination time returned by the preceding page (optional)
	searchSessionId := "searchSessionId_example" // string | Reuse across pages of one search (optional)
	statusIds := "statusIds_example" // string | Comma-separated condition/status IDs (optional)
	order := "order_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VintedAPI.VintedSearchVintedItems(context.Background()).Query(query).Market(market).SellerCountry(sellerCountry).Page(page).PerPage(perPage).PriceFrom(priceFrom).PriceTo(priceTo).BrandIds(brandIds).CatalogIds(catalogIds).ColorIds(colorIds).SizeIds(sizeIds).MaterialIds(materialIds).Time(time).SearchSessionId(searchSessionId).StatusIds(statusIds).Order(order).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VintedAPI.VintedSearchVintedItems``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VintedSearchVintedItems`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `VintedAPI.VintedSearchVintedItems`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiVintedSearchVintedItemsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search text | 
 **market** | **string** | Market code | [default to &quot;fr&quot;]
 **sellerCountry** | **string** | Filter to items whose seller is physically located in one of these comma-separated ISO-2 country codes (e.g. &#39;fr&#39; or &#39;fr,be&#39;). Market domains federate cross-border EU listings and Vinted has no native country filter, so each item is enriched with its seller&#39;s country and non-matching ones are dropped. Adds 1 credit per uncached seller looked up (cached for 7 days). | 
 **page** | **int32** |  | [default to 1]
 **perPage** | **int32** |  | [default to 20]
 **priceFrom** | **float32** |  | 
 **priceTo** | **float32** |  | 
 **brandIds** | **string** |  | 
 **catalogIds** | **string** | Comma-separated Vinted catalog (category) IDs to restrict the search to, e.g. &#39;1904&#39; or &#39;1904,79&#39;. Vinted applies this before searching, so pagination totals reflect the filtered set. A catalog ID is the &#x60;catalog[]&#x60; value in a Vinted category URL (vinted.fr/catalog?catalog[]&#x3D;1904). | 
 **colorIds** | **string** | Comma-separated color IDs | 
 **sizeIds** | **string** | Comma-separated size IDs | 
 **materialIds** | **string** | Comma-separated material IDs | 
 **time** | **int32** | Pagination time returned by the preceding page | 
 **searchSessionId** | **string** | Reuse across pages of one search | 
 **statusIds** | **string** | Comma-separated condition/status IDs | 
 **order** | **string** |  | 

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


## VintedVintedScraperHealthCheck

> interface{} VintedVintedScraperHealthCheck(ctx).Execute()

Vinted scraper health check



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
	resp, r, err := apiClient.VintedAPI.VintedVintedScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VintedAPI.VintedVintedScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VintedVintedScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `VintedAPI.VintedVintedScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiVintedVintedScraperHealthCheckRequest struct via the builder pattern


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


## VintedVintedScraperHealthCheckHead

> interface{} VintedVintedScraperHealthCheckHead(ctx).Execute()

Vinted scraper health check



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
	resp, r, err := apiClient.VintedAPI.VintedVintedScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VintedAPI.VintedVintedScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VintedVintedScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `VintedAPI.VintedVintedScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiVintedVintedScraperHealthCheckHeadRequest struct via the builder pattern


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


# \WallapopAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**WallapopAutocomplete**](WallapopAPI.md#WallapopAutocomplete) | **Get** /v1/wallapop/autocomplete | Autocomplete
[**WallapopGetListingDetail**](WallapopAPI.md#WallapopGetListingDetail) | **Get** /v1/wallapop/items/{item_id} | Get listing detail
[**WallapopGetUserListings**](WallapopAPI.md#WallapopGetUserListings) | **Get** /v1/wallapop/users/{user_id}/items | Get user listings
[**WallapopGetUserProfile**](WallapopAPI.md#WallapopGetUserProfile) | **Get** /v1/wallapop/users/{user_id} | Get user profile
[**WallapopGetUserReviews**](WallapopAPI.md#WallapopGetUserReviews) | **Get** /v1/wallapop/users/{user_id}/reviews | Get user reviews
[**WallapopListCategories**](WallapopAPI.md#WallapopListCategories) | **Get** /v1/wallapop/categories | List categories
[**WallapopListFilterOptions**](WallapopAPI.md#WallapopListFilterOptions) | **Get** /v1/wallapop/filters/{filter_id}/options | List filter options
[**WallapopListMarkets**](WallapopAPI.md#WallapopListMarkets) | **Get** /v1/wallapop/markets | List markets
[**WallapopListSearchFilters**](WallapopAPI.md#WallapopListSearchFilters) | **Get** /v1/wallapop/filters | List search filters
[**WallapopSearchListings**](WallapopAPI.md#WallapopSearchListings) | **Get** /v1/wallapop/search | Search listings
[**WallapopWallapopScraperHealthCheck**](WallapopAPI.md#WallapopWallapopScraperHealthCheck) | **Get** /v1/wallapop/health | Wallapop scraper health check
[**WallapopWallapopScraperHealthCheckHead**](WallapopAPI.md#WallapopWallapopScraperHealthCheckHead) | **Head** /v1/wallapop/health | Wallapop scraper health check



## WallapopAutocomplete

> interface{} WallapopAutocomplete(ctx).Query(query).Market(market).Execute()

Autocomplete



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
	query := "query_example" // string | Partial search text, e.g. 'bici'
	market := "market_example" // string | Market: es (Spain), it (Italy), pt (Portugal) (optional) (default to "es")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WallapopAPI.WallapopAutocomplete(context.Background()).Query(query).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WallapopAPI.WallapopAutocomplete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WallapopAutocomplete`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WallapopAPI.WallapopAutocomplete`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWallapopAutocompleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Partial search text, e.g. &#39;bici&#39; | 
 **market** | **string** | Market: es (Spain), it (Italy), pt (Portugal) | [default to &quot;es&quot;]

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


## WallapopGetListingDetail

> interface{} WallapopGetListingDetail(ctx, itemId).Market(market).Execute()

Get listing detail



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
	market := "market_example" // string | Market: es (Spain), it (Italy), pt (Portugal) (optional) (default to "es")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WallapopAPI.WallapopGetListingDetail(context.Background(), itemId).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WallapopAPI.WallapopGetListingDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WallapopGetListingDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WallapopAPI.WallapopGetListingDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**itemId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWallapopGetListingDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | Market: es (Spain), it (Italy), pt (Portugal) | [default to &quot;es&quot;]

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


## WallapopGetUserListings

> interface{} WallapopGetUserListings(ctx, userId).Market(market).NextPage(nextPage).Execute()

Get user listings



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
	userId := "userId_example" // string | 
	market := "market_example" // string | Market: es (Spain), it (Italy), pt (Portugal) (optional) (default to "es")
	nextPage := "nextPage_example" // string | Cursor from the previous page's next_page (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WallapopAPI.WallapopGetUserListings(context.Background(), userId).Market(market).NextPage(nextPage).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WallapopAPI.WallapopGetUserListings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WallapopGetUserListings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WallapopAPI.WallapopGetUserListings`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWallapopGetUserListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | Market: es (Spain), it (Italy), pt (Portugal) | [default to &quot;es&quot;]
 **nextPage** | **string** | Cursor from the previous page&#39;s next_page | 

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


## WallapopGetUserProfile

> interface{} WallapopGetUserProfile(ctx, userId).Market(market).Execute()

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
	userId := "userId_example" // string | 
	market := "market_example" // string | Market: es (Spain), it (Italy), pt (Portugal) (optional) (default to "es")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WallapopAPI.WallapopGetUserProfile(context.Background(), userId).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WallapopAPI.WallapopGetUserProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WallapopGetUserProfile`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WallapopAPI.WallapopGetUserProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWallapopGetUserProfileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | Market: es (Spain), it (Italy), pt (Portugal) | [default to &quot;es&quot;]

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


## WallapopGetUserReviews

> interface{} WallapopGetUserReviews(ctx, userId).Market(market).NextPage(nextPage).Execute()

Get user reviews



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
	userId := "userId_example" // string | 
	market := "market_example" // string | Market: es (Spain), it (Italy), pt (Portugal) (optional) (default to "es")
	nextPage := "nextPage_example" // string | Cursor from the previous page's next_page (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WallapopAPI.WallapopGetUserReviews(context.Background(), userId).Market(market).NextPage(nextPage).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WallapopAPI.WallapopGetUserReviews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WallapopGetUserReviews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WallapopAPI.WallapopGetUserReviews`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWallapopGetUserReviewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | Market: es (Spain), it (Italy), pt (Portugal) | [default to &quot;es&quot;]
 **nextPage** | **string** | Cursor from the previous page&#39;s next_page | 

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


## WallapopListCategories

> interface{} WallapopListCategories(ctx).Market(market).Execute()

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
	market := "market_example" // string | Market: es (Spain), it (Italy), pt (Portugal) (optional) (default to "es")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WallapopAPI.WallapopListCategories(context.Background()).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WallapopAPI.WallapopListCategories``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WallapopListCategories`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WallapopAPI.WallapopListCategories`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWallapopListCategoriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **market** | **string** | Market: es (Spain), it (Italy), pt (Portugal) | [default to &quot;es&quot;]

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


## WallapopListFilterOptions

> interface{} WallapopListFilterOptions(ctx, filterId).CategoryId(categoryId).Query(query).Market(market).Execute()

List filter options



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
	filterId := "filterId_example" // string | 
	categoryId := int32(56) // int32 | Category to scope options to (optional)
	query := "query_example" // string | Search text to scope options to (optional)
	market := "market_example" // string | Market: es (Spain), it (Italy), pt (Portugal) (optional) (default to "es")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WallapopAPI.WallapopListFilterOptions(context.Background(), filterId).CategoryId(categoryId).Query(query).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WallapopAPI.WallapopListFilterOptions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WallapopListFilterOptions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WallapopAPI.WallapopListFilterOptions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**filterId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWallapopListFilterOptionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **categoryId** | **int32** | Category to scope options to | 
 **query** | **string** | Search text to scope options to | 
 **market** | **string** | Market: es (Spain), it (Italy), pt (Portugal) | [default to &quot;es&quot;]

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


## WallapopListMarkets

> interface{} WallapopListMarkets(ctx).Execute()

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
	resp, r, err := apiClient.WallapopAPI.WallapopListMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WallapopAPI.WallapopListMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WallapopListMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WallapopAPI.WallapopListMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiWallapopListMarketsRequest struct via the builder pattern


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


## WallapopListSearchFilters

> interface{} WallapopListSearchFilters(ctx).CategoryId(categoryId).Query(query).Market(market).Execute()

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
	categoryId := int32(56) // int32 | Category the filters apply to (optional)
	query := "query_example" // string | Search text the filters apply to (optional)
	market := "market_example" // string | Market: es (Spain), it (Italy), pt (Portugal) (optional) (default to "es")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WallapopAPI.WallapopListSearchFilters(context.Background()).CategoryId(categoryId).Query(query).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WallapopAPI.WallapopListSearchFilters``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WallapopListSearchFilters`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WallapopAPI.WallapopListSearchFilters`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWallapopListSearchFiltersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **categoryId** | **int32** | Category the filters apply to | 
 **query** | **string** | Search text the filters apply to | 
 **market** | **string** | Market: es (Spain), it (Italy), pt (Portugal) | [default to &quot;es&quot;]

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


## WallapopSearchListings

> interface{} WallapopSearchListings(ctx).Query(query).Market(market).Latitude(latitude).Longitude(longitude).DistanceKm(distanceKm).CategoryId(categoryId).MinPrice(minPrice).MaxPrice(maxPrice).Condition(condition).Brand(brand).Model(model).Color(color).TimeFilter(timeFilter).Shippable(shippable).HasWarranty(hasWarranty).Refurbished(refurbished).MinYear(minYear).MaxYear(maxYear).MinKm(minKm).MaxKm(maxKm).Gearbox(gearbox).MinHorsepower(minHorsepower).MaxHorsepower(maxHorsepower).OrderBy(orderBy).NextPage(nextPage).Execute()

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
	query := "query_example" // string | Search text, e.g. 'iphone 14' (optional)
	market := "market_example" // string | Market: es (Spain), it (Italy), pt (Portugal) (optional) (default to "es")
	latitude := float32(8.14) // float32 | Search centre latitude (defaults to the market capital) (optional)
	longitude := float32(8.14) // float32 | Search centre longitude (optional)
	distanceKm := int32(56) // int32 | Search radius (optional)
	categoryId := int32(56) // int32 | Category id from /categories (optional)
	minPrice := float32(8.14) // float32 | Minimum price (EUR) (optional)
	maxPrice := float32(8.14) // float32 | Maximum price (EUR) (optional)
	condition := "condition_example" // string | Comma-separated: un_opened, in_box, new, as_good_as_new, good, fair, has_given_it_all (optional)
	brand := "brand_example" // string | Brand, e.g. Apple (optional)
	model := "model_example" // string | Model, e.g. iPhone 14 (optional)
	color := "color_example" // string | Colour id, e.g. black (optional)
	timeFilter := "timeFilter_example" // string | Only listings published within this window (optional)
	shippable := true // bool | Only listings that ship (optional) (default to false)
	hasWarranty := true // bool | Only listings with a warranty (optional) (default to false)
	refurbished := true // bool | Only refurbished listings (optional) (default to false)
	minYear := int32(56) // int32 | Cars: earliest model year (optional)
	maxYear := int32(56) // int32 | Cars: latest model year (optional)
	minKm := int32(56) // int32 | Cars: minimum mileage (optional)
	maxKm := int32(56) // int32 | Cars: maximum mileage (optional)
	gearbox := "gearbox_example" // string | Cars (optional)
	minHorsepower := int32(56) // int32 | Cars: minimum power (optional)
	maxHorsepower := int32(56) // int32 | Cars: maximum power (optional)
	orderBy := "orderBy_example" // string | Sort order (optional) (default to "most_relevance")
	nextPage := "nextPage_example" // string | Cursor from the previous page's next_page; other parameters are then ignored (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WallapopAPI.WallapopSearchListings(context.Background()).Query(query).Market(market).Latitude(latitude).Longitude(longitude).DistanceKm(distanceKm).CategoryId(categoryId).MinPrice(minPrice).MaxPrice(maxPrice).Condition(condition).Brand(brand).Model(model).Color(color).TimeFilter(timeFilter).Shippable(shippable).HasWarranty(hasWarranty).Refurbished(refurbished).MinYear(minYear).MaxYear(maxYear).MinKm(minKm).MaxKm(maxKm).Gearbox(gearbox).MinHorsepower(minHorsepower).MaxHorsepower(maxHorsepower).OrderBy(orderBy).NextPage(nextPage).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WallapopAPI.WallapopSearchListings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WallapopSearchListings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WallapopAPI.WallapopSearchListings`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWallapopSearchListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search text, e.g. &#39;iphone 14&#39; | 
 **market** | **string** | Market: es (Spain), it (Italy), pt (Portugal) | [default to &quot;es&quot;]
 **latitude** | **float32** | Search centre latitude (defaults to the market capital) | 
 **longitude** | **float32** | Search centre longitude | 
 **distanceKm** | **int32** | Search radius | 
 **categoryId** | **int32** | Category id from /categories | 
 **minPrice** | **float32** | Minimum price (EUR) | 
 **maxPrice** | **float32** | Maximum price (EUR) | 
 **condition** | **string** | Comma-separated: un_opened, in_box, new, as_good_as_new, good, fair, has_given_it_all | 
 **brand** | **string** | Brand, e.g. Apple | 
 **model** | **string** | Model, e.g. iPhone 14 | 
 **color** | **string** | Colour id, e.g. black | 
 **timeFilter** | **string** | Only listings published within this window | 
 **shippable** | **bool** | Only listings that ship | [default to false]
 **hasWarranty** | **bool** | Only listings with a warranty | [default to false]
 **refurbished** | **bool** | Only refurbished listings | [default to false]
 **minYear** | **int32** | Cars: earliest model year | 
 **maxYear** | **int32** | Cars: latest model year | 
 **minKm** | **int32** | Cars: minimum mileage | 
 **maxKm** | **int32** | Cars: maximum mileage | 
 **gearbox** | **string** | Cars | 
 **minHorsepower** | **int32** | Cars: minimum power | 
 **maxHorsepower** | **int32** | Cars: maximum power | 
 **orderBy** | **string** | Sort order | [default to &quot;most_relevance&quot;]
 **nextPage** | **string** | Cursor from the previous page&#39;s next_page; other parameters are then ignored | 

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


## WallapopWallapopScraperHealthCheck

> interface{} WallapopWallapopScraperHealthCheck(ctx).Execute()

Wallapop scraper health check



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
	resp, r, err := apiClient.WallapopAPI.WallapopWallapopScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WallapopAPI.WallapopWallapopScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WallapopWallapopScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WallapopAPI.WallapopWallapopScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiWallapopWallapopScraperHealthCheckRequest struct via the builder pattern


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


## WallapopWallapopScraperHealthCheckHead

> interface{} WallapopWallapopScraperHealthCheckHead(ctx).Execute()

Wallapop scraper health check



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
	resp, r, err := apiClient.WallapopAPI.WallapopWallapopScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WallapopAPI.WallapopWallapopScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WallapopWallapopScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `WallapopAPI.WallapopWallapopScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiWallapopWallapopScraperHealthCheckHeadRequest struct via the builder pattern


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


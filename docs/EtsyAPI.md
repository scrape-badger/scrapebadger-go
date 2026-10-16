# \EtsyAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**EtsyGetCategories**](EtsyAPI.md#EtsyGetCategories) | **Get** /v1/etsy/categories | Get categories
[**EtsyGetListingDetail**](EtsyAPI.md#EtsyGetListingDetail) | **Get** /v1/etsy/listings/{listing_id} | Get listing detail
[**EtsyGetListingReviews**](EtsyAPI.md#EtsyGetListingReviews) | **Get** /v1/etsy/listings/{listing_id}/reviews | Get listing reviews
[**EtsyGetSearchSuggestions**](EtsyAPI.md#EtsyGetSearchSuggestions) | **Get** /v1/etsy/autocomplete | Get search suggestions
[**EtsyGetShopListings**](EtsyAPI.md#EtsyGetShopListings) | **Get** /v1/etsy/shops/{shop_name}/listings | Get shop listings
[**EtsyGetShopProfile**](EtsyAPI.md#EtsyGetShopProfile) | **Get** /v1/etsy/shops/{shop_name} | Get shop profile
[**EtsyGetShopReviews**](EtsyAPI.md#EtsyGetShopReviews) | **Get** /v1/etsy/shops/{shop_name}/reviews | Get shop reviews
[**EtsySearchListings**](EtsyAPI.md#EtsySearchListings) | **Get** /v1/etsy/search | Search listings



## EtsyGetCategories

> interface{} EtsyGetCategories(ctx).Country(country).Currency(currency).Language(language).Execute()

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
	country := "country_example" // string |  (optional) (default to "US")
	currency := "currency_example" // string |  (optional) (default to "USD")
	language := "language_example" // string |  (optional) (default to "en-US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EtsyAPI.EtsyGetCategories(context.Background()).Country(country).Currency(currency).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EtsyAPI.EtsyGetCategories``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EtsyGetCategories`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EtsyAPI.EtsyGetCategories`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiEtsyGetCategoriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **country** | **string** |  | [default to &quot;US&quot;]
 **currency** | **string** |  | [default to &quot;USD&quot;]
 **language** | **string** |  | [default to &quot;en-US&quot;]

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


## EtsyGetListingDetail

> interface{} EtsyGetListingDetail(ctx, listingId).Country(country).Currency(currency).Language(language).Execute()

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
	listingId := "listingId_example" // string | 
	country := "country_example" // string |  (optional) (default to "US")
	currency := "currency_example" // string |  (optional) (default to "USD")
	language := "language_example" // string |  (optional) (default to "en-US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EtsyAPI.EtsyGetListingDetail(context.Background(), listingId).Country(country).Currency(currency).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EtsyAPI.EtsyGetListingDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EtsyGetListingDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EtsyAPI.EtsyGetListingDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listingId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiEtsyGetListingDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** |  | [default to &quot;US&quot;]
 **currency** | **string** |  | [default to &quot;USD&quot;]
 **language** | **string** |  | [default to &quot;en-US&quot;]

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


## EtsyGetListingReviews

> interface{} EtsyGetListingReviews(ctx, listingId).Page(page).Sort(sort).Country(country).Currency(currency).Language(language).Execute()

Get listing reviews

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
	listingId := "listingId_example" // string | 
	page := int32(56) // int32 |  (optional) (default to 1)
	sort := "sort_example" // string |  (optional) (default to "Relevancy")
	country := "country_example" // string |  (optional) (default to "US")
	currency := "currency_example" // string |  (optional) (default to "USD")
	language := "language_example" // string |  (optional) (default to "en-US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EtsyAPI.EtsyGetListingReviews(context.Background(), listingId).Page(page).Sort(sort).Country(country).Currency(currency).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EtsyAPI.EtsyGetListingReviews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EtsyGetListingReviews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EtsyAPI.EtsyGetListingReviews`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listingId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiEtsyGetListingReviewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** |  | [default to 1]
 **sort** | **string** |  | [default to &quot;Relevancy&quot;]
 **country** | **string** |  | [default to &quot;US&quot;]
 **currency** | **string** |  | [default to &quot;USD&quot;]
 **language** | **string** |  | [default to &quot;en-US&quot;]

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


## EtsyGetSearchSuggestions

> interface{} EtsyGetSearchSuggestions(ctx).Query(query).Country(country).Currency(currency).Language(language).Execute()

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
	currency := "currency_example" // string |  (optional) (default to "USD")
	language := "language_example" // string |  (optional) (default to "en-US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EtsyAPI.EtsyGetSearchSuggestions(context.Background()).Query(query).Country(country).Currency(currency).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EtsyAPI.EtsyGetSearchSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EtsyGetSearchSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EtsyAPI.EtsyGetSearchSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiEtsyGetSearchSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 
 **country** | **string** |  | [default to &quot;US&quot;]
 **currency** | **string** |  | [default to &quot;USD&quot;]
 **language** | **string** |  | [default to &quot;en-US&quot;]

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


## EtsyGetShopListings

> interface{} EtsyGetShopListings(ctx, shopName).Page(page).Country(country).Currency(currency).Language(language).Execute()

Get shop listings

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
	shopName := "shopName_example" // string | 
	page := int32(56) // int32 |  (optional) (default to 1)
	country := "country_example" // string |  (optional) (default to "US")
	currency := "currency_example" // string |  (optional) (default to "USD")
	language := "language_example" // string |  (optional) (default to "en-US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EtsyAPI.EtsyGetShopListings(context.Background(), shopName).Page(page).Country(country).Currency(currency).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EtsyAPI.EtsyGetShopListings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EtsyGetShopListings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EtsyAPI.EtsyGetShopListings`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopName** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiEtsyGetShopListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** |  | [default to 1]
 **country** | **string** |  | [default to &quot;US&quot;]
 **currency** | **string** |  | [default to &quot;USD&quot;]
 **language** | **string** |  | [default to &quot;en-US&quot;]

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


## EtsyGetShopProfile

> interface{} EtsyGetShopProfile(ctx, shopName).Country(country).Currency(currency).Language(language).Execute()

Get shop profile

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
	shopName := "shopName_example" // string | 
	country := "country_example" // string |  (optional) (default to "US")
	currency := "currency_example" // string |  (optional) (default to "USD")
	language := "language_example" // string |  (optional) (default to "en-US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EtsyAPI.EtsyGetShopProfile(context.Background(), shopName).Country(country).Currency(currency).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EtsyAPI.EtsyGetShopProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EtsyGetShopProfile`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EtsyAPI.EtsyGetShopProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopName** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiEtsyGetShopProfileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** |  | [default to &quot;US&quot;]
 **currency** | **string** |  | [default to &quot;USD&quot;]
 **language** | **string** |  | [default to &quot;en-US&quot;]

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


## EtsyGetShopReviews

> interface{} EtsyGetShopReviews(ctx, shopName).Page(page).Country(country).Currency(currency).Language(language).Execute()

Get shop reviews

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
	shopName := "shopName_example" // string | 
	page := int32(56) // int32 |  (optional) (default to 1)
	country := "country_example" // string |  (optional) (default to "US")
	currency := "currency_example" // string |  (optional) (default to "USD")
	language := "language_example" // string |  (optional) (default to "en-US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EtsyAPI.EtsyGetShopReviews(context.Background(), shopName).Page(page).Country(country).Currency(currency).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EtsyAPI.EtsyGetShopReviews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EtsyGetShopReviews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EtsyAPI.EtsyGetShopReviews`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**shopName** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiEtsyGetShopReviewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** |  | [default to 1]
 **country** | **string** |  | [default to &quot;US&quot;]
 **currency** | **string** |  | [default to &quot;USD&quot;]
 **language** | **string** |  | [default to &quot;en-US&quot;]

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


## EtsySearchListings

> interface{} EtsySearchListings(ctx).Query(query).Page(page).Country(country).Currency(currency).Language(language).Sort(sort).MinPrice(minPrice).MaxPrice(maxPrice).Execute()

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
	query := "query_example" // string | 
	page := int32(56) // int32 |  (optional) (default to 1)
	country := "country_example" // string |  (optional) (default to "US")
	currency := "currency_example" // string |  (optional) (default to "USD")
	language := "language_example" // string |  (optional) (default to "en-US")
	sort := "sort_example" // string |  (optional) (default to "most_relevant")
	minPrice := float32(8.14) // float32 |  (optional)
	maxPrice := float32(8.14) // float32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EtsyAPI.EtsySearchListings(context.Background()).Query(query).Page(page).Country(country).Currency(currency).Language(language).Sort(sort).MinPrice(minPrice).MaxPrice(maxPrice).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EtsyAPI.EtsySearchListings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EtsySearchListings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `EtsyAPI.EtsySearchListings`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiEtsySearchListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 
 **page** | **int32** |  | [default to 1]
 **country** | **string** |  | [default to &quot;US&quot;]
 **currency** | **string** |  | [default to &quot;USD&quot;]
 **language** | **string** |  | [default to &quot;en-US&quot;]
 **sort** | **string** |  | [default to &quot;most_relevant&quot;]
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


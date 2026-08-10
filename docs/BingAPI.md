# \BingAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**BingBingScraperHealthCheck**](BingAPI.md#BingBingScraperHealthCheck) | **Get** /v1/bing/health | Bing scraper health check
[**BingBingScraperHealthCheckHead**](BingAPI.md#BingBingScraperHealthCheckHead) | **Head** /v1/bing/health | Bing scraper health check
[**BingImageSearch**](BingAPI.md#BingImageSearch) | **Get** /v1/bing/images | Image search
[**BingListSupportedMarkets**](BingAPI.md#BingListSupportedMarkets) | **Get** /v1/bing/markets | List supported markets
[**BingNewsSearch**](BingAPI.md#BingNewsSearch) | **Get** /v1/bing/news | News search
[**BingSearchSuggestions**](BingAPI.md#BingSearchSuggestions) | **Get** /v1/bing/autocomplete | Search suggestions
[**BingVideoSearch**](BingAPI.md#BingVideoSearch) | **Get** /v1/bing/videos | Video search
[**BingWebSearch**](BingAPI.md#BingWebSearch) | **Get** /v1/bing/search | Web search



## BingBingScraperHealthCheck

> interface{} BingBingScraperHealthCheck(ctx).Execute()

Bing scraper health check



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
	resp, r, err := apiClient.BingAPI.BingBingScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BingAPI.BingBingScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BingBingScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BingAPI.BingBingScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiBingBingScraperHealthCheckRequest struct via the builder pattern


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


## BingBingScraperHealthCheckHead

> interface{} BingBingScraperHealthCheckHead(ctx).Execute()

Bing scraper health check



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
	resp, r, err := apiClient.BingAPI.BingBingScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BingAPI.BingBingScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BingBingScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BingAPI.BingBingScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiBingBingScraperHealthCheckHeadRequest struct via the builder pattern


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


## BingImageSearch

> interface{} BingImageSearch(ctx).Query(query).Market(market).Count(count).SafeSearch(safeSearch).Execute()

Image search



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
	query := "query_example" // string | Search keywords, e.g. 'golden retriever'
	market := "market_example" // string | Bing market code, e.g. 'en-US', 'en-GB', 'de-DE'. See /markets. (optional) (default to "en-US")
	count := int32(56) // int32 | Results to return (optional) (default to 35)
	safeSearch := "safeSearch_example" // string | off | moderate | strict (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BingAPI.BingImageSearch(context.Background()).Query(query).Market(market).Count(count).SafeSearch(safeSearch).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BingAPI.BingImageSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BingImageSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BingAPI.BingImageSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBingImageSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords, e.g. &#39;golden retriever&#39; | 
 **market** | **string** | Bing market code, e.g. &#39;en-US&#39;, &#39;en-GB&#39;, &#39;de-DE&#39;. See /markets. | [default to &quot;en-US&quot;]
 **count** | **int32** | Results to return | [default to 35]
 **safeSearch** | **string** | off | moderate | strict | 

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


## BingListSupportedMarkets

> interface{} BingListSupportedMarkets(ctx).Execute()

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
	resp, r, err := apiClient.BingAPI.BingListSupportedMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BingAPI.BingListSupportedMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BingListSupportedMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BingAPI.BingListSupportedMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiBingListSupportedMarketsRequest struct via the builder pattern


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


## BingNewsSearch

> interface{} BingNewsSearch(ctx).Query(query).Market(market).Freshness(freshness).Execute()

News search



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
	query := "query_example" // string | Search keywords, e.g. 'interest rates'
	market := "market_example" // string | Bing market code, e.g. 'en-US', 'en-GB', 'de-DE'. See /markets. (optional) (default to "en-US")
	freshness := "freshness_example" // string | day | week | month — restrict to recent articles (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BingAPI.BingNewsSearch(context.Background()).Query(query).Market(market).Freshness(freshness).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BingAPI.BingNewsSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BingNewsSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BingAPI.BingNewsSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBingNewsSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords, e.g. &#39;interest rates&#39; | 
 **market** | **string** | Bing market code, e.g. &#39;en-US&#39;, &#39;en-GB&#39;, &#39;de-DE&#39;. See /markets. | [default to &quot;en-US&quot;]
 **freshness** | **string** | day | week | month — restrict to recent articles | 

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


## BingSearchSuggestions

> interface{} BingSearchSuggestions(ctx).Query(query).Market(market).Execute()

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
	query := "query_example" // string | Partial search term, e.g. 'coff'
	market := "market_example" // string | Bing market code, e.g. 'en-US', 'en-GB', 'de-DE'. See /markets. (optional) (default to "en-US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BingAPI.BingSearchSuggestions(context.Background()).Query(query).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BingAPI.BingSearchSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BingSearchSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BingAPI.BingSearchSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBingSearchSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Partial search term, e.g. &#39;coff&#39; | 
 **market** | **string** | Bing market code, e.g. &#39;en-US&#39;, &#39;en-GB&#39;, &#39;de-DE&#39;. See /markets. | [default to &quot;en-US&quot;]

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


## BingVideoSearch

> interface{} BingVideoSearch(ctx).Query(query).Market(market).Count(count).SafeSearch(safeSearch).Execute()

Video search



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
	query := "query_example" // string | Search keywords, e.g. 'espresso tutorial'
	market := "market_example" // string | Bing market code, e.g. 'en-US', 'en-GB', 'de-DE'. See /markets. (optional) (default to "en-US")
	count := int32(56) // int32 | Results to return (optional) (default to 35)
	safeSearch := "safeSearch_example" // string | off | moderate | strict (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BingAPI.BingVideoSearch(context.Background()).Query(query).Market(market).Count(count).SafeSearch(safeSearch).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BingAPI.BingVideoSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BingVideoSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BingAPI.BingVideoSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBingVideoSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords, e.g. &#39;espresso tutorial&#39; | 
 **market** | **string** | Bing market code, e.g. &#39;en-US&#39;, &#39;en-GB&#39;, &#39;de-DE&#39;. See /markets. | [default to &quot;en-US&quot;]
 **count** | **int32** | Results to return | [default to 35]
 **safeSearch** | **string** | off | moderate | strict | 

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


## BingWebSearch

> interface{} BingWebSearch(ctx).Query(query).Market(market).Count(count).Offset(offset).SafeSearch(safeSearch).Execute()

Web search



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
	query := "query_example" // string | Search keywords, e.g. 'coffee machine'
	market := "market_example" // string | Bing market code, e.g. 'en-US', 'en-GB', 'de-DE'. See /markets. (optional) (default to "en-US")
	count := int32(56) // int32 | Results per page (1-50) (optional) (default to 10)
	offset := int32(56) // int32 | Zero-based result offset for pagination (optional) (default to 0)
	safeSearch := "safeSearch_example" // string | off | moderate | strict (default moderate) (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BingAPI.BingWebSearch(context.Background()).Query(query).Market(market).Count(count).Offset(offset).SafeSearch(safeSearch).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BingAPI.BingWebSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BingWebSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BingAPI.BingWebSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBingWebSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords, e.g. &#39;coffee machine&#39; | 
 **market** | **string** | Bing market code, e.g. &#39;en-US&#39;, &#39;en-GB&#39;, &#39;de-DE&#39;. See /markets. | [default to &quot;en-US&quot;]
 **count** | **int32** | Results per page (1-50) | [default to 10]
 **offset** | **int32** | Zero-based result offset for pagination | [default to 0]
 **safeSearch** | **string** | off | moderate | strict (default moderate) | 

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


# \YahooAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**YahooImageSearch**](YahooAPI.md#YahooImageSearch) | **Get** /v1/yahoo/images | Image search
[**YahooListSupportedMarkets**](YahooAPI.md#YahooListSupportedMarkets) | **Get** /v1/yahoo/markets | List supported markets
[**YahooNewsSearch**](YahooAPI.md#YahooNewsSearch) | **Get** /v1/yahoo/news | News search
[**YahooSearchSuggestions**](YahooAPI.md#YahooSearchSuggestions) | **Get** /v1/yahoo/autocomplete | Search suggestions
[**YahooVideoSearch**](YahooAPI.md#YahooVideoSearch) | **Get** /v1/yahoo/videos | Video search
[**YahooWebSearch**](YahooAPI.md#YahooWebSearch) | **Get** /v1/yahoo/search | Web search
[**YahooYahooScraperHealthCheck**](YahooAPI.md#YahooYahooScraperHealthCheck) | **Get** /v1/yahoo/health | Yahoo scraper health check
[**YahooYahooScraperHealthCheckHead**](YahooAPI.md#YahooYahooScraperHealthCheckHead) | **Head** /v1/yahoo/health | Yahoo scraper health check



## YahooImageSearch

> interface{} YahooImageSearch(ctx).Query(query).Market(market).Count(count).Execute()

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
	market := "market_example" // string | Yahoo market code, e.g. 'us', 'uk', 'fr', 'de'. See /markets. (optional) (default to "us")
	count := int32(56) // int32 | Results to return (optional) (default to 30)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YahooAPI.YahooImageSearch(context.Background()).Query(query).Market(market).Count(count).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YahooAPI.YahooImageSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YahooImageSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YahooAPI.YahooImageSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiYahooImageSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords, e.g. &#39;golden retriever&#39; | 
 **market** | **string** | Yahoo market code, e.g. &#39;us&#39;, &#39;uk&#39;, &#39;fr&#39;, &#39;de&#39;. See /markets. | [default to &quot;us&quot;]
 **count** | **int32** | Results to return | [default to 30]

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


## YahooListSupportedMarkets

> interface{} YahooListSupportedMarkets(ctx).Execute()

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
	resp, r, err := apiClient.YahooAPI.YahooListSupportedMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YahooAPI.YahooListSupportedMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YahooListSupportedMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YahooAPI.YahooListSupportedMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiYahooListSupportedMarketsRequest struct via the builder pattern


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


## YahooNewsSearch

> interface{} YahooNewsSearch(ctx).Query(query).Market(market).Execute()

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
	market := "market_example" // string | Yahoo market code, e.g. 'us', 'uk', 'fr', 'de'. See /markets. (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YahooAPI.YahooNewsSearch(context.Background()).Query(query).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YahooAPI.YahooNewsSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YahooNewsSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YahooAPI.YahooNewsSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiYahooNewsSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords, e.g. &#39;interest rates&#39; | 
 **market** | **string** | Yahoo market code, e.g. &#39;us&#39;, &#39;uk&#39;, &#39;fr&#39;, &#39;de&#39;. See /markets. | [default to &quot;us&quot;]

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


## YahooSearchSuggestions

> interface{} YahooSearchSuggestions(ctx).Query(query).Market(market).Execute()

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
	market := "market_example" // string | Yahoo market code, e.g. 'us', 'uk', 'fr', 'de'. See /markets. (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YahooAPI.YahooSearchSuggestions(context.Background()).Query(query).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YahooAPI.YahooSearchSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YahooSearchSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YahooAPI.YahooSearchSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiYahooSearchSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Partial search term, e.g. &#39;coff&#39; | 
 **market** | **string** | Yahoo market code, e.g. &#39;us&#39;, &#39;uk&#39;, &#39;fr&#39;, &#39;de&#39;. See /markets. | [default to &quot;us&quot;]

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


## YahooVideoSearch

> interface{} YahooVideoSearch(ctx).Query(query).Market(market).Count(count).Execute()

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
	market := "market_example" // string | Yahoo market code, e.g. 'us', 'uk', 'fr', 'de'. See /markets. (optional) (default to "us")
	count := int32(56) // int32 | Results to return (optional) (default to 30)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YahooAPI.YahooVideoSearch(context.Background()).Query(query).Market(market).Count(count).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YahooAPI.YahooVideoSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YahooVideoSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YahooAPI.YahooVideoSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiYahooVideoSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords, e.g. &#39;espresso tutorial&#39; | 
 **market** | **string** | Yahoo market code, e.g. &#39;us&#39;, &#39;uk&#39;, &#39;fr&#39;, &#39;de&#39;. See /markets. | [default to &quot;us&quot;]
 **count** | **int32** | Results to return | [default to 30]

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


## YahooWebSearch

> interface{} YahooWebSearch(ctx).Query(query).Market(market).Offset(offset).SafeSearch(safeSearch).Execute()

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
	market := "market_example" // string | Yahoo market code, e.g. 'us', 'uk', 'fr', 'de'. See /markets. (optional) (default to "us")
	offset := int32(56) // int32 | Zero-based result offset for pagination (optional) (default to 0)
	safeSearch := "safeSearch_example" // string | off | moderate | strict (default moderate) (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YahooAPI.YahooWebSearch(context.Background()).Query(query).Market(market).Offset(offset).SafeSearch(safeSearch).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YahooAPI.YahooWebSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YahooWebSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YahooAPI.YahooWebSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiYahooWebSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords, e.g. &#39;coffee machine&#39; | 
 **market** | **string** | Yahoo market code, e.g. &#39;us&#39;, &#39;uk&#39;, &#39;fr&#39;, &#39;de&#39;. See /markets. | [default to &quot;us&quot;]
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


## YahooYahooScraperHealthCheck

> interface{} YahooYahooScraperHealthCheck(ctx).Execute()

Yahoo scraper health check



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
	resp, r, err := apiClient.YahooAPI.YahooYahooScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YahooAPI.YahooYahooScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YahooYahooScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YahooAPI.YahooYahooScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiYahooYahooScraperHealthCheckRequest struct via the builder pattern


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


## YahooYahooScraperHealthCheckHead

> interface{} YahooYahooScraperHealthCheckHead(ctx).Execute()

Yahoo scraper health check



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
	resp, r, err := apiClient.YahooAPI.YahooYahooScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YahooAPI.YahooYahooScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YahooYahooScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YahooAPI.YahooYahooScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiYahooYahooScraperHealthCheckHeadRequest struct via the builder pattern


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


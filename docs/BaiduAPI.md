# \BaiduAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**BaiduBaiduImageSearch**](BaiduAPI.md#BaiduBaiduImageSearch) | **Get** /v1/baidu/images | Baidu image search
[**BaiduBaiduNewsSearch**](BaiduAPI.md#BaiduBaiduNewsSearch) | **Get** /v1/baidu/news | Baidu news search
[**BaiduBaiduScraperHealthCheck**](BaiduAPI.md#BaiduBaiduScraperHealthCheck) | **Get** /v1/baidu/health | Baidu scraper health check
[**BaiduBaiduScraperHealthCheckHead**](BaiduAPI.md#BaiduBaiduScraperHealthCheckHead) | **Head** /v1/baidu/health | Baidu scraper health check
[**BaiduBaiduWebSearch**](BaiduAPI.md#BaiduBaiduWebSearch) | **Get** /v1/baidu/search | Baidu web search
[**BaiduSearchSuggestions**](BaiduAPI.md#BaiduSearchSuggestions) | **Get** /v1/baidu/autocomplete | Search suggestions



## BaiduBaiduImageSearch

> interface{} BaiduBaiduImageSearch(ctx).Query(query).Page(page).Execute()

Baidu image search



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
	query := "query_example" // string | Search keywords
	page := int32(56) // int32 | 30 images per page (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BaiduAPI.BaiduBaiduImageSearch(context.Background()).Query(query).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BaiduAPI.BaiduBaiduImageSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BaiduBaiduImageSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BaiduAPI.BaiduBaiduImageSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBaiduBaiduImageSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords | 
 **page** | **int32** | 30 images per page | [default to 1]

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


## BaiduBaiduNewsSearch

> interface{} BaiduBaiduNewsSearch(ctx).Query(query).Page(page).Execute()

Baidu news search



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
	query := "query_example" // string | Search keywords
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BaiduAPI.BaiduBaiduNewsSearch(context.Background()).Query(query).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BaiduAPI.BaiduBaiduNewsSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BaiduBaiduNewsSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BaiduAPI.BaiduBaiduNewsSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBaiduBaiduNewsSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords | 
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


## BaiduBaiduScraperHealthCheck

> interface{} BaiduBaiduScraperHealthCheck(ctx).Execute()

Baidu scraper health check



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
	resp, r, err := apiClient.BaiduAPI.BaiduBaiduScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BaiduAPI.BaiduBaiduScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BaiduBaiduScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BaiduAPI.BaiduBaiduScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiBaiduBaiduScraperHealthCheckRequest struct via the builder pattern


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


## BaiduBaiduScraperHealthCheckHead

> interface{} BaiduBaiduScraperHealthCheckHead(ctx).Execute()

Baidu scraper health check



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
	resp, r, err := apiClient.BaiduAPI.BaiduBaiduScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BaiduAPI.BaiduBaiduScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BaiduBaiduScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BaiduAPI.BaiduBaiduScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiBaiduBaiduScraperHealthCheckHeadRequest struct via the builder pattern


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


## BaiduBaiduWebSearch

> interface{} BaiduBaiduWebSearch(ctx).Query(query).Page(page).Num(num).Execute()

Baidu web search



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
	query := "query_example" // string | Search keywords, e.g. '咖啡机' or 'coffee machine'
	page := int32(56) // int32 | Result page (10 results per page) (optional) (default to 1)
	num := int32(56) // int32 | Results per page (rn) (optional) (default to 10)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BaiduAPI.BaiduBaiduWebSearch(context.Background()).Query(query).Page(page).Num(num).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BaiduAPI.BaiduBaiduWebSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BaiduBaiduWebSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BaiduAPI.BaiduBaiduWebSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBaiduBaiduWebSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords, e.g. &#39;咖啡机&#39; or &#39;coffee machine&#39; | 
 **page** | **int32** | Result page (10 results per page) | [default to 1]
 **num** | **int32** | Results per page (rn) | [default to 10]

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


## BaiduSearchSuggestions

> interface{} BaiduSearchSuggestions(ctx).Query(query).Execute()

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
	query := "query_example" // string | Partial search term, e.g. '咖啡' or 'coff'

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BaiduAPI.BaiduSearchSuggestions(context.Background()).Query(query).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BaiduAPI.BaiduSearchSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BaiduSearchSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BaiduAPI.BaiduSearchSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBaiduSearchSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Partial search term, e.g. &#39;咖啡&#39; or &#39;coff&#39; | 

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


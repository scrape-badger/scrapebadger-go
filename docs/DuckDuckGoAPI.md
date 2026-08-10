# \DuckDuckGoAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DuckduckgoDuckduckgoScraperHealthCheck**](DuckDuckGoAPI.md#DuckduckgoDuckduckgoScraperHealthCheck) | **Get** /v1/duckduckgo/health | DuckDuckGo scraper health check
[**DuckduckgoDuckduckgoScraperHealthCheckHead**](DuckDuckGoAPI.md#DuckduckgoDuckduckgoScraperHealthCheckHead) | **Head** /v1/duckduckgo/health | DuckDuckGo scraper health check
[**DuckduckgoImageSearch**](DuckDuckGoAPI.md#DuckduckgoImageSearch) | **Get** /v1/duckduckgo/images | Image search
[**DuckduckgoInstantAnswer**](DuckDuckGoAPI.md#DuckduckgoInstantAnswer) | **Get** /v1/duckduckgo/instant | Instant Answer
[**DuckduckgoListSupportedRegions**](DuckDuckGoAPI.md#DuckduckgoListSupportedRegions) | **Get** /v1/duckduckgo/regions | List supported regions
[**DuckduckgoNewsSearch**](DuckDuckGoAPI.md#DuckduckgoNewsSearch) | **Get** /v1/duckduckgo/news | News search
[**DuckduckgoSearchSuggestions**](DuckDuckGoAPI.md#DuckduckgoSearchSuggestions) | **Get** /v1/duckduckgo/autocomplete | Search suggestions
[**DuckduckgoVideoSearch**](DuckDuckGoAPI.md#DuckduckgoVideoSearch) | **Get** /v1/duckduckgo/videos | Video search
[**DuckduckgoWebSearch**](DuckDuckGoAPI.md#DuckduckgoWebSearch) | **Get** /v1/duckduckgo/search | Web search



## DuckduckgoDuckduckgoScraperHealthCheck

> interface{} DuckduckgoDuckduckgoScraperHealthCheck(ctx).Execute()

DuckDuckGo scraper health check



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
	resp, r, err := apiClient.DuckDuckGoAPI.DuckduckgoDuckduckgoScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DuckDuckGoAPI.DuckduckgoDuckduckgoScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DuckduckgoDuckduckgoScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DuckDuckGoAPI.DuckduckgoDuckduckgoScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiDuckduckgoDuckduckgoScraperHealthCheckRequest struct via the builder pattern


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


## DuckduckgoDuckduckgoScraperHealthCheckHead

> interface{} DuckduckgoDuckduckgoScraperHealthCheckHead(ctx).Execute()

DuckDuckGo scraper health check



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
	resp, r, err := apiClient.DuckDuckGoAPI.DuckduckgoDuckduckgoScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DuckDuckGoAPI.DuckduckgoDuckduckgoScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DuckduckgoDuckduckgoScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DuckDuckGoAPI.DuckduckgoDuckduckgoScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiDuckduckgoDuckduckgoScraperHealthCheckHeadRequest struct via the builder pattern


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


## DuckduckgoImageSearch

> interface{} DuckduckgoImageSearch(ctx).Query(query).Region(region).Safesearch(safesearch).Page(page).Size(size).Color(color).ImageType(imageType).Layout(layout).License(license).Execute()

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
	query := "query_example" // string | Search query
	region := "region_example" // string | DuckDuckGo region code (kl), e.g. us-en, uk-en, de-de. wt-wt = all regions. (optional) (default to "wt-wt")
	safesearch := "safesearch_example" // string | on | moderate | off (optional) (default to "moderate")
	page := int32(56) // int32 | 100 results per page (optional) (default to 1)
	size := "size_example" // string | Small | Medium | Large | Wallpaper (optional) (default to "")
	color := "color_example" // string | color | Monochrome | Red | Blue | … (optional) (default to "")
	imageType := "imageType_example" // string | photo | clipart | gif | transparent | line (optional) (default to "")
	layout := "layout_example" // string | Square | Tall | Wide (optional) (default to "")
	license := "license_example" // string | Any | Public | Share | ShareCommercially | Modify (optional) (default to "")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DuckDuckGoAPI.DuckduckgoImageSearch(context.Background()).Query(query).Region(region).Safesearch(safesearch).Page(page).Size(size).Color(color).ImageType(imageType).Layout(layout).License(license).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DuckDuckGoAPI.DuckduckgoImageSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DuckduckgoImageSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DuckDuckGoAPI.DuckduckgoImageSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiDuckduckgoImageSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search query | 
 **region** | **string** | DuckDuckGo region code (kl), e.g. us-en, uk-en, de-de. wt-wt &#x3D; all regions. | [default to &quot;wt-wt&quot;]
 **safesearch** | **string** | on | moderate | off | [default to &quot;moderate&quot;]
 **page** | **int32** | 100 results per page | [default to 1]
 **size** | **string** | Small | Medium | Large | Wallpaper | [default to &quot;&quot;]
 **color** | **string** | color | Monochrome | Red | Blue | … | [default to &quot;&quot;]
 **imageType** | **string** | photo | clipart | gif | transparent | line | [default to &quot;&quot;]
 **layout** | **string** | Square | Tall | Wide | [default to &quot;&quot;]
 **license** | **string** | Any | Public | Share | ShareCommercially | Modify | [default to &quot;&quot;]

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


## DuckduckgoInstantAnswer

> interface{} DuckduckgoInstantAnswer(ctx).Query(query).Execute()

Instant Answer



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
	query := "query_example" // string | Query for the Instant Answer API

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DuckDuckGoAPI.DuckduckgoInstantAnswer(context.Background()).Query(query).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DuckDuckGoAPI.DuckduckgoInstantAnswer``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DuckduckgoInstantAnswer`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DuckDuckGoAPI.DuckduckgoInstantAnswer`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiDuckduckgoInstantAnswerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Query for the Instant Answer API | 

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


## DuckduckgoListSupportedRegions

> interface{} DuckduckgoListSupportedRegions(ctx).Execute()

List supported regions



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
	resp, r, err := apiClient.DuckDuckGoAPI.DuckduckgoListSupportedRegions(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DuckDuckGoAPI.DuckduckgoListSupportedRegions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DuckduckgoListSupportedRegions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DuckDuckGoAPI.DuckduckgoListSupportedRegions`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiDuckduckgoListSupportedRegionsRequest struct via the builder pattern


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


## DuckduckgoNewsSearch

> interface{} DuckduckgoNewsSearch(ctx).Query(query).Region(region).Safesearch(safesearch).Timelimit(timelimit).Page(page).Execute()

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
	query := "query_example" // string | Search query
	region := "region_example" // string | DuckDuckGo region code (kl), e.g. us-en, uk-en, de-de. wt-wt = all regions. (optional) (default to "wt-wt")
	safesearch := "safesearch_example" // string | on | moderate | off (optional) (default to "moderate")
	timelimit := "timelimit_example" // string | day | week | month | year (optional) (default to "")
	page := int32(56) // int32 | 30 results per page (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DuckDuckGoAPI.DuckduckgoNewsSearch(context.Background()).Query(query).Region(region).Safesearch(safesearch).Timelimit(timelimit).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DuckDuckGoAPI.DuckduckgoNewsSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DuckduckgoNewsSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DuckDuckGoAPI.DuckduckgoNewsSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiDuckduckgoNewsSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search query | 
 **region** | **string** | DuckDuckGo region code (kl), e.g. us-en, uk-en, de-de. wt-wt &#x3D; all regions. | [default to &quot;wt-wt&quot;]
 **safesearch** | **string** | on | moderate | off | [default to &quot;moderate&quot;]
 **timelimit** | **string** | day | week | month | year | [default to &quot;&quot;]
 **page** | **int32** | 30 results per page | [default to 1]

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


## DuckduckgoSearchSuggestions

> interface{} DuckduckgoSearchSuggestions(ctx).Query(query).Region(region).Execute()

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
	query := "query_example" // string | Partial query to complete
	region := "region_example" // string | DuckDuckGo region code (kl), e.g. us-en, uk-en, de-de. wt-wt = all regions. (optional) (default to "wt-wt")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DuckDuckGoAPI.DuckduckgoSearchSuggestions(context.Background()).Query(query).Region(region).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DuckDuckGoAPI.DuckduckgoSearchSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DuckduckgoSearchSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DuckDuckGoAPI.DuckduckgoSearchSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiDuckduckgoSearchSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Partial query to complete | 
 **region** | **string** | DuckDuckGo region code (kl), e.g. us-en, uk-en, de-de. wt-wt &#x3D; all regions. | [default to &quot;wt-wt&quot;]

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


## DuckduckgoVideoSearch

> interface{} DuckduckgoVideoSearch(ctx).Query(query).Region(region).Safesearch(safesearch).Page(page).Duration(duration).Resolution(resolution).Execute()

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
	query := "query_example" // string | Search query
	region := "region_example" // string | DuckDuckGo region code (kl), e.g. us-en, uk-en, de-de. wt-wt = all regions. (optional) (default to "wt-wt")
	safesearch := "safesearch_example" // string | on | moderate | off (optional) (default to "moderate")
	page := int32(56) // int32 | 60 results per page (optional) (default to 1)
	duration := "duration_example" // string | short | medium | long (optional) (default to "")
	resolution := "resolution_example" // string | high | standard (optional) (default to "")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DuckDuckGoAPI.DuckduckgoVideoSearch(context.Background()).Query(query).Region(region).Safesearch(safesearch).Page(page).Duration(duration).Resolution(resolution).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DuckDuckGoAPI.DuckduckgoVideoSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DuckduckgoVideoSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DuckDuckGoAPI.DuckduckgoVideoSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiDuckduckgoVideoSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search query | 
 **region** | **string** | DuckDuckGo region code (kl), e.g. us-en, uk-en, de-de. wt-wt &#x3D; all regions. | [default to &quot;wt-wt&quot;]
 **safesearch** | **string** | on | moderate | off | [default to &quot;moderate&quot;]
 **page** | **int32** | 60 results per page | [default to 1]
 **duration** | **string** | short | medium | long | [default to &quot;&quot;]
 **resolution** | **string** | high | standard | [default to &quot;&quot;]

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


## DuckduckgoWebSearch

> interface{} DuckduckgoWebSearch(ctx).Query(query).Region(region).Safesearch(safesearch).Timelimit(timelimit).Page(page).Execute()

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
	query := "query_example" // string | Search query
	region := "region_example" // string | DuckDuckGo region code (kl), e.g. us-en, uk-en, de-de. wt-wt = all regions. (optional) (default to "wt-wt")
	safesearch := "safesearch_example" // string | on | moderate | off (optional) (default to "moderate")
	timelimit := "timelimit_example" // string | day | week | month | year (optional) (default to "")
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DuckDuckGoAPI.DuckduckgoWebSearch(context.Background()).Query(query).Region(region).Safesearch(safesearch).Timelimit(timelimit).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DuckDuckGoAPI.DuckduckgoWebSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DuckduckgoWebSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DuckDuckGoAPI.DuckduckgoWebSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiDuckduckgoWebSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search query | 
 **region** | **string** | DuckDuckGo region code (kl), e.g. us-en, uk-en, de-de. wt-wt &#x3D; all regions. | [default to &quot;wt-wt&quot;]
 **safesearch** | **string** | on | moderate | off | [default to &quot;moderate&quot;]
 **timelimit** | **string** | day | week | month | year | [default to &quot;&quot;]
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


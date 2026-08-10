# \YandexAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**YandexImageSearch**](YandexAPI.md#YandexImageSearch) | **Get** /v1/yandex/images/search | Image search
[**YandexListSupportedMarkets**](YandexAPI.md#YandexListSupportedMarkets) | **Get** /v1/yandex/markets | List supported markets
[**YandexReverseImageSearch**](YandexAPI.md#YandexReverseImageSearch) | **Get** /v1/yandex/images/reverse | Reverse image search
[**YandexWebSearch**](YandexAPI.md#YandexWebSearch) | **Get** /v1/yandex/search | Web search
[**YandexYandexScraperHealthCheck**](YandexAPI.md#YandexYandexScraperHealthCheck) | **Get** /v1/yandex/health | Yandex scraper health check
[**YandexYandexScraperHealthCheckHead**](YandexAPI.md#YandexYandexScraperHealthCheckHead) | **Head** /v1/yandex/health | Yandex scraper health check



## YandexImageSearch

> interface{} YandexImageSearch(ctx).Query(query).Domain(domain).Page(page).Execute()

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
	query := "query_example" // string | Image search query, e.g. 'coffee machine'
	domain := "domain_example" // string | Yandex market: 'tr' (yandex.com.tr, DEFAULT — the domain that reliably clears anti-bot), 'com', 'ru', 'by', 'kz', 'uz'. 'com'/'ru' have a lower success rate. (optional) (default to "tr")
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YandexAPI.YandexImageSearch(context.Background()).Query(query).Domain(domain).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YandexAPI.YandexImageSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YandexImageSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YandexAPI.YandexImageSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiYandexImageSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Image search query, e.g. &#39;coffee machine&#39; | 
 **domain** | **string** | Yandex market: &#39;tr&#39; (yandex.com.tr, DEFAULT — the domain that reliably clears anti-bot), &#39;com&#39;, &#39;ru&#39;, &#39;by&#39;, &#39;kz&#39;, &#39;uz&#39;. &#39;com&#39;/&#39;ru&#39; have a lower success rate. | [default to &quot;tr&quot;]
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


## YandexListSupportedMarkets

> interface{} YandexListSupportedMarkets(ctx).Execute()

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
	resp, r, err := apiClient.YandexAPI.YandexListSupportedMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YandexAPI.YandexListSupportedMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YandexListSupportedMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YandexAPI.YandexListSupportedMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiYandexListSupportedMarketsRequest struct via the builder pattern


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


## YandexReverseImageSearch

> interface{} YandexReverseImageSearch(ctx).ImageUrl(imageUrl).Domain(domain).Execute()

Reverse image search



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
	imageUrl := "imageUrl_example" // string | Public URL of the image to reverse-search
	domain := "domain_example" // string | Yandex market: 'tr' (yandex.com.tr, DEFAULT — the domain that reliably clears anti-bot), 'com', 'ru', 'by', 'kz', 'uz'. 'com'/'ru' have a lower success rate. (optional) (default to "tr")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YandexAPI.YandexReverseImageSearch(context.Background()).ImageUrl(imageUrl).Domain(domain).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YandexAPI.YandexReverseImageSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YandexReverseImageSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YandexAPI.YandexReverseImageSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiYandexReverseImageSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **imageUrl** | **string** | Public URL of the image to reverse-search | 
 **domain** | **string** | Yandex market: &#39;tr&#39; (yandex.com.tr, DEFAULT — the domain that reliably clears anti-bot), &#39;com&#39;, &#39;ru&#39;, &#39;by&#39;, &#39;kz&#39;, &#39;uz&#39;. &#39;com&#39;/&#39;ru&#39; have a lower success rate. | [default to &quot;tr&quot;]

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


## YandexWebSearch

> interface{} YandexWebSearch(ctx).Query(query).Domain(domain).Page(page).Lr(lr).Lang(lang).Execute()

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
	query := "query_example" // string | Search query, e.g. 'coffee machine'
	domain := "domain_example" // string | Yandex market: 'tr' (yandex.com.tr, DEFAULT — the domain that reliably clears anti-bot), 'com', 'ru', 'by', 'kz', 'uz'. 'com'/'ru' have a lower success rate. (optional) (default to "tr")
	page := int32(56) // int32 |  (optional) (default to 1)
	lr := int32(56) // int32 | Yandex region id, e.g. 213=Moscow, 84=USA (optional)
	lang := "lang_example" // string | UI language: ru, en, tr, be, kk, uk (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YandexAPI.YandexWebSearch(context.Background()).Query(query).Domain(domain).Page(page).Lr(lr).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YandexAPI.YandexWebSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YandexWebSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YandexAPI.YandexWebSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiYandexWebSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search query, e.g. &#39;coffee machine&#39; | 
 **domain** | **string** | Yandex market: &#39;tr&#39; (yandex.com.tr, DEFAULT — the domain that reliably clears anti-bot), &#39;com&#39;, &#39;ru&#39;, &#39;by&#39;, &#39;kz&#39;, &#39;uz&#39;. &#39;com&#39;/&#39;ru&#39; have a lower success rate. | [default to &quot;tr&quot;]
 **page** | **int32** |  | [default to 1]
 **lr** | **int32** | Yandex region id, e.g. 213&#x3D;Moscow, 84&#x3D;USA | 
 **lang** | **string** | UI language: ru, en, tr, be, kk, uk | 

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


## YandexYandexScraperHealthCheck

> interface{} YandexYandexScraperHealthCheck(ctx).Execute()

Yandex scraper health check



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
	resp, r, err := apiClient.YandexAPI.YandexYandexScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YandexAPI.YandexYandexScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YandexYandexScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YandexAPI.YandexYandexScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiYandexYandexScraperHealthCheckRequest struct via the builder pattern


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


## YandexYandexScraperHealthCheckHead

> interface{} YandexYandexScraperHealthCheckHead(ctx).Execute()

Yandex scraper health check



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
	resp, r, err := apiClient.YandexAPI.YandexYandexScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YandexAPI.YandexYandexScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YandexYandexScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YandexAPI.YandexYandexScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiYandexYandexScraperHealthCheckHeadRequest struct via the builder pattern


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


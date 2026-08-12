# \AppStoreAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AppStoreGetAppDetail**](AppStoreAPI.md#AppStoreGetAppDetail) | **Get** /v1/app-store/apps/{app_id} | Get app detail
[**AppStoreGetAppReviews**](AppStoreAPI.md#AppStoreGetAppReviews) | **Get** /v1/app-store/apps/{app_id}/reviews | Get app reviews
[**AppStoreGetDeveloperApps**](AppStoreAPI.md#AppStoreGetDeveloperApps) | **Get** /v1/app-store/developers/{artist_id} | Get developer apps
[**AppStoreListGenres**](AppStoreAPI.md#AppStoreListGenres) | **Get** /v1/app-store/genres | List genres
[**AppStoreListMarkets**](AppStoreAPI.md#AppStoreListMarkets) | **Get** /v1/app-store/markets | List markets
[**AppStoreSearchApps**](AppStoreAPI.md#AppStoreSearchApps) | **Get** /v1/app-store/search | Search apps
[**AppStoreTopCharts**](AppStoreAPI.md#AppStoreTopCharts) | **Get** /v1/app-store/charts | Top charts



## AppStoreGetAppDetail

> interface{} AppStoreGetAppDetail(ctx, appId).Country(country).Lang(lang).IncludeExtras(includeExtras).Execute()

Get app detail



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
	appId := "appId_example" // string | Numeric trackId (e.g. '310633997') or bundle id (e.g. 'net.whatsapp.WhatsApp').
	country := "country_example" // string |  (optional) (default to "us")
	lang := "lang_example" // string | Result language, e.g. 'en_us' (optional)
	includeExtras := true // bool | Fetch the storefront page for rating histogram, IAP list, full-res screenshots and App Privacy. Set false to skip the 2nd fetch. (optional) (default to true)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppStoreAPI.AppStoreGetAppDetail(context.Background(), appId).Country(country).Lang(lang).IncludeExtras(includeExtras).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppStoreAPI.AppStoreGetAppDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AppStoreGetAppDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AppStoreAPI.AppStoreGetAppDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**appId** | **string** | Numeric trackId (e.g. &#39;310633997&#39;) or bundle id (e.g. &#39;net.whatsapp.WhatsApp&#39;). | 

### Other Parameters

Other parameters are passed through a pointer to a apiAppStoreGetAppDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** |  | [default to &quot;us&quot;]
 **lang** | **string** | Result language, e.g. &#39;en_us&#39; | 
 **includeExtras** | **bool** | Fetch the storefront page for rating histogram, IAP list, full-res screenshots and App Privacy. Set false to skip the 2nd fetch. | [default to true]

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


## AppStoreGetAppReviews

> interface{} AppStoreGetAppReviews(ctx, appId).Country(country).Page(page).Sort(sort).Execute()

Get app reviews



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
	appId := "appId_example" // string | Numeric trackId, e.g. '310633997'
	country := "country_example" // string |  (optional) (default to "us")
	page := int32(56) // int32 | Apple caps reviews at 10 pages (optional) (default to 1)
	sort := "sort_example" // string | mostRecent | mostHelpful (optional) (default to "mostRecent")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppStoreAPI.AppStoreGetAppReviews(context.Background(), appId).Country(country).Page(page).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppStoreAPI.AppStoreGetAppReviews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AppStoreGetAppReviews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AppStoreAPI.AppStoreGetAppReviews`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**appId** | **string** | Numeric trackId, e.g. &#39;310633997&#39; | 

### Other Parameters

Other parameters are passed through a pointer to a apiAppStoreGetAppReviewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** |  | [default to &quot;us&quot;]
 **page** | **int32** | Apple caps reviews at 10 pages | [default to 1]
 **sort** | **string** | mostRecent | mostHelpful | [default to &quot;mostRecent&quot;]

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


## AppStoreGetDeveloperApps

> interface{} AppStoreGetDeveloperApps(ctx, artistId).Country(country).Execute()

Get developer apps



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
	artistId := "artistId_example" // string | Numeric artistId (developer id)
	country := "country_example" // string |  (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppStoreAPI.AppStoreGetDeveloperApps(context.Background(), artistId).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppStoreAPI.AppStoreGetDeveloperApps``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AppStoreGetDeveloperApps`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AppStoreAPI.AppStoreGetDeveloperApps`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**artistId** | **string** | Numeric artistId (developer id) | 

### Other Parameters

Other parameters are passed through a pointer to a apiAppStoreGetDeveloperAppsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** |  | [default to &quot;us&quot;]

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


## AppStoreListGenres

> interface{} AppStoreListGenres(ctx).Execute()

List genres



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
	resp, r, err := apiClient.AppStoreAPI.AppStoreListGenres(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppStoreAPI.AppStoreListGenres``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AppStoreListGenres`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AppStoreAPI.AppStoreListGenres`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAppStoreListGenresRequest struct via the builder pattern


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


## AppStoreListMarkets

> interface{} AppStoreListMarkets(ctx).Execute()

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
	resp, r, err := apiClient.AppStoreAPI.AppStoreListMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppStoreAPI.AppStoreListMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AppStoreListMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AppStoreAPI.AppStoreListMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAppStoreListMarketsRequest struct via the builder pattern


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


## AppStoreSearchApps

> interface{} AppStoreSearchApps(ctx).Query(query).Country(country).Entity(entity).Limit(limit).Offset(offset).Lang(lang).Execute()

Search apps



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
	query := "query_example" // string | Search term, e.g. 'chat'
	country := "country_example" // string | App Store country code (optional) (default to "us")
	entity := "entity_example" // string | software | iPadSoftware | macSoftware (optional) (default to "software")
	limit := int32(56) // int32 |  (optional) (default to 25)
	offset := int32(56) // int32 |  (optional) (default to 0)
	lang := "lang_example" // string | Language, e.g. 'en_us' (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppStoreAPI.AppStoreSearchApps(context.Background()).Query(query).Country(country).Entity(entity).Limit(limit).Offset(offset).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppStoreAPI.AppStoreSearchApps``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AppStoreSearchApps`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AppStoreAPI.AppStoreSearchApps`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAppStoreSearchAppsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search term, e.g. &#39;chat&#39; | 
 **country** | **string** | App Store country code | [default to &quot;us&quot;]
 **entity** | **string** | software | iPadSoftware | macSoftware | [default to &quot;software&quot;]
 **limit** | **int32** |  | [default to 25]
 **offset** | **int32** |  | [default to 0]
 **lang** | **string** | Language, e.g. &#39;en_us&#39; | 

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


## AppStoreTopCharts

> interface{} AppStoreTopCharts(ctx).Country(country).Type_(type_).Genre(genre).Limit(limit).Entity(entity).Execute()

Top charts



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
	country := "country_example" // string |  (optional) (default to "us")
	type_ := "type__example" // string | top-free | top-paid | top-grossing (optional) (default to "top-free")
	genre := int32(56) // int32 | Apple genre id (optional), e.g. 6014 (optional)
	limit := int32(56) // int32 |  (optional) (default to 50)
	entity := "entity_example" // string | apps (iPhone) | ipad (optional) (default to "apps")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppStoreAPI.AppStoreTopCharts(context.Background()).Country(country).Type_(type_).Genre(genre).Limit(limit).Entity(entity).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppStoreAPI.AppStoreTopCharts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AppStoreTopCharts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AppStoreAPI.AppStoreTopCharts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAppStoreTopChartsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **country** | **string** |  | [default to &quot;us&quot;]
 **type_** | **string** | top-free | top-paid | top-grossing | [default to &quot;top-free&quot;]
 **genre** | **int32** | Apple genre id (optional), e.g. 6014 | 
 **limit** | **int32** |  | [default to 50]
 **entity** | **string** | apps (iPhone) | ipad | [default to &quot;apps&quot;]

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


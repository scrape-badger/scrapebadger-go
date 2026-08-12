# \GooglePlayAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GooglePlayBrowseACategory**](GooglePlayAPI.md#GooglePlayBrowseACategory) | **Get** /v1/google-play/categories/{category_id} | Browse a category
[**GooglePlayGetAppDetail**](GooglePlayAPI.md#GooglePlayGetAppDetail) | **Get** /v1/google-play/apps/{app_id} | Get app detail
[**GooglePlayGetAppPermissions**](GooglePlayAPI.md#GooglePlayGetAppPermissions) | **Get** /v1/google-play/apps/{app_id}/permissions | Get app permissions
[**GooglePlayGetAppReviews**](GooglePlayAPI.md#GooglePlayGetAppReviews) | **Get** /v1/google-play/apps/{app_id}/reviews | Get app reviews
[**GooglePlayGetDeveloperApps**](GooglePlayAPI.md#GooglePlayGetDeveloperApps) | **Get** /v1/google-play/developers/{developer} | Get developer apps
[**GooglePlayGetSimilarApps**](GooglePlayAPI.md#GooglePlayGetSimilarApps) | **Get** /v1/google-play/apps/{app_id}/similar | Get similar apps
[**GooglePlayListCategories**](GooglePlayAPI.md#GooglePlayListCategories) | **Get** /v1/google-play/categories | List categories
[**GooglePlayListMarkets**](GooglePlayAPI.md#GooglePlayListMarkets) | **Get** /v1/google-play/markets | List markets
[**GooglePlaySearchApps**](GooglePlayAPI.md#GooglePlaySearchApps) | **Get** /v1/google-play/search | Search apps
[**GooglePlayTopCharts**](GooglePlayAPI.md#GooglePlayTopCharts) | **Get** /v1/google-play/collections/{collection} | Top charts



## GooglePlayBrowseACategory

> interface{} GooglePlayBrowseACategory(ctx, categoryId).Country(country).Lang(lang).Execute()

Browse a category



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
	categoryId := "categoryId_example" // string | Play category id, e.g. 'GAME_PUZZLE' or 'SOCIAL'
	country := "country_example" // string | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. 'US' (optional) (default to "US")
	lang := "lang_example" // string | Play content language (hl), e.g. 'en' or 'pt-BR' (optional) (default to "en")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayBrowseACategory(context.Background(), categoryId).Country(country).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayBrowseACategory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayBrowseACategory`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayBrowseACategory`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**categoryId** | **string** | Play category id, e.g. &#39;GAME_PUZZLE&#39; or &#39;SOCIAL&#39; | 

### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayBrowseACategoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. &#39;US&#39; | [default to &quot;US&quot;]
 **lang** | **string** | Play content language (hl), e.g. &#39;en&#39; or &#39;pt-BR&#39; | [default to &quot;en&quot;]

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


## GooglePlayGetAppDetail

> interface{} GooglePlayGetAppDetail(ctx, appId).Country(country).Lang(lang).Execute()

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
	appId := "appId_example" // string | Android package id, e.g. 'com.whatsapp'.
	country := "country_example" // string | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. 'US' (optional) (default to "US")
	lang := "lang_example" // string | Play content language (hl), e.g. 'en' or 'pt-BR' (optional) (default to "en")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayGetAppDetail(context.Background(), appId).Country(country).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayGetAppDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayGetAppDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayGetAppDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**appId** | **string** | Android package id, e.g. &#39;com.whatsapp&#39;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayGetAppDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. &#39;US&#39; | [default to &quot;US&quot;]
 **lang** | **string** | Play content language (hl), e.g. &#39;en&#39; or &#39;pt-BR&#39; | [default to &quot;en&quot;]

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


## GooglePlayGetAppPermissions

> interface{} GooglePlayGetAppPermissions(ctx, appId).Lang(lang).Execute()

Get app permissions



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
	appId := "appId_example" // string | Android package id, e.g. 'com.whatsapp'.
	lang := "lang_example" // string | Play content language (hl), e.g. 'en' or 'pt-BR' (optional) (default to "en")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayGetAppPermissions(context.Background(), appId).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayGetAppPermissions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayGetAppPermissions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayGetAppPermissions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**appId** | **string** | Android package id, e.g. &#39;com.whatsapp&#39;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayGetAppPermissionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **lang** | **string** | Play content language (hl), e.g. &#39;en&#39; or &#39;pt-BR&#39; | [default to &quot;en&quot;]

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


## GooglePlayGetAppReviews

> interface{} GooglePlayGetAppReviews(ctx, appId).Country(country).Lang(lang).Sort(sort).Count(count).PageToken(pageToken).Execute()

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
	appId := "appId_example" // string | Android package id, e.g. 'com.whatsapp'.
	country := "country_example" // string | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. 'US' (optional) (default to "US")
	lang := "lang_example" // string | Play content language (hl), e.g. 'en' or 'pt-BR' (optional) (default to "en")
	sort := "sort_example" // string | newest | rating | helpfulness (optional) (default to "newest")
	count := int32(56) // int32 |  (optional) (default to 40)
	pageToken := "pageToken_example" // string | Pagination token (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayGetAppReviews(context.Background(), appId).Country(country).Lang(lang).Sort(sort).Count(count).PageToken(pageToken).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayGetAppReviews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayGetAppReviews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayGetAppReviews`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**appId** | **string** | Android package id, e.g. &#39;com.whatsapp&#39;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayGetAppReviewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. &#39;US&#39; | [default to &quot;US&quot;]
 **lang** | **string** | Play content language (hl), e.g. &#39;en&#39; or &#39;pt-BR&#39; | [default to &quot;en&quot;]
 **sort** | **string** | newest | rating | helpfulness | [default to &quot;newest&quot;]
 **count** | **int32** |  | [default to 40]
 **pageToken** | **string** | Pagination token | 

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


## GooglePlayGetDeveloperApps

> interface{} GooglePlayGetDeveloperApps(ctx, developer).Country(country).Lang(lang).Execute()

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
	developer := "developer_example" // string | Developer name or numeric id
	country := "country_example" // string | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. 'US' (optional) (default to "US")
	lang := "lang_example" // string | Play content language (hl), e.g. 'en' or 'pt-BR' (optional) (default to "en")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayGetDeveloperApps(context.Background(), developer).Country(country).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayGetDeveloperApps``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayGetDeveloperApps`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayGetDeveloperApps`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**developer** | **string** | Developer name or numeric id | 

### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayGetDeveloperAppsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. &#39;US&#39; | [default to &quot;US&quot;]
 **lang** | **string** | Play content language (hl), e.g. &#39;en&#39; or &#39;pt-BR&#39; | [default to &quot;en&quot;]

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


## GooglePlayGetSimilarApps

> interface{} GooglePlayGetSimilarApps(ctx, appId).Country(country).Lang(lang).Execute()

Get similar apps



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
	appId := "appId_example" // string | Android package id, e.g. 'com.whatsapp'.
	country := "country_example" // string | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. 'US' (optional) (default to "US")
	lang := "lang_example" // string | Play content language (hl), e.g. 'en' or 'pt-BR' (optional) (default to "en")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayGetSimilarApps(context.Background(), appId).Country(country).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayGetSimilarApps``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayGetSimilarApps`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayGetSimilarApps`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**appId** | **string** | Android package id, e.g. &#39;com.whatsapp&#39;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayGetSimilarAppsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. &#39;US&#39; | [default to &quot;US&quot;]
 **lang** | **string** | Play content language (hl), e.g. &#39;en&#39; or &#39;pt-BR&#39; | [default to &quot;en&quot;]

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


## GooglePlayListCategories

> interface{} GooglePlayListCategories(ctx).Execute()

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayListCategories(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayListCategories``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayListCategories`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayListCategories`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayListCategoriesRequest struct via the builder pattern


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


## GooglePlayListMarkets

> interface{} GooglePlayListMarkets(ctx).Execute()

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
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayListMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayListMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayListMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayListMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayListMarketsRequest struct via the builder pattern


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


## GooglePlaySearchApps

> interface{} GooglePlaySearchApps(ctx).Query(query).Country(country).Lang(lang).Price(price).Execute()

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
	query := "query_example" // string | Search keywords, e.g. 'puzzle'
	country := "country_example" // string | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. 'US' (optional) (default to "US")
	lang := "lang_example" // string | Play content language (hl), e.g. 'en' or 'pt-BR' (optional) (default to "en")
	price := "price_example" // string | free | paid | all (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlaySearchApps(context.Background()).Query(query).Country(country).Lang(lang).Price(price).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlaySearchApps``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlaySearchApps`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlaySearchApps`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlaySearchAppsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords, e.g. &#39;puzzle&#39; | 
 **country** | **string** | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. &#39;US&#39; | [default to &quot;US&quot;]
 **lang** | **string** | Play content language (hl), e.g. &#39;en&#39; or &#39;pt-BR&#39; | [default to &quot;en&quot;]
 **price** | **string** | free | paid | all | 

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


## GooglePlayTopCharts

> interface{} GooglePlayTopCharts(ctx, collection).Category(category).Country(country).Lang(lang).Execute()

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
	collection := "collection_example" // string | topselling_free | topselling_paid | topgrossing
	category := "category_example" // string | Play category, e.g. 'GAME' (optional) (default to "APPLICATION")
	country := "country_example" // string | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. 'US' (optional) (default to "US")
	lang := "lang_example" // string | Play content language (hl), e.g. 'en' or 'pt-BR' (optional) (default to "en")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayTopCharts(context.Background(), collection).Category(category).Country(country).Lang(lang).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayTopCharts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayTopCharts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayTopCharts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**collection** | **string** | topselling_free | topselling_paid | topgrossing | 

### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayTopChartsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **category** | **string** | Play category, e.g. &#39;GAME&#39; | [default to &quot;APPLICATION&quot;]
 **country** | **string** | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. &#39;US&#39; | [default to &quot;US&quot;]
 **lang** | **string** | Play content language (hl), e.g. &#39;en&#39; or &#39;pt-BR&#39; | [default to &quot;en&quot;]

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


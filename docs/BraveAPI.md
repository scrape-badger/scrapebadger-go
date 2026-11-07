# \BraveAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**BraveAutocomplete**](BraveAPI.md#BraveAutocomplete) | **Get** /v1/brave/autocomplete | Autocomplete
[**BraveImageSearch**](BraveAPI.md#BraveImageSearch) | **Get** /v1/brave/images | Image search
[**BraveListSupportedLocales**](BraveAPI.md#BraveListSupportedLocales) | **Get** /v1/brave/locales | List supported locales
[**BraveNewsSearch**](BraveAPI.md#BraveNewsSearch) | **Get** /v1/brave/news | News search
[**BraveVideoSearch**](BraveAPI.md#BraveVideoSearch) | **Get** /v1/brave/videos | Video search
[**BraveWebSearch**](BraveAPI.md#BraveWebSearch) | **Get** /v1/brave/search | Web search



## BraveAutocomplete

> BraveAutocompleteResponse BraveAutocomplete(ctx).Query(query).Country(country).Execute()

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
	query := "query_example" // string | 
	country := "country_example" // string |  (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BraveAPI.BraveAutocomplete(context.Background()).Query(query).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BraveAPI.BraveAutocomplete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BraveAutocomplete`: BraveAutocompleteResponse
	fmt.Fprintf(os.Stdout, "Response from `BraveAPI.BraveAutocomplete`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBraveAutocompleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 
 **country** | **string** |  | [default to &quot;us&quot;]

### Return type

[**BraveAutocompleteResponse**](BraveAutocompleteResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BraveImageSearch

> BraveResponse BraveImageSearch(ctx).Query(query).Country(country).UiLanguage(uiLanguage).SafeSearch(safeSearch).Count(count).Execute()

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
	query := "query_example" // string | Native Brave search query
	country := "country_example" // string | Native result region; see /locales (optional) (default to "us")
	uiLanguage := "uiLanguage_example" // string | UI labels/date language; does not restrict result language (optional) (default to "en-us")
	safeSearch := "safeSearch_example" // string |  (optional) (default to "moderate")
	count := int32(56) // int32 | Slice the initial native image batch (optional) (default to 50)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BraveAPI.BraveImageSearch(context.Background()).Query(query).Country(country).UiLanguage(uiLanguage).SafeSearch(safeSearch).Count(count).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BraveAPI.BraveImageSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BraveImageSearch`: BraveResponse
	fmt.Fprintf(os.Stdout, "Response from `BraveAPI.BraveImageSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBraveImageSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Native Brave search query | 
 **country** | **string** | Native result region; see /locales | [default to &quot;us&quot;]
 **uiLanguage** | **string** | UI labels/date language; does not restrict result language | [default to &quot;en-us&quot;]
 **safeSearch** | **string** |  | [default to &quot;moderate&quot;]
 **count** | **int32** | Slice the initial native image batch | [default to 50]

### Return type

[**BraveResponse**](BraveResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BraveListSupportedLocales

> BraveLocalesResponse BraveListSupportedLocales(ctx).Execute()

List supported locales



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
	resp, r, err := apiClient.BraveAPI.BraveListSupportedLocales(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BraveAPI.BraveListSupportedLocales``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BraveListSupportedLocales`: BraveLocalesResponse
	fmt.Fprintf(os.Stdout, "Response from `BraveAPI.BraveListSupportedLocales`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiBraveListSupportedLocalesRequest struct via the builder pattern


### Return type

[**BraveLocalesResponse**](BraveLocalesResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BraveNewsSearch

> BraveResponse BraveNewsSearch(ctx).Query(query).Country(country).UiLanguage(uiLanguage).SafeSearch(safeSearch).Count(count).Execute()

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
	query := "query_example" // string | Native Brave search query
	country := "country_example" // string | Native result region; see /locales (optional) (default to "us")
	uiLanguage := "uiLanguage_example" // string | UI labels/date language; does not restrict result language (optional) (default to "en-us")
	safeSearch := "safeSearch_example" // string |  (optional) (default to "moderate")
	count := int32(56) // int32 | Slice the initial native news batch (optional) (default to 35)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BraveAPI.BraveNewsSearch(context.Background()).Query(query).Country(country).UiLanguage(uiLanguage).SafeSearch(safeSearch).Count(count).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BraveAPI.BraveNewsSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BraveNewsSearch`: BraveResponse
	fmt.Fprintf(os.Stdout, "Response from `BraveAPI.BraveNewsSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBraveNewsSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Native Brave search query | 
 **country** | **string** | Native result region; see /locales | [default to &quot;us&quot;]
 **uiLanguage** | **string** | UI labels/date language; does not restrict result language | [default to &quot;en-us&quot;]
 **safeSearch** | **string** |  | [default to &quot;moderate&quot;]
 **count** | **int32** | Slice the initial native news batch | [default to 35]

### Return type

[**BraveResponse**](BraveResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BraveVideoSearch

> BravePagedResponse BraveVideoSearch(ctx).Query(query).Country(country).UiLanguage(uiLanguage).SafeSearch(safeSearch).Page(page).Count(count).Execute()

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
	query := "query_example" // string | Native Brave search query
	country := "country_example" // string | Native result region; see /locales (optional) (default to "us")
	uiLanguage := "uiLanguage_example" // string | UI labels/date language; does not restrict result language (optional) (default to "en-us")
	safeSearch := "safeSearch_example" // string |  (optional) (default to "moderate")
	page := int32(56) // int32 | 1-based native page ordinal (optional) (default to 1)
	count := int32(56) // int32 |  (optional) (default to 50)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BraveAPI.BraveVideoSearch(context.Background()).Query(query).Country(country).UiLanguage(uiLanguage).SafeSearch(safeSearch).Page(page).Count(count).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BraveAPI.BraveVideoSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BraveVideoSearch`: BravePagedResponse
	fmt.Fprintf(os.Stdout, "Response from `BraveAPI.BraveVideoSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBraveVideoSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Native Brave search query | 
 **country** | **string** | Native result region; see /locales | [default to &quot;us&quot;]
 **uiLanguage** | **string** | UI labels/date language; does not restrict result language | [default to &quot;en-us&quot;]
 **safeSearch** | **string** |  | [default to &quot;moderate&quot;]
 **page** | **int32** | 1-based native page ordinal | [default to 1]
 **count** | **int32** |  | [default to 50]

### Return type

[**BravePagedResponse**](BravePagedResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BraveWebSearch

> BraveSearchResponse BraveWebSearch(ctx).Query(query).Country(country).UiLanguage(uiLanguage).SafeSearch(safeSearch).Page(page).Count(count).Freshness(freshness).Spellcheck(spellcheck).Execute()

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
	query := "query_example" // string | Native Brave search query
	country := "country_example" // string | Native result region; see /locales (optional) (default to "us")
	uiLanguage := "uiLanguage_example" // string | UI labels/date language; does not restrict result language (optional) (default to "en-us")
	safeSearch := "safeSearch_example" // string |  (optional) (default to "moderate")
	page := int32(56) // int32 | 1-based native page ordinal (optional) (default to 1)
	count := int32(56) // int32 | Slice one native page; does not change native page boundaries (optional) (default to 20)
	freshness := "freshness_example" // string |  (optional) (default to "any")
	spellcheck := true // bool | Allow native spelling correction (optional) (default to false)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BraveAPI.BraveWebSearch(context.Background()).Query(query).Country(country).UiLanguage(uiLanguage).SafeSearch(safeSearch).Page(page).Count(count).Freshness(freshness).Spellcheck(spellcheck).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BraveAPI.BraveWebSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BraveWebSearch`: BraveSearchResponse
	fmt.Fprintf(os.Stdout, "Response from `BraveAPI.BraveWebSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBraveWebSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Native Brave search query | 
 **country** | **string** | Native result region; see /locales | [default to &quot;us&quot;]
 **uiLanguage** | **string** | UI labels/date language; does not restrict result language | [default to &quot;en-us&quot;]
 **safeSearch** | **string** |  | [default to &quot;moderate&quot;]
 **page** | **int32** | 1-based native page ordinal | [default to 1]
 **count** | **int32** | Slice one native page; does not change native page boundaries | [default to 20]
 **freshness** | **string** |  | [default to &quot;any&quot;]
 **spellcheck** | **bool** | Allow native spelling correction | [default to false]

### Return type

[**BraveSearchResponse**](BraveSearchResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


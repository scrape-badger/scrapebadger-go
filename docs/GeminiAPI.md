# \GeminiAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GeminiAskGeminiAQuestion**](GeminiAPI.md#GeminiAskGeminiAQuestion) | **Get** /v1/gemini/ask | Ask Gemini a question
[**GeminiAskGeminiAQuestionPost**](GeminiAPI.md#GeminiAskGeminiAQuestionPost) | **Post** /v1/gemini/ask | Ask Gemini a question (POST)
[**GeminiGeminiScraperHealthCheck**](GeminiAPI.md#GeminiGeminiScraperHealthCheck) | **Get** /v1/gemini/health | Gemini scraper health check
[**GeminiGeminiScraperHealthCheckHead**](GeminiAPI.md#GeminiGeminiScraperHealthCheckHead) | **Head** /v1/gemini/health | Gemini scraper health check
[**GeminiMeasureABrandSVisibilityInAGeminiAnswer**](GeminiAPI.md#GeminiMeasureABrandSVisibilityInAGeminiAnswer) | **Get** /v1/gemini/brand-visibility | Measure a brand&#39;s visibility in a Gemini answer
[**GeminiMeasureABrandSVisibilityInAGeminiAnswerPost**](GeminiAPI.md#GeminiMeasureABrandSVisibilityInAGeminiAnswerPost) | **Post** /v1/gemini/brand-visibility | Measure a brand&#39;s visibility in a Gemini answer (POST)



## GeminiAskGeminiAQuestion

> interface{} GeminiAskGeminiAQuestion(ctx).Prompt(prompt).Country(country).WebSearch(webSearch).Execute()

Ask Gemini a question



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
	prompt := "prompt_example" // string | The prompt to send to Gemini (max 4096 characters).
	country := "country_example" // string | ISO-3166 alpha-2 egress country, e.g. 'US', 'GB', 'DE'. (optional)
	webSearch := "webSearch_example" // string | auto (let Gemini decide) | force (ask it to browse) | off (answer from memory). `web_search_triggered` in the response always reports what actually happened. (optional) (default to "auto")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GeminiAPI.GeminiAskGeminiAQuestion(context.Background()).Prompt(prompt).Country(country).WebSearch(webSearch).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GeminiAPI.GeminiAskGeminiAQuestion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GeminiAskGeminiAQuestion`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GeminiAPI.GeminiAskGeminiAQuestion`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGeminiAskGeminiAQuestionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **prompt** | **string** | The prompt to send to Gemini (max 4096 characters). | 
 **country** | **string** | ISO-3166 alpha-2 egress country, e.g. &#39;US&#39;, &#39;GB&#39;, &#39;DE&#39;. | 
 **webSearch** | **string** | auto (let Gemini decide) | force (ask it to browse) | off (answer from memory). &#x60;web_search_triggered&#x60; in the response always reports what actually happened. | [default to &quot;auto&quot;]

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


## GeminiAskGeminiAQuestionPost

> interface{} GeminiAskGeminiAQuestionPost(ctx).Execute()

Ask Gemini a question (POST)



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
	resp, r, err := apiClient.GeminiAPI.GeminiAskGeminiAQuestionPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GeminiAPI.GeminiAskGeminiAQuestionPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GeminiAskGeminiAQuestionPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GeminiAPI.GeminiAskGeminiAQuestionPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGeminiAskGeminiAQuestionPostRequest struct via the builder pattern


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


## GeminiGeminiScraperHealthCheck

> interface{} GeminiGeminiScraperHealthCheck(ctx).Execute()

Gemini scraper health check



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
	resp, r, err := apiClient.GeminiAPI.GeminiGeminiScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GeminiAPI.GeminiGeminiScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GeminiGeminiScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GeminiAPI.GeminiGeminiScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGeminiGeminiScraperHealthCheckRequest struct via the builder pattern


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


## GeminiGeminiScraperHealthCheckHead

> interface{} GeminiGeminiScraperHealthCheckHead(ctx).Execute()

Gemini scraper health check



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
	resp, r, err := apiClient.GeminiAPI.GeminiGeminiScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GeminiAPI.GeminiGeminiScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GeminiGeminiScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GeminiAPI.GeminiGeminiScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGeminiGeminiScraperHealthCheckHeadRequest struct via the builder pattern


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


## GeminiMeasureABrandSVisibilityInAGeminiAnswer

> interface{} GeminiMeasureABrandSVisibilityInAGeminiAnswer(ctx).Prompt(prompt).Brand(brand).Domain(domain).Aliases(aliases).Competitors(competitors).Country(country).WebSearch(webSearch).Execute()

Measure a brand's visibility in a Gemini answer



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
	prompt := "prompt_example" // string | The prompt to ask Gemini.
	brand := "brand_example" // string | Brand name to look for in the answer.
	domain := "domain_example" // string | Brand domain, for citation matching. (optional)
	aliases := "aliases_example" // string | Comma-separated alternative names. (optional)
	competitors := "competitors_example" // string | Comma-separated competitor names. (optional)
	country := "country_example" // string | ISO-3166 alpha-2 egress country. (optional)
	webSearch := "webSearch_example" // string | auto | force | off (optional) (default to "force")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GeminiAPI.GeminiMeasureABrandSVisibilityInAGeminiAnswer(context.Background()).Prompt(prompt).Brand(brand).Domain(domain).Aliases(aliases).Competitors(competitors).Country(country).WebSearch(webSearch).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GeminiAPI.GeminiMeasureABrandSVisibilityInAGeminiAnswer``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GeminiMeasureABrandSVisibilityInAGeminiAnswer`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GeminiAPI.GeminiMeasureABrandSVisibilityInAGeminiAnswer`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGeminiMeasureABrandSVisibilityInAGeminiAnswerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **prompt** | **string** | The prompt to ask Gemini. | 
 **brand** | **string** | Brand name to look for in the answer. | 
 **domain** | **string** | Brand domain, for citation matching. | 
 **aliases** | **string** | Comma-separated alternative names. | 
 **competitors** | **string** | Comma-separated competitor names. | 
 **country** | **string** | ISO-3166 alpha-2 egress country. | 
 **webSearch** | **string** | auto | force | off | [default to &quot;force&quot;]

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


## GeminiMeasureABrandSVisibilityInAGeminiAnswerPost

> interface{} GeminiMeasureABrandSVisibilityInAGeminiAnswerPost(ctx).Execute()

Measure a brand's visibility in a Gemini answer (POST)



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
	resp, r, err := apiClient.GeminiAPI.GeminiMeasureABrandSVisibilityInAGeminiAnswerPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GeminiAPI.GeminiMeasureABrandSVisibilityInAGeminiAnswerPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GeminiMeasureABrandSVisibilityInAGeminiAnswerPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GeminiAPI.GeminiMeasureABrandSVisibilityInAGeminiAnswerPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGeminiMeasureABrandSVisibilityInAGeminiAnswerPostRequest struct via the builder pattern


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


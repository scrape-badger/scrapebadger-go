# \PerplexityAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**PerplexityAskPerplexityAQuestion**](PerplexityAPI.md#PerplexityAskPerplexityAQuestion) | **Get** /v1/perplexity/ask | Ask Perplexity a question
[**PerplexityAskPerplexityAQuestionPost**](PerplexityAPI.md#PerplexityAskPerplexityAQuestionPost) | **Post** /v1/perplexity/ask | Ask Perplexity a question (POST)
[**PerplexityMeasureABrandSVisibilityInAPerplexityAnswer**](PerplexityAPI.md#PerplexityMeasureABrandSVisibilityInAPerplexityAnswer) | **Get** /v1/perplexity/brand-visibility | Measure a brand&#39;s visibility in a Perplexity answer
[**PerplexityMeasureABrandSVisibilityInAPerplexityAnswerPost**](PerplexityAPI.md#PerplexityMeasureABrandSVisibilityInAPerplexityAnswerPost) | **Post** /v1/perplexity/brand-visibility | Measure a brand&#39;s visibility in a Perplexity answer (POST)
[**PerplexityPerplexityScraperHealthCheck**](PerplexityAPI.md#PerplexityPerplexityScraperHealthCheck) | **Get** /v1/perplexity/health | Perplexity scraper health check
[**PerplexityPerplexityScraperHealthCheckHead**](PerplexityAPI.md#PerplexityPerplexityScraperHealthCheckHead) | **Head** /v1/perplexity/health | Perplexity scraper health check



## PerplexityAskPerplexityAQuestion

> interface{} PerplexityAskPerplexityAQuestion(ctx).Prompt(prompt).Country(country).Execute()

Ask Perplexity a question



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
	prompt := "prompt_example" // string | The prompt to send to Perplexity (max 4096 characters).
	country := "country_example" // string | ISO-3166 alpha-2 egress country, e.g. 'US', 'GB', 'DE'. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PerplexityAPI.PerplexityAskPerplexityAQuestion(context.Background()).Prompt(prompt).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PerplexityAPI.PerplexityAskPerplexityAQuestion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PerplexityAskPerplexityAQuestion`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `PerplexityAPI.PerplexityAskPerplexityAQuestion`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiPerplexityAskPerplexityAQuestionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **prompt** | **string** | The prompt to send to Perplexity (max 4096 characters). | 
 **country** | **string** | ISO-3166 alpha-2 egress country, e.g. &#39;US&#39;, &#39;GB&#39;, &#39;DE&#39;. | 

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


## PerplexityAskPerplexityAQuestionPost

> interface{} PerplexityAskPerplexityAQuestionPost(ctx).Execute()

Ask Perplexity a question (POST)



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
	resp, r, err := apiClient.PerplexityAPI.PerplexityAskPerplexityAQuestionPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PerplexityAPI.PerplexityAskPerplexityAQuestionPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PerplexityAskPerplexityAQuestionPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `PerplexityAPI.PerplexityAskPerplexityAQuestionPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiPerplexityAskPerplexityAQuestionPostRequest struct via the builder pattern


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


## PerplexityMeasureABrandSVisibilityInAPerplexityAnswer

> interface{} PerplexityMeasureABrandSVisibilityInAPerplexityAnswer(ctx).Prompt(prompt).Brand(brand).Domain(domain).Aliases(aliases).Competitors(competitors).Country(country).Execute()

Measure a brand's visibility in a Perplexity answer



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
	prompt := "prompt_example" // string | The prompt to ask Perplexity.
	brand := "brand_example" // string | Brand name to look for in the answer.
	domain := "domain_example" // string | Brand domain, for citation matching. (optional)
	aliases := "aliases_example" // string | Comma-separated alternative names. (optional)
	competitors := "competitors_example" // string | Comma-separated competitor names. (optional)
	country := "country_example" // string | ISO-3166 alpha-2 egress country. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PerplexityAPI.PerplexityMeasureABrandSVisibilityInAPerplexityAnswer(context.Background()).Prompt(prompt).Brand(brand).Domain(domain).Aliases(aliases).Competitors(competitors).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PerplexityAPI.PerplexityMeasureABrandSVisibilityInAPerplexityAnswer``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PerplexityMeasureABrandSVisibilityInAPerplexityAnswer`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `PerplexityAPI.PerplexityMeasureABrandSVisibilityInAPerplexityAnswer`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiPerplexityMeasureABrandSVisibilityInAPerplexityAnswerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **prompt** | **string** | The prompt to ask Perplexity. | 
 **brand** | **string** | Brand name to look for in the answer. | 
 **domain** | **string** | Brand domain, for citation matching. | 
 **aliases** | **string** | Comma-separated alternative names. | 
 **competitors** | **string** | Comma-separated competitor names. | 
 **country** | **string** | ISO-3166 alpha-2 egress country. | 

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


## PerplexityMeasureABrandSVisibilityInAPerplexityAnswerPost

> interface{} PerplexityMeasureABrandSVisibilityInAPerplexityAnswerPost(ctx).Execute()

Measure a brand's visibility in a Perplexity answer (POST)



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
	resp, r, err := apiClient.PerplexityAPI.PerplexityMeasureABrandSVisibilityInAPerplexityAnswerPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PerplexityAPI.PerplexityMeasureABrandSVisibilityInAPerplexityAnswerPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PerplexityMeasureABrandSVisibilityInAPerplexityAnswerPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `PerplexityAPI.PerplexityMeasureABrandSVisibilityInAPerplexityAnswerPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiPerplexityMeasureABrandSVisibilityInAPerplexityAnswerPostRequest struct via the builder pattern


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


## PerplexityPerplexityScraperHealthCheck

> interface{} PerplexityPerplexityScraperHealthCheck(ctx).Execute()

Perplexity scraper health check



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
	resp, r, err := apiClient.PerplexityAPI.PerplexityPerplexityScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PerplexityAPI.PerplexityPerplexityScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PerplexityPerplexityScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `PerplexityAPI.PerplexityPerplexityScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiPerplexityPerplexityScraperHealthCheckRequest struct via the builder pattern


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


## PerplexityPerplexityScraperHealthCheckHead

> interface{} PerplexityPerplexityScraperHealthCheckHead(ctx).Execute()

Perplexity scraper health check



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
	resp, r, err := apiClient.PerplexityAPI.PerplexityPerplexityScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PerplexityAPI.PerplexityPerplexityScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PerplexityPerplexityScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `PerplexityAPI.PerplexityPerplexityScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiPerplexityPerplexityScraperHealthCheckHeadRequest struct via the builder pattern


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


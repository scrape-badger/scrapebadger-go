# \CopilotAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CopilotAskCopilotAQuestion**](CopilotAPI.md#CopilotAskCopilotAQuestion) | **Get** /v1/copilot/ask | Ask Copilot a question
[**CopilotAskCopilotAQuestionPost**](CopilotAPI.md#CopilotAskCopilotAQuestionPost) | **Post** /v1/copilot/ask | Ask Copilot a question (POST)
[**CopilotCopilotScraperHealthCheck**](CopilotAPI.md#CopilotCopilotScraperHealthCheck) | **Get** /v1/copilot/health | Copilot scraper health check
[**CopilotCopilotScraperHealthCheckHead**](CopilotAPI.md#CopilotCopilotScraperHealthCheckHead) | **Head** /v1/copilot/health | Copilot scraper health check
[**CopilotListCopilotMarkets**](CopilotAPI.md#CopilotListCopilotMarkets) | **Get** /v1/copilot/markets | List Copilot markets
[**CopilotMeasureABrandSVisibilityInACopilotAnswer**](CopilotAPI.md#CopilotMeasureABrandSVisibilityInACopilotAnswer) | **Get** /v1/copilot/brand-visibility | Measure a brand&#39;s visibility in a Copilot answer
[**CopilotMeasureABrandSVisibilityInACopilotAnswerPost**](CopilotAPI.md#CopilotMeasureABrandSVisibilityInACopilotAnswerPost) | **Post** /v1/copilot/brand-visibility | Measure a brand&#39;s visibility in a Copilot answer (POST)



## CopilotAskCopilotAQuestion

> interface{} CopilotAskCopilotAQuestion(ctx).Prompt(prompt).Country(country).Market(market).StrictCountry(strictCountry).Execute()

Ask Copilot a question



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
	prompt := "prompt_example" // string | The prompt to send to Copilot (max 2000 characters).
	country := "country_example" // string | ISO-3166 alpha-2 country to ask from, e.g. 'JP', 'US', 'GB'. Unless `market` is set, Copilot also answers in that country's market. (optional)
	market := "market_example" // string | Bing market (language-COUNTRY), e.g. 'ja-JP', 'en-GB'. Defaults to the country's. (optional)
	strictCountry := true // bool | Answer only from an exit in `country`, never another one; 503 `country_unavailable` (not billed) when none answers. Requires `country`. (optional) (default to false)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CopilotAPI.CopilotAskCopilotAQuestion(context.Background()).Prompt(prompt).Country(country).Market(market).StrictCountry(strictCountry).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CopilotAPI.CopilotAskCopilotAQuestion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CopilotAskCopilotAQuestion`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `CopilotAPI.CopilotAskCopilotAQuestion`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCopilotAskCopilotAQuestionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **prompt** | **string** | The prompt to send to Copilot (max 2000 characters). | 
 **country** | **string** | ISO-3166 alpha-2 country to ask from, e.g. &#39;JP&#39;, &#39;US&#39;, &#39;GB&#39;. Unless &#x60;market&#x60; is set, Copilot also answers in that country&#39;s market. | 
 **market** | **string** | Bing market (language-COUNTRY), e.g. &#39;ja-JP&#39;, &#39;en-GB&#39;. Defaults to the country&#39;s. | 
 **strictCountry** | **bool** | Answer only from an exit in &#x60;country&#x60;, never another one; 503 &#x60;country_unavailable&#x60; (not billed) when none answers. Requires &#x60;country&#x60;. | [default to false]

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


## CopilotAskCopilotAQuestionPost

> interface{} CopilotAskCopilotAQuestionPost(ctx).Execute()

Ask Copilot a question (POST)



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
	resp, r, err := apiClient.CopilotAPI.CopilotAskCopilotAQuestionPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CopilotAPI.CopilotAskCopilotAQuestionPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CopilotAskCopilotAQuestionPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `CopilotAPI.CopilotAskCopilotAQuestionPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiCopilotAskCopilotAQuestionPostRequest struct via the builder pattern


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


## CopilotCopilotScraperHealthCheck

> interface{} CopilotCopilotScraperHealthCheck(ctx).Execute()

Copilot scraper health check



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
	resp, r, err := apiClient.CopilotAPI.CopilotCopilotScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CopilotAPI.CopilotCopilotScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CopilotCopilotScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `CopilotAPI.CopilotCopilotScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiCopilotCopilotScraperHealthCheckRequest struct via the builder pattern


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


## CopilotCopilotScraperHealthCheckHead

> interface{} CopilotCopilotScraperHealthCheckHead(ctx).Execute()

Copilot scraper health check



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
	resp, r, err := apiClient.CopilotAPI.CopilotCopilotScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CopilotAPI.CopilotCopilotScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CopilotCopilotScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `CopilotAPI.CopilotCopilotScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiCopilotCopilotScraperHealthCheckHeadRequest struct via the builder pattern


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


## CopilotListCopilotMarkets

> interface{} CopilotListCopilotMarkets(ctx).Execute()

List Copilot markets



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
	resp, r, err := apiClient.CopilotAPI.CopilotListCopilotMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CopilotAPI.CopilotListCopilotMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CopilotListCopilotMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `CopilotAPI.CopilotListCopilotMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiCopilotListCopilotMarketsRequest struct via the builder pattern


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


## CopilotMeasureABrandSVisibilityInACopilotAnswer

> interface{} CopilotMeasureABrandSVisibilityInACopilotAnswer(ctx).Prompt(prompt).Brand(brand).Domain(domain).Aliases(aliases).Competitors(competitors).Country(country).Market(market).StrictCountry(strictCountry).Execute()

Measure a brand's visibility in a Copilot answer



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
	prompt := "prompt_example" // string | The prompt to ask Copilot.
	brand := "brand_example" // string | Brand name to look for in the answer.
	domain := "domain_example" // string | Brand domain, for citation matching. (optional)
	aliases := "aliases_example" // string | Comma-separated alternative names. (optional)
	competitors := "competitors_example" // string | Comma-separated competitor names. (optional)
	country := "country_example" // string | ISO-3166 alpha-2 country to ask from, e.g. 'JP', 'US', 'GB'. Unless `market` is set, Copilot also answers in that country's market. (optional)
	market := "market_example" // string | Bing market (language-COUNTRY), e.g. 'ja-JP', 'en-GB'. Defaults to the country's. (optional)
	strictCountry := true // bool | Answer only from an exit in `country`, never another one; 503 `country_unavailable` (not billed) when none answers. Requires `country`. (optional) (default to false)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CopilotAPI.CopilotMeasureABrandSVisibilityInACopilotAnswer(context.Background()).Prompt(prompt).Brand(brand).Domain(domain).Aliases(aliases).Competitors(competitors).Country(country).Market(market).StrictCountry(strictCountry).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CopilotAPI.CopilotMeasureABrandSVisibilityInACopilotAnswer``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CopilotMeasureABrandSVisibilityInACopilotAnswer`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `CopilotAPI.CopilotMeasureABrandSVisibilityInACopilotAnswer`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCopilotMeasureABrandSVisibilityInACopilotAnswerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **prompt** | **string** | The prompt to ask Copilot. | 
 **brand** | **string** | Brand name to look for in the answer. | 
 **domain** | **string** | Brand domain, for citation matching. | 
 **aliases** | **string** | Comma-separated alternative names. | 
 **competitors** | **string** | Comma-separated competitor names. | 
 **country** | **string** | ISO-3166 alpha-2 country to ask from, e.g. &#39;JP&#39;, &#39;US&#39;, &#39;GB&#39;. Unless &#x60;market&#x60; is set, Copilot also answers in that country&#39;s market. | 
 **market** | **string** | Bing market (language-COUNTRY), e.g. &#39;ja-JP&#39;, &#39;en-GB&#39;. Defaults to the country&#39;s. | 
 **strictCountry** | **bool** | Answer only from an exit in &#x60;country&#x60;, never another one; 503 &#x60;country_unavailable&#x60; (not billed) when none answers. Requires &#x60;country&#x60;. | [default to false]

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


## CopilotMeasureABrandSVisibilityInACopilotAnswerPost

> interface{} CopilotMeasureABrandSVisibilityInACopilotAnswerPost(ctx).Execute()

Measure a brand's visibility in a Copilot answer (POST)



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
	resp, r, err := apiClient.CopilotAPI.CopilotMeasureABrandSVisibilityInACopilotAnswerPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CopilotAPI.CopilotMeasureABrandSVisibilityInACopilotAnswerPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CopilotMeasureABrandSVisibilityInACopilotAnswerPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `CopilotAPI.CopilotMeasureABrandSVisibilityInACopilotAnswerPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiCopilotMeasureABrandSVisibilityInACopilotAnswerPostRequest struct via the builder pattern


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


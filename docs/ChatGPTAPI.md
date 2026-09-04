# \ChatGPTAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ChatgptAskChatgptAQuestion**](ChatGPTAPI.md#ChatgptAskChatgptAQuestion) | **Get** /v1/chatgpt/ask | Ask ChatGPT a question
[**ChatgptAskChatgptAQuestionPost**](ChatGPTAPI.md#ChatgptAskChatgptAQuestionPost) | **Post** /v1/chatgpt/ask | Ask ChatGPT a question (POST)
[**ChatgptChatgptScraperHealthCheck**](ChatGPTAPI.md#ChatgptChatgptScraperHealthCheck) | **Get** /v1/chatgpt/health | ChatGPT scraper health check
[**ChatgptChatgptScraperHealthCheckHead**](ChatGPTAPI.md#ChatgptChatgptScraperHealthCheckHead) | **Head** /v1/chatgpt/health | ChatGPT scraper health check
[**ChatgptListChatgptModels**](ChatGPTAPI.md#ChatgptListChatgptModels) | **Get** /v1/chatgpt/models | List ChatGPT models
[**ChatgptMeasureABrandSVisibilityInAChatgptAnswer**](ChatGPTAPI.md#ChatgptMeasureABrandSVisibilityInAChatgptAnswer) | **Get** /v1/chatgpt/brand-visibility | Measure a brand&#39;s visibility in a ChatGPT answer
[**ChatgptMeasureABrandSVisibilityInAChatgptAnswerPost**](ChatGPTAPI.md#ChatgptMeasureABrandSVisibilityInAChatgptAnswerPost) | **Post** /v1/chatgpt/brand-visibility | Measure a brand&#39;s visibility in a ChatGPT answer (POST)



## ChatgptAskChatgptAQuestion

> interface{} ChatgptAskChatgptAQuestion(ctx).Prompt(prompt).Country(country).WebSearch(webSearch).ImageUrl(imageUrl).Execute()

Ask ChatGPT a question



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
	prompt := "prompt_example" // string | The prompt to send to ChatGPT (max 4096 characters).
	country := "country_example" // string | ISO-3166 alpha-2 egress country, e.g. 'US', 'GB', 'DE'. (optional)
	webSearch := "webSearch_example" // string | auto (let ChatGPT decide) | force (ask it to browse) | off (answer from memory). `web_search_triggered` in the response always reports what actually happened. (optional) (default to "auto")
	imageUrl := "imageUrl_example" // string | Public http(s) URL of an image to attach to the prompt. ChatGPT reads it and answers about it. POST also accepts `image_base64`. Exactly one of the two. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChatGPTAPI.ChatgptAskChatgptAQuestion(context.Background()).Prompt(prompt).Country(country).WebSearch(webSearch).ImageUrl(imageUrl).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatGPTAPI.ChatgptAskChatgptAQuestion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatgptAskChatgptAQuestion`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ChatGPTAPI.ChatgptAskChatgptAQuestion`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiChatgptAskChatgptAQuestionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **prompt** | **string** | The prompt to send to ChatGPT (max 4096 characters). | 
 **country** | **string** | ISO-3166 alpha-2 egress country, e.g. &#39;US&#39;, &#39;GB&#39;, &#39;DE&#39;. | 
 **webSearch** | **string** | auto (let ChatGPT decide) | force (ask it to browse) | off (answer from memory). &#x60;web_search_triggered&#x60; in the response always reports what actually happened. | [default to &quot;auto&quot;]
 **imageUrl** | **string** | Public http(s) URL of an image to attach to the prompt. ChatGPT reads it and answers about it. POST also accepts &#x60;image_base64&#x60;. Exactly one of the two. | 

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


## ChatgptAskChatgptAQuestionPost

> interface{} ChatgptAskChatgptAQuestionPost(ctx).Execute()

Ask ChatGPT a question (POST)



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
	resp, r, err := apiClient.ChatGPTAPI.ChatgptAskChatgptAQuestionPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatGPTAPI.ChatgptAskChatgptAQuestionPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatgptAskChatgptAQuestionPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ChatGPTAPI.ChatgptAskChatgptAQuestionPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiChatgptAskChatgptAQuestionPostRequest struct via the builder pattern


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


## ChatgptChatgptScraperHealthCheck

> interface{} ChatgptChatgptScraperHealthCheck(ctx).Execute()

ChatGPT scraper health check



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
	resp, r, err := apiClient.ChatGPTAPI.ChatgptChatgptScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatGPTAPI.ChatgptChatgptScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatgptChatgptScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ChatGPTAPI.ChatgptChatgptScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiChatgptChatgptScraperHealthCheckRequest struct via the builder pattern


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


## ChatgptChatgptScraperHealthCheckHead

> interface{} ChatgptChatgptScraperHealthCheckHead(ctx).Execute()

ChatGPT scraper health check



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
	resp, r, err := apiClient.ChatGPTAPI.ChatgptChatgptScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatGPTAPI.ChatgptChatgptScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatgptChatgptScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ChatGPTAPI.ChatgptChatgptScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiChatgptChatgptScraperHealthCheckHeadRequest struct via the builder pattern


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


## ChatgptListChatgptModels

> interface{} ChatgptListChatgptModels(ctx).Country(country).Execute()

List ChatGPT models



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
	country := "country_example" // string | ISO-3166 alpha-2 egress country. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChatGPTAPI.ChatgptListChatgptModels(context.Background()).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatGPTAPI.ChatgptListChatgptModels``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatgptListChatgptModels`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ChatGPTAPI.ChatgptListChatgptModels`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiChatgptListChatgptModelsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
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


## ChatgptMeasureABrandSVisibilityInAChatgptAnswer

> interface{} ChatgptMeasureABrandSVisibilityInAChatgptAnswer(ctx).Prompt(prompt).Brand(brand).Domain(domain).Aliases(aliases).Competitors(competitors).Country(country).WebSearch(webSearch).Execute()

Measure a brand's visibility in a ChatGPT answer



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
	prompt := "prompt_example" // string | The prompt to ask ChatGPT.
	brand := "brand_example" // string | Brand name to look for in the answer.
	domain := "domain_example" // string | Brand domain, for citation matching. (optional)
	aliases := "aliases_example" // string | Comma-separated alternative names. (optional)
	competitors := "competitors_example" // string | Comma-separated competitor names. (optional)
	country := "country_example" // string | ISO-3166 alpha-2 egress country. (optional)
	webSearch := "webSearch_example" // string | auto | force | off (optional) (default to "force")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChatGPTAPI.ChatgptMeasureABrandSVisibilityInAChatgptAnswer(context.Background()).Prompt(prompt).Brand(brand).Domain(domain).Aliases(aliases).Competitors(competitors).Country(country).WebSearch(webSearch).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatGPTAPI.ChatgptMeasureABrandSVisibilityInAChatgptAnswer``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatgptMeasureABrandSVisibilityInAChatgptAnswer`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ChatGPTAPI.ChatgptMeasureABrandSVisibilityInAChatgptAnswer`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiChatgptMeasureABrandSVisibilityInAChatgptAnswerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **prompt** | **string** | The prompt to ask ChatGPT. | 
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


## ChatgptMeasureABrandSVisibilityInAChatgptAnswerPost

> interface{} ChatgptMeasureABrandSVisibilityInAChatgptAnswerPost(ctx).Execute()

Measure a brand's visibility in a ChatGPT answer (POST)



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
	resp, r, err := apiClient.ChatGPTAPI.ChatgptMeasureABrandSVisibilityInAChatgptAnswerPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChatGPTAPI.ChatgptMeasureABrandSVisibilityInAChatgptAnswerPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ChatgptMeasureABrandSVisibilityInAChatgptAnswerPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ChatGPTAPI.ChatgptMeasureABrandSVisibilityInAChatgptAnswerPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiChatgptMeasureABrandSVisibilityInAChatgptAnswerPostRequest struct via the builder pattern


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


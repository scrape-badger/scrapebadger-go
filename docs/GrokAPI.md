# \GrokAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GrokAskGrokAQuestion**](GrokAPI.md#GrokAskGrokAQuestion) | **Get** /v1/grok/ask | Ask Grok a question
[**GrokAskGrokAQuestionPost**](GrokAPI.md#GrokAskGrokAQuestionPost) | **Post** /v1/grok/ask | Ask Grok a question (POST)
[**GrokGetAGrokConversation**](GrokAPI.md#GrokGetAGrokConversation) | **Get** /v1/grok/conversations/{conversation_id} | Get a Grok conversation
[**GrokGrokScraperHealthCheck**](GrokAPI.md#GrokGrokScraperHealthCheck) | **Get** /v1/grok/health | Grok scraper health check
[**GrokGrokScraperHealthCheckHead**](GrokAPI.md#GrokGrokScraperHealthCheckHead) | **Head** /v1/grok/health | Grok scraper health check
[**GrokListGrokAssistantModes**](GrokAPI.md#GrokListGrokAssistantModes) | **Get** /v1/grok/models | List Grok assistant modes
[**GrokMeasureBrandVisibilityInGrok**](GrokAPI.md#GrokMeasureBrandVisibilityInGrok) | **Get** /v1/grok/brand-visibility | Measure brand visibility in Grok
[**GrokMeasureBrandVisibilityInGrokPost**](GrokAPI.md#GrokMeasureBrandVisibilityInGrokPost) | **Post** /v1/grok/brand-visibility | Measure brand visibility in Grok (POST)



## GrokAskGrokAQuestion

> interface{} GrokAskGrokAQuestion(ctx).Prompt(prompt).ConversationId(conversationId).Mode(mode).WebSearch(webSearch).Execute()

Ask Grok a question



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
	prompt := "prompt_example" // string | Prompt to send to Grok (max 4000 characters).
	conversationId := "conversationId_example" // string | Existing Grok conversation to continue. (optional)
	mode := "mode_example" // string | Assistant mode: auto, fast, or expert. (optional) (default to "auto")
	webSearch := "webSearch_example" // string | Web and X search: auto, force, or off. (optional) (default to "auto")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GrokAPI.GrokAskGrokAQuestion(context.Background()).Prompt(prompt).ConversationId(conversationId).Mode(mode).WebSearch(webSearch).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GrokAPI.GrokAskGrokAQuestion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GrokAskGrokAQuestion`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GrokAPI.GrokAskGrokAQuestion`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGrokAskGrokAQuestionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **prompt** | **string** | Prompt to send to Grok (max 4000 characters). | 
 **conversationId** | **string** | Existing Grok conversation to continue. | 
 **mode** | **string** | Assistant mode: auto, fast, or expert. | [default to &quot;auto&quot;]
 **webSearch** | **string** | Web and X search: auto, force, or off. | [default to &quot;auto&quot;]

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


## GrokAskGrokAQuestionPost

> interface{} GrokAskGrokAQuestionPost(ctx).Execute()

Ask Grok a question (POST)

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
	resp, r, err := apiClient.GrokAPI.GrokAskGrokAQuestionPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GrokAPI.GrokAskGrokAQuestionPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GrokAskGrokAQuestionPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GrokAPI.GrokAskGrokAQuestionPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGrokAskGrokAQuestionPostRequest struct via the builder pattern


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


## GrokGetAGrokConversation

> interface{} GrokGetAGrokConversation(ctx, conversationId).Execute()

Get a Grok conversation

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
	conversationId := "conversationId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GrokAPI.GrokGetAGrokConversation(context.Background(), conversationId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GrokAPI.GrokGetAGrokConversation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GrokGetAGrokConversation`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GrokAPI.GrokGetAGrokConversation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**conversationId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGrokGetAGrokConversationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


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


## GrokGrokScraperHealthCheck

> interface{} GrokGrokScraperHealthCheck(ctx).Execute()

Grok scraper health check

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
	resp, r, err := apiClient.GrokAPI.GrokGrokScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GrokAPI.GrokGrokScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GrokGrokScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GrokAPI.GrokGrokScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGrokGrokScraperHealthCheckRequest struct via the builder pattern


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


## GrokGrokScraperHealthCheckHead

> interface{} GrokGrokScraperHealthCheckHead(ctx).Execute()

Grok scraper health check

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
	resp, r, err := apiClient.GrokAPI.GrokGrokScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GrokAPI.GrokGrokScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GrokGrokScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GrokAPI.GrokGrokScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGrokGrokScraperHealthCheckHeadRequest struct via the builder pattern


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


## GrokListGrokAssistantModes

> interface{} GrokListGrokAssistantModes(ctx).Execute()

List Grok assistant modes

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
	resp, r, err := apiClient.GrokAPI.GrokListGrokAssistantModes(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GrokAPI.GrokListGrokAssistantModes``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GrokListGrokAssistantModes`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GrokAPI.GrokListGrokAssistantModes`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGrokListGrokAssistantModesRequest struct via the builder pattern


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


## GrokMeasureBrandVisibilityInGrok

> interface{} GrokMeasureBrandVisibilityInGrok(ctx).Prompt(prompt).Brand(brand).Competitors(competitors).BrandDomain(brandDomain).Mode(mode).WebSearch(webSearch).Execute()

Measure brand visibility in Grok

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
	prompt := "prompt_example" // string | Buyer or category prompt to send to Grok.
	brand := "brand_example" // string | Brand name to measure.
	competitors := []*string{"Inner_example"} // []*string | Competitor brand names. (optional) (default to [])
	brandDomain := "brandDomain_example" // string | Brand domain for citation rank. (optional)
	mode := "mode_example" // string | Assistant mode: auto, fast, or expert. (optional) (default to "auto")
	webSearch := "webSearch_example" // string | Web and X search mode. (optional) (default to "force")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GrokAPI.GrokMeasureBrandVisibilityInGrok(context.Background()).Prompt(prompt).Brand(brand).Competitors(competitors).BrandDomain(brandDomain).Mode(mode).WebSearch(webSearch).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GrokAPI.GrokMeasureBrandVisibilityInGrok``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GrokMeasureBrandVisibilityInGrok`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GrokAPI.GrokMeasureBrandVisibilityInGrok`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGrokMeasureBrandVisibilityInGrokRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **prompt** | **string** | Buyer or category prompt to send to Grok. | 
 **brand** | **string** | Brand name to measure. | 
 **competitors** | **[]string** | Competitor brand names. | [default to []]
 **brandDomain** | **string** | Brand domain for citation rank. | 
 **mode** | **string** | Assistant mode: auto, fast, or expert. | [default to &quot;auto&quot;]
 **webSearch** | **string** | Web and X search mode. | [default to &quot;force&quot;]

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


## GrokMeasureBrandVisibilityInGrokPost

> interface{} GrokMeasureBrandVisibilityInGrokPost(ctx).Execute()

Measure brand visibility in Grok (POST)

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
	resp, r, err := apiClient.GrokAPI.GrokMeasureBrandVisibilityInGrokPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GrokAPI.GrokMeasureBrandVisibilityInGrokPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GrokMeasureBrandVisibilityInGrokPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GrokAPI.GrokMeasureBrandVisibilityInGrokPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGrokMeasureBrandVisibilityInGrokPostRequest struct via the builder pattern


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


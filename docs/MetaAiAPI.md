# \MetaAiAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**MetaAiAskMetaAiAQuestion**](MetaAiAPI.md#MetaAiAskMetaAiAQuestion) | **Get** /v1/meta-ai/ask | Ask Meta AI a question
[**MetaAiAskMetaAiAQuestionPost**](MetaAiAPI.md#MetaAiAskMetaAiAQuestionPost) | **Post** /v1/meta-ai/ask | Ask Meta AI a question (POST)
[**MetaAiListMetaAiAssistantModes**](MetaAiAPI.md#MetaAiListMetaAiAssistantModes) | **Get** /v1/meta-ai/models | List Meta AI assistant modes
[**MetaAiMetaAiScraperHealthCheck**](MetaAiAPI.md#MetaAiMetaAiScraperHealthCheck) | **Get** /v1/meta-ai/health | Meta AI scraper health check
[**MetaAiMetaAiScraperHealthCheckHead**](MetaAiAPI.md#MetaAiMetaAiScraperHealthCheckHead) | **Head** /v1/meta-ai/health | Meta AI scraper health check



## MetaAiAskMetaAiAQuestion

> interface{} MetaAiAskMetaAiAQuestion(ctx).Prompt(prompt).Country(country).Execute()

Ask Meta AI a question



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
	prompt := "prompt_example" // string | The prompt to send to Meta AI (max 4000 characters).
	country := "country_example" // string | ISO-3166 alpha-2 egress country, e.g. 'US', 'GB', 'DE'. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MetaAiAPI.MetaAiAskMetaAiAQuestion(context.Background()).Prompt(prompt).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MetaAiAPI.MetaAiAskMetaAiAQuestion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MetaAiAskMetaAiAQuestion`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `MetaAiAPI.MetaAiAskMetaAiAQuestion`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiMetaAiAskMetaAiAQuestionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **prompt** | **string** | The prompt to send to Meta AI (max 4000 characters). | 
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


## MetaAiAskMetaAiAQuestionPost

> interface{} MetaAiAskMetaAiAQuestionPost(ctx).Execute()

Ask Meta AI a question (POST)



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
	resp, r, err := apiClient.MetaAiAPI.MetaAiAskMetaAiAQuestionPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MetaAiAPI.MetaAiAskMetaAiAQuestionPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MetaAiAskMetaAiAQuestionPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `MetaAiAPI.MetaAiAskMetaAiAQuestionPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiMetaAiAskMetaAiAQuestionPostRequest struct via the builder pattern


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


## MetaAiListMetaAiAssistantModes

> interface{} MetaAiListMetaAiAssistantModes(ctx).Country(country).Execute()

List Meta AI assistant modes



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
	resp, r, err := apiClient.MetaAiAPI.MetaAiListMetaAiAssistantModes(context.Background()).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MetaAiAPI.MetaAiListMetaAiAssistantModes``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MetaAiListMetaAiAssistantModes`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `MetaAiAPI.MetaAiListMetaAiAssistantModes`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiMetaAiListMetaAiAssistantModesRequest struct via the builder pattern


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


## MetaAiMetaAiScraperHealthCheck

> interface{} MetaAiMetaAiScraperHealthCheck(ctx).Execute()

Meta AI scraper health check



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
	resp, r, err := apiClient.MetaAiAPI.MetaAiMetaAiScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MetaAiAPI.MetaAiMetaAiScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MetaAiMetaAiScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `MetaAiAPI.MetaAiMetaAiScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiMetaAiMetaAiScraperHealthCheckRequest struct via the builder pattern


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


## MetaAiMetaAiScraperHealthCheckHead

> interface{} MetaAiMetaAiScraperHealthCheckHead(ctx).Execute()

Meta AI scraper health check



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
	resp, r, err := apiClient.MetaAiAPI.MetaAiMetaAiScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MetaAiAPI.MetaAiMetaAiScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MetaAiMetaAiScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `MetaAiAPI.MetaAiMetaAiScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiMetaAiMetaAiScraperHealthCheckHeadRequest struct via the builder pattern


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


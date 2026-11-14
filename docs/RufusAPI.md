# \RufusAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**RufusAmazonRufusScraperHealthCheck**](RufusAPI.md#RufusAmazonRufusScraperHealthCheck) | **Get** /v1/rufus/health | Amazon Rufus scraper health check
[**RufusAmazonRufusScraperHealthCheckHead**](RufusAPI.md#RufusAmazonRufusScraperHealthCheckHead) | **Head** /v1/rufus/health | Amazon Rufus scraper health check
[**RufusAskAmazonRufusAQuestion**](RufusAPI.md#RufusAskAmazonRufusAQuestion) | **Get** /v1/rufus/ask | Ask Amazon Rufus a question
[**RufusAskAmazonRufusAQuestionPost**](RufusAPI.md#RufusAskAmazonRufusAQuestionPost) | **Post** /v1/rufus/ask | Ask Amazon Rufus a question (POST)
[**RufusListAmazonRufusModels**](RufusAPI.md#RufusListAmazonRufusModels) | **Get** /v1/rufus/models | List Amazon Rufus models



## RufusAmazonRufusScraperHealthCheck

> interface{} RufusAmazonRufusScraperHealthCheck(ctx).Execute()

Amazon Rufus scraper health check



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
	resp, r, err := apiClient.RufusAPI.RufusAmazonRufusScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RufusAPI.RufusAmazonRufusScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RufusAmazonRufusScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RufusAPI.RufusAmazonRufusScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiRufusAmazonRufusScraperHealthCheckRequest struct via the builder pattern


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


## RufusAmazonRufusScraperHealthCheckHead

> interface{} RufusAmazonRufusScraperHealthCheckHead(ctx).Execute()

Amazon Rufus scraper health check



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
	resp, r, err := apiClient.RufusAPI.RufusAmazonRufusScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RufusAPI.RufusAmazonRufusScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RufusAmazonRufusScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RufusAPI.RufusAmazonRufusScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiRufusAmazonRufusScraperHealthCheckHeadRequest struct via the builder pattern


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


## RufusAskAmazonRufusAQuestion

> interface{} RufusAskAmazonRufusAQuestion(ctx).Prompt(prompt).Asin(asin).Execute()

Ask Amazon Rufus a question



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
	prompt := "prompt_example" // string | The shopping question to ask (max 4000 characters).
	asin := "asin_example" // string | Optional product ASIN whose page should provide the shopping context. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RufusAPI.RufusAskAmazonRufusAQuestion(context.Background()).Prompt(prompt).Asin(asin).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RufusAPI.RufusAskAmazonRufusAQuestion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RufusAskAmazonRufusAQuestion`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RufusAPI.RufusAskAmazonRufusAQuestion`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRufusAskAmazonRufusAQuestionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **prompt** | **string** | The shopping question to ask (max 4000 characters). | 
 **asin** | **string** | Optional product ASIN whose page should provide the shopping context. | 

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


## RufusAskAmazonRufusAQuestionPost

> interface{} RufusAskAmazonRufusAQuestionPost(ctx).RufusAskRequest(rufusAskRequest).Execute()

Ask Amazon Rufus a question (POST)



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
	rufusAskRequest := *openapiclient.NewRufusAskRequest("Prompt_example") // RufusAskRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RufusAPI.RufusAskAmazonRufusAQuestionPost(context.Background()).RufusAskRequest(rufusAskRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RufusAPI.RufusAskAmazonRufusAQuestionPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RufusAskAmazonRufusAQuestionPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RufusAPI.RufusAskAmazonRufusAQuestionPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRufusAskAmazonRufusAQuestionPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rufusAskRequest** | [**RufusAskRequest**](RufusAskRequest.md) |  | 

### Return type

**interface{}**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RufusListAmazonRufusModels

> interface{} RufusListAmazonRufusModels(ctx).Execute()

List Amazon Rufus models



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
	resp, r, err := apiClient.RufusAPI.RufusListAmazonRufusModels(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RufusAPI.RufusListAmazonRufusModels``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RufusListAmazonRufusModels`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RufusAPI.RufusListAmazonRufusModels`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiRufusListAmazonRufusModelsRequest struct via the builder pattern


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


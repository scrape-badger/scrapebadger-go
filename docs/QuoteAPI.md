# \QuoteAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**QuoteQuoteACall**](QuoteAPI.md#QuoteQuoteACall) | **Post** /v1/quote | Quote a call



## QuoteQuoteACall

> interface{} QuoteQuoteACall(ctx).QuoteRequest(quoteRequest).Execute()

Quote a call



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
	quoteRequest := *openapiclient.NewQuoteRequest("Path_example") // QuoteRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.QuoteAPI.QuoteQuoteACall(context.Background()).QuoteRequest(quoteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `QuoteAPI.QuoteQuoteACall``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `QuoteQuoteACall`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `QuoteAPI.QuoteQuoteACall`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiQuoteQuoteACallRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quoteRequest** | [**QuoteRequest**](QuoteRequest.md) |  | 

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


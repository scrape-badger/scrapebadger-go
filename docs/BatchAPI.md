# \BatchAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**BatchSubmitABatchOfAsyncRequests**](BatchAPI.md#BatchSubmitABatchOfAsyncRequests) | **Post** /v1/batch | Submit a batch of async requests



## BatchSubmitABatchOfAsyncRequests

> interface{} BatchSubmitABatchOfAsyncRequests(ctx).BatchRequest(batchRequest).Execute()

Submit a batch of async requests



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
	batchRequest := *openapiclient.NewBatchRequest([]openapiclient.BatchItem{*openapiclient.NewBatchItem("Path_example")}) // BatchRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BatchAPI.BatchSubmitABatchOfAsyncRequests(context.Background()).BatchRequest(batchRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BatchAPI.BatchSubmitABatchOfAsyncRequests``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BatchSubmitABatchOfAsyncRequests`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BatchAPI.BatchSubmitABatchOfAsyncRequests`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBatchSubmitABatchOfAsyncRequestsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **batchRequest** | [**BatchRequest**](BatchRequest.md) |  | 

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


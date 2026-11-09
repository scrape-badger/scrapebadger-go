# \ResultsAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ResultsReReadAResultRemoved**](ResultsAPI.md#ResultsReReadAResultRemoved) | **Get** /v1/results/{result_id} | Re-read a result (removed)



## ResultsReReadAResultRemoved

> interface{} ResultsReReadAResultRemoved(ctx, resultId).Execute()

Re-read a result (removed)



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
	resultId := "resultId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ResultsAPI.ResultsReReadAResultRemoved(context.Background(), resultId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ResultsAPI.ResultsReReadAResultRemoved``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ResultsReReadAResultRemoved`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ResultsAPI.ResultsReReadAResultRemoved`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**resultId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiResultsReReadAResultRemovedRequest struct via the builder pattern


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


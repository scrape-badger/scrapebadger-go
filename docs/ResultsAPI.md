# \ResultsAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ResultsReReadAResult**](ResultsAPI.md#ResultsReReadAResult) | **Get** /v1/results/{result_id} | Re-read a result



## ResultsReReadAResult

> interface{} ResultsReReadAResult(ctx, resultId).Execute()

Re-read a result



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
	resp, r, err := apiClient.ResultsAPI.ResultsReReadAResult(context.Background(), resultId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ResultsAPI.ResultsReReadAResult``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ResultsReReadAResult`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ResultsAPI.ResultsReReadAResult`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**resultId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiResultsReReadAResultRequest struct via the builder pattern


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


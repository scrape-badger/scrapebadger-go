# \FeedbackAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**FeedbackReportABugOrSendFeedback**](FeedbackAPI.md#FeedbackReportABugOrSendFeedback) | **Post** /v1/feedback | Report a bug or send feedback



## FeedbackReportABugOrSendFeedback

> interface{} FeedbackReportABugOrSendFeedback(ctx).FeedbackRequest(feedbackRequest).Execute()

Report a bug or send feedback



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
	feedbackRequest := *openapiclient.NewFeedbackRequest("Type_example", "Summary_example") // FeedbackRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FeedbackAPI.FeedbackReportABugOrSendFeedback(context.Background()).FeedbackRequest(feedbackRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FeedbackAPI.FeedbackReportABugOrSendFeedback``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FeedbackReportABugOrSendFeedback`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FeedbackAPI.FeedbackReportABugOrSendFeedback`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiFeedbackReportABugOrSendFeedbackRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **feedbackRequest** | [**FeedbackRequest**](FeedbackRequest.md) |  | 

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


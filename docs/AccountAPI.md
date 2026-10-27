# \AccountAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AccountGetAccountInfo**](AccountAPI.md#AccountGetAccountInfo) | **Get** /v1/account/me | Get account info
[**AccountGetTheWebhookSigningSecret**](AccountAPI.md#AccountGetTheWebhookSigningSecret) | **Get** /v1/account/webhook-secret | Get the webhook signing secret
[**AccountRotateTheWebhookSigningSecret**](AccountAPI.md#AccountRotateTheWebhookSigningSecret) | **Post** /v1/account/webhook-secret/rotate | Rotate the webhook signing secret



## AccountGetAccountInfo

> AccountInfo AccountGetAccountInfo(ctx).Execute()

Get account info



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
	resp, r, err := apiClient.AccountAPI.AccountGetAccountInfo(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AccountAPI.AccountGetAccountInfo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AccountGetAccountInfo`: AccountInfo
	fmt.Fprintf(os.Stdout, "Response from `AccountAPI.AccountGetAccountInfo`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAccountGetAccountInfoRequest struct via the builder pattern


### Return type

[**AccountInfo**](AccountInfo.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AccountGetTheWebhookSigningSecret

> WebhookSecret AccountGetTheWebhookSigningSecret(ctx).Execute()

Get the webhook signing secret



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
	resp, r, err := apiClient.AccountAPI.AccountGetTheWebhookSigningSecret(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AccountAPI.AccountGetTheWebhookSigningSecret``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AccountGetTheWebhookSigningSecret`: WebhookSecret
	fmt.Fprintf(os.Stdout, "Response from `AccountAPI.AccountGetTheWebhookSigningSecret`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAccountGetTheWebhookSigningSecretRequest struct via the builder pattern


### Return type

[**WebhookSecret**](WebhookSecret.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AccountRotateTheWebhookSigningSecret

> WebhookSecret AccountRotateTheWebhookSigningSecret(ctx).Execute()

Rotate the webhook signing secret



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
	resp, r, err := apiClient.AccountAPI.AccountRotateTheWebhookSigningSecret(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AccountAPI.AccountRotateTheWebhookSigningSecret``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AccountRotateTheWebhookSigningSecret`: WebhookSecret
	fmt.Fprintf(os.Stdout, "Response from `AccountAPI.AccountRotateTheWebhookSigningSecret`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAccountRotateTheWebhookSigningSecretRequest struct via the builder pattern


### Return type

[**WebhookSecret**](WebhookSecret.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


# \GooglePlayAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GooglePlayBrowseACategory**](GooglePlayAPI.md#GooglePlayBrowseACategory) | **Get** /v1/google-play/categories/{category_id} | Browse a category
[**GooglePlayGetAppDetail**](GooglePlayAPI.md#GooglePlayGetAppDetail) | **Get** /v1/google-play/apps/{app_id} | Get app detail
[**GooglePlayGetAppPermissions**](GooglePlayAPI.md#GooglePlayGetAppPermissions) | **Get** /v1/google-play/apps/{app_id}/permissions | Get app permissions
[**GooglePlayGetAppReviews**](GooglePlayAPI.md#GooglePlayGetAppReviews) | **Get** /v1/google-play/apps/{app_id}/reviews | Get app reviews
[**GooglePlayGetDeveloperApps**](GooglePlayAPI.md#GooglePlayGetDeveloperApps) | **Get** /v1/google-play/developers/{developer} | Get developer apps
[**GooglePlayGetSimilarApps**](GooglePlayAPI.md#GooglePlayGetSimilarApps) | **Get** /v1/google-play/apps/{app_id}/similar | Get similar apps
[**GooglePlayListCategories**](GooglePlayAPI.md#GooglePlayListCategories) | **Get** /v1/google-play/categories | List categories
[**GooglePlayListMarkets**](GooglePlayAPI.md#GooglePlayListMarkets) | **Get** /v1/google-play/markets | List markets
[**GooglePlaySearchApps**](GooglePlayAPI.md#GooglePlaySearchApps) | **Get** /v1/google-play/search | Search apps
[**GooglePlayTopCharts**](GooglePlayAPI.md#GooglePlayTopCharts) | **Get** /v1/google-play/collections/{collection} | Top charts



## GooglePlayBrowseACategory

> interface{} GooglePlayBrowseACategory(ctx, categoryId).Country(country).Lang(lang).Num(num).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()

Browse a category



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
	categoryId := "categoryId_example" // string | Play category id, e.g. 'GAME_PUZZLE' or 'SOCIAL'
	country := "country_example" // string | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. 'US' (optional) (default to "US")
	lang := "lang_example" // string | Play content language (hl), e.g. 'en' or 'pt-BR' (optional) (default to "en")
	num := int32(56) // int32 | Max apps; follows each rail's 'see more' continuation above the ~40-120 the page renders directly (optional) (default to 100)
	prefer := "respond-async, wait=25" // string | `respond-async[, wait=N]` (RFC 7240): run the call async. If it has not finished after `wait` seconds (0-120, default 25) the answer is `202` with a `request_id`; poll `GET /v1/requests/{request_id}`. Its `wait=` wins over `async_wait`; without one, `async_wait` sets the wait. (optional)
	xCallbackURL := "xCallbackURL_example" // string | An `https` URL that receives the signed `request.completed` webhook when the call finishes. Implies async: on its own (no `Prefer`, `async` or `async_wait`) the answer is an immediate `202`; with `Prefer: respond-async` or `async=true` the call still waits 25 s unless a wait is given. Wins over `callback_url`. (optional)
	idempotencyKey := "idempotencyKey_example" // string | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call's current state (`Idempotent-Replayed: true`) without running or billing it again; on a different call it is `409 idempotency_key_reused`. Applies to async calls only; on a synchronous call it is ignored. Wins over `idempotency_key`. (optional)
	async := true // bool | Query form of `Prefer: respond-async`: `true` or `1` (also `yes`, `on`; `false`, `0`, `no`, `off` leave the call synchronous). Waits 25 s unless `async_wait` is given. Not sent to the scraper. (optional)
	asyncWait := int32(56) // int32 | Seconds (0-120; values outside are clamped) to wait for the result before answering `202`. Implies async. Not sent to the scraper. (optional)
	callbackUrl := "callbackUrl_example" // string | Query form of `X-Callback-URL` (URL-encode it). Implies async; on its own the answer is an immediate `202` (wait 0). Not sent to the scraper. (optional)
	idempotencyKey2 := "idempotencyKey_example" // string | Query form of `Idempotency-Key`. Not sent to the scraper. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayBrowseACategory(context.Background(), categoryId).Country(country).Lang(lang).Num(num).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayBrowseACategory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayBrowseACategory`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayBrowseACategory`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**categoryId** | **string** | Play category id, e.g. &#39;GAME_PUZZLE&#39; or &#39;SOCIAL&#39; | 

### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayBrowseACategoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. &#39;US&#39; | [default to &quot;US&quot;]
 **lang** | **string** | Play content language (hl), e.g. &#39;en&#39; or &#39;pt-BR&#39; | [default to &quot;en&quot;]
 **num** | **int32** | Max apps; follows each rail&#39;s &#39;see more&#39; continuation above the ~40-120 the page renders directly | [default to 100]
 **prefer** | **string** | &#x60;respond-async[, wait&#x3D;N]&#x60; (RFC 7240): run the call async. If it has not finished after &#x60;wait&#x60; seconds (0-120, default 25) the answer is &#x60;202&#x60; with a &#x60;request_id&#x60;; poll &#x60;GET /v1/requests/{request_id}&#x60;. Its &#x60;wait&#x3D;&#x60; wins over &#x60;async_wait&#x60;; without one, &#x60;async_wait&#x60; sets the wait. | 
 **xCallbackURL** | **string** | An &#x60;https&#x60; URL that receives the signed &#x60;request.completed&#x60; webhook when the call finishes. Implies async: on its own (no &#x60;Prefer&#x60;, &#x60;async&#x60; or &#x60;async_wait&#x60;) the answer is an immediate &#x60;202&#x60;; with &#x60;Prefer: respond-async&#x60; or &#x60;async&#x3D;true&#x60; the call still waits 25 s unless a wait is given. Wins over &#x60;callback_url&#x60;. | 
 **idempotencyKey** | **string** | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call&#39;s current state (&#x60;Idempotent-Replayed: true&#x60;) without running or billing it again; on a different call it is &#x60;409 idempotency_key_reused&#x60;. Applies to async calls only; on a synchronous call it is ignored. Wins over &#x60;idempotency_key&#x60;. | 
 **async** | **bool** | Query form of &#x60;Prefer: respond-async&#x60;: &#x60;true&#x60; or &#x60;1&#x60; (also &#x60;yes&#x60;, &#x60;on&#x60;; &#x60;false&#x60;, &#x60;0&#x60;, &#x60;no&#x60;, &#x60;off&#x60; leave the call synchronous). Waits 25 s unless &#x60;async_wait&#x60; is given. Not sent to the scraper. | 
 **asyncWait** | **int32** | Seconds (0-120; values outside are clamped) to wait for the result before answering &#x60;202&#x60;. Implies async. Not sent to the scraper. | 
 **callbackUrl** | **string** | Query form of &#x60;X-Callback-URL&#x60; (URL-encode it). Implies async; on its own the answer is an immediate &#x60;202&#x60; (wait 0). Not sent to the scraper. | 
 **idempotencyKey2** | **string** | Query form of &#x60;Idempotency-Key&#x60;. Not sent to the scraper. | 

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


## GooglePlayGetAppDetail

> interface{} GooglePlayGetAppDetail(ctx, appId).Country(country).Lang(lang).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()

Get app detail



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
	appId := "appId_example" // string | Android package id, e.g. 'com.whatsapp'.
	country := "country_example" // string | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. 'US' (optional) (default to "US")
	lang := "lang_example" // string | Play content language (hl), e.g. 'en' or 'pt-BR' (optional) (default to "en")
	prefer := "respond-async, wait=25" // string | `respond-async[, wait=N]` (RFC 7240): run the call async. If it has not finished after `wait` seconds (0-120, default 25) the answer is `202` with a `request_id`; poll `GET /v1/requests/{request_id}`. Its `wait=` wins over `async_wait`; without one, `async_wait` sets the wait. (optional)
	xCallbackURL := "xCallbackURL_example" // string | An `https` URL that receives the signed `request.completed` webhook when the call finishes. Implies async: on its own (no `Prefer`, `async` or `async_wait`) the answer is an immediate `202`; with `Prefer: respond-async` or `async=true` the call still waits 25 s unless a wait is given. Wins over `callback_url`. (optional)
	idempotencyKey := "idempotencyKey_example" // string | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call's current state (`Idempotent-Replayed: true`) without running or billing it again; on a different call it is `409 idempotency_key_reused`. Applies to async calls only; on a synchronous call it is ignored. Wins over `idempotency_key`. (optional)
	async := true // bool | Query form of `Prefer: respond-async`: `true` or `1` (also `yes`, `on`; `false`, `0`, `no`, `off` leave the call synchronous). Waits 25 s unless `async_wait` is given. Not sent to the scraper. (optional)
	asyncWait := int32(56) // int32 | Seconds (0-120; values outside are clamped) to wait for the result before answering `202`. Implies async. Not sent to the scraper. (optional)
	callbackUrl := "callbackUrl_example" // string | Query form of `X-Callback-URL` (URL-encode it). Implies async; on its own the answer is an immediate `202` (wait 0). Not sent to the scraper. (optional)
	idempotencyKey2 := "idempotencyKey_example" // string | Query form of `Idempotency-Key`. Not sent to the scraper. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayGetAppDetail(context.Background(), appId).Country(country).Lang(lang).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayGetAppDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayGetAppDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayGetAppDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**appId** | **string** | Android package id, e.g. &#39;com.whatsapp&#39;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayGetAppDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. &#39;US&#39; | [default to &quot;US&quot;]
 **lang** | **string** | Play content language (hl), e.g. &#39;en&#39; or &#39;pt-BR&#39; | [default to &quot;en&quot;]
 **prefer** | **string** | &#x60;respond-async[, wait&#x3D;N]&#x60; (RFC 7240): run the call async. If it has not finished after &#x60;wait&#x60; seconds (0-120, default 25) the answer is &#x60;202&#x60; with a &#x60;request_id&#x60;; poll &#x60;GET /v1/requests/{request_id}&#x60;. Its &#x60;wait&#x3D;&#x60; wins over &#x60;async_wait&#x60;; without one, &#x60;async_wait&#x60; sets the wait. | 
 **xCallbackURL** | **string** | An &#x60;https&#x60; URL that receives the signed &#x60;request.completed&#x60; webhook when the call finishes. Implies async: on its own (no &#x60;Prefer&#x60;, &#x60;async&#x60; or &#x60;async_wait&#x60;) the answer is an immediate &#x60;202&#x60;; with &#x60;Prefer: respond-async&#x60; or &#x60;async&#x3D;true&#x60; the call still waits 25 s unless a wait is given. Wins over &#x60;callback_url&#x60;. | 
 **idempotencyKey** | **string** | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call&#39;s current state (&#x60;Idempotent-Replayed: true&#x60;) without running or billing it again; on a different call it is &#x60;409 idempotency_key_reused&#x60;. Applies to async calls only; on a synchronous call it is ignored. Wins over &#x60;idempotency_key&#x60;. | 
 **async** | **bool** | Query form of &#x60;Prefer: respond-async&#x60;: &#x60;true&#x60; or &#x60;1&#x60; (also &#x60;yes&#x60;, &#x60;on&#x60;; &#x60;false&#x60;, &#x60;0&#x60;, &#x60;no&#x60;, &#x60;off&#x60; leave the call synchronous). Waits 25 s unless &#x60;async_wait&#x60; is given. Not sent to the scraper. | 
 **asyncWait** | **int32** | Seconds (0-120; values outside are clamped) to wait for the result before answering &#x60;202&#x60;. Implies async. Not sent to the scraper. | 
 **callbackUrl** | **string** | Query form of &#x60;X-Callback-URL&#x60; (URL-encode it). Implies async; on its own the answer is an immediate &#x60;202&#x60; (wait 0). Not sent to the scraper. | 
 **idempotencyKey2** | **string** | Query form of &#x60;Idempotency-Key&#x60;. Not sent to the scraper. | 

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


## GooglePlayGetAppPermissions

> interface{} GooglePlayGetAppPermissions(ctx, appId).Lang(lang).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()

Get app permissions



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
	appId := "appId_example" // string | Android package id, e.g. 'com.whatsapp'.
	lang := "lang_example" // string | Play content language (hl), e.g. 'en' or 'pt-BR' (optional) (default to "en")
	prefer := "respond-async, wait=25" // string | `respond-async[, wait=N]` (RFC 7240): run the call async. If it has not finished after `wait` seconds (0-120, default 25) the answer is `202` with a `request_id`; poll `GET /v1/requests/{request_id}`. Its `wait=` wins over `async_wait`; without one, `async_wait` sets the wait. (optional)
	xCallbackURL := "xCallbackURL_example" // string | An `https` URL that receives the signed `request.completed` webhook when the call finishes. Implies async: on its own (no `Prefer`, `async` or `async_wait`) the answer is an immediate `202`; with `Prefer: respond-async` or `async=true` the call still waits 25 s unless a wait is given. Wins over `callback_url`. (optional)
	idempotencyKey := "idempotencyKey_example" // string | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call's current state (`Idempotent-Replayed: true`) without running or billing it again; on a different call it is `409 idempotency_key_reused`. Applies to async calls only; on a synchronous call it is ignored. Wins over `idempotency_key`. (optional)
	async := true // bool | Query form of `Prefer: respond-async`: `true` or `1` (also `yes`, `on`; `false`, `0`, `no`, `off` leave the call synchronous). Waits 25 s unless `async_wait` is given. Not sent to the scraper. (optional)
	asyncWait := int32(56) // int32 | Seconds (0-120; values outside are clamped) to wait for the result before answering `202`. Implies async. Not sent to the scraper. (optional)
	callbackUrl := "callbackUrl_example" // string | Query form of `X-Callback-URL` (URL-encode it). Implies async; on its own the answer is an immediate `202` (wait 0). Not sent to the scraper. (optional)
	idempotencyKey2 := "idempotencyKey_example" // string | Query form of `Idempotency-Key`. Not sent to the scraper. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayGetAppPermissions(context.Background(), appId).Lang(lang).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayGetAppPermissions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayGetAppPermissions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayGetAppPermissions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**appId** | **string** | Android package id, e.g. &#39;com.whatsapp&#39;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayGetAppPermissionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **lang** | **string** | Play content language (hl), e.g. &#39;en&#39; or &#39;pt-BR&#39; | [default to &quot;en&quot;]
 **prefer** | **string** | &#x60;respond-async[, wait&#x3D;N]&#x60; (RFC 7240): run the call async. If it has not finished after &#x60;wait&#x60; seconds (0-120, default 25) the answer is &#x60;202&#x60; with a &#x60;request_id&#x60;; poll &#x60;GET /v1/requests/{request_id}&#x60;. Its &#x60;wait&#x3D;&#x60; wins over &#x60;async_wait&#x60;; without one, &#x60;async_wait&#x60; sets the wait. | 
 **xCallbackURL** | **string** | An &#x60;https&#x60; URL that receives the signed &#x60;request.completed&#x60; webhook when the call finishes. Implies async: on its own (no &#x60;Prefer&#x60;, &#x60;async&#x60; or &#x60;async_wait&#x60;) the answer is an immediate &#x60;202&#x60;; with &#x60;Prefer: respond-async&#x60; or &#x60;async&#x3D;true&#x60; the call still waits 25 s unless a wait is given. Wins over &#x60;callback_url&#x60;. | 
 **idempotencyKey** | **string** | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call&#39;s current state (&#x60;Idempotent-Replayed: true&#x60;) without running or billing it again; on a different call it is &#x60;409 idempotency_key_reused&#x60;. Applies to async calls only; on a synchronous call it is ignored. Wins over &#x60;idempotency_key&#x60;. | 
 **async** | **bool** | Query form of &#x60;Prefer: respond-async&#x60;: &#x60;true&#x60; or &#x60;1&#x60; (also &#x60;yes&#x60;, &#x60;on&#x60;; &#x60;false&#x60;, &#x60;0&#x60;, &#x60;no&#x60;, &#x60;off&#x60; leave the call synchronous). Waits 25 s unless &#x60;async_wait&#x60; is given. Not sent to the scraper. | 
 **asyncWait** | **int32** | Seconds (0-120; values outside are clamped) to wait for the result before answering &#x60;202&#x60;. Implies async. Not sent to the scraper. | 
 **callbackUrl** | **string** | Query form of &#x60;X-Callback-URL&#x60; (URL-encode it). Implies async; on its own the answer is an immediate &#x60;202&#x60; (wait 0). Not sent to the scraper. | 
 **idempotencyKey2** | **string** | Query form of &#x60;Idempotency-Key&#x60;. Not sent to the scraper. | 

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


## GooglePlayGetAppReviews

> interface{} GooglePlayGetAppReviews(ctx, appId).Country(country).Lang(lang).Sort(sort).Count(count).PageToken(pageToken).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()

Get app reviews



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
	appId := "appId_example" // string | Android package id, e.g. 'com.whatsapp'.
	country := "country_example" // string | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. 'US' (optional) (default to "US")
	lang := "lang_example" // string | Play content language (hl), e.g. 'en' or 'pt-BR' (optional) (default to "en")
	sort := "sort_example" // string | newest | rating | helpfulness (optional) (default to "newest")
	count := int32(56) // int32 |  (optional) (default to 40)
	pageToken := "pageToken_example" // string | Pagination token (optional)
	prefer := "respond-async, wait=25" // string | `respond-async[, wait=N]` (RFC 7240): run the call async. If it has not finished after `wait` seconds (0-120, default 25) the answer is `202` with a `request_id`; poll `GET /v1/requests/{request_id}`. Its `wait=` wins over `async_wait`; without one, `async_wait` sets the wait. (optional)
	xCallbackURL := "xCallbackURL_example" // string | An `https` URL that receives the signed `request.completed` webhook when the call finishes. Implies async: on its own (no `Prefer`, `async` or `async_wait`) the answer is an immediate `202`; with `Prefer: respond-async` or `async=true` the call still waits 25 s unless a wait is given. Wins over `callback_url`. (optional)
	idempotencyKey := "idempotencyKey_example" // string | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call's current state (`Idempotent-Replayed: true`) without running or billing it again; on a different call it is `409 idempotency_key_reused`. Applies to async calls only; on a synchronous call it is ignored. Wins over `idempotency_key`. (optional)
	async := true // bool | Query form of `Prefer: respond-async`: `true` or `1` (also `yes`, `on`; `false`, `0`, `no`, `off` leave the call synchronous). Waits 25 s unless `async_wait` is given. Not sent to the scraper. (optional)
	asyncWait := int32(56) // int32 | Seconds (0-120; values outside are clamped) to wait for the result before answering `202`. Implies async. Not sent to the scraper. (optional)
	callbackUrl := "callbackUrl_example" // string | Query form of `X-Callback-URL` (URL-encode it). Implies async; on its own the answer is an immediate `202` (wait 0). Not sent to the scraper. (optional)
	idempotencyKey2 := "idempotencyKey_example" // string | Query form of `Idempotency-Key`. Not sent to the scraper. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayGetAppReviews(context.Background(), appId).Country(country).Lang(lang).Sort(sort).Count(count).PageToken(pageToken).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayGetAppReviews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayGetAppReviews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayGetAppReviews`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**appId** | **string** | Android package id, e.g. &#39;com.whatsapp&#39;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayGetAppReviewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. &#39;US&#39; | [default to &quot;US&quot;]
 **lang** | **string** | Play content language (hl), e.g. &#39;en&#39; or &#39;pt-BR&#39; | [default to &quot;en&quot;]
 **sort** | **string** | newest | rating | helpfulness | [default to &quot;newest&quot;]
 **count** | **int32** |  | [default to 40]
 **pageToken** | **string** | Pagination token | 
 **prefer** | **string** | &#x60;respond-async[, wait&#x3D;N]&#x60; (RFC 7240): run the call async. If it has not finished after &#x60;wait&#x60; seconds (0-120, default 25) the answer is &#x60;202&#x60; with a &#x60;request_id&#x60;; poll &#x60;GET /v1/requests/{request_id}&#x60;. Its &#x60;wait&#x3D;&#x60; wins over &#x60;async_wait&#x60;; without one, &#x60;async_wait&#x60; sets the wait. | 
 **xCallbackURL** | **string** | An &#x60;https&#x60; URL that receives the signed &#x60;request.completed&#x60; webhook when the call finishes. Implies async: on its own (no &#x60;Prefer&#x60;, &#x60;async&#x60; or &#x60;async_wait&#x60;) the answer is an immediate &#x60;202&#x60;; with &#x60;Prefer: respond-async&#x60; or &#x60;async&#x3D;true&#x60; the call still waits 25 s unless a wait is given. Wins over &#x60;callback_url&#x60;. | 
 **idempotencyKey** | **string** | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call&#39;s current state (&#x60;Idempotent-Replayed: true&#x60;) without running or billing it again; on a different call it is &#x60;409 idempotency_key_reused&#x60;. Applies to async calls only; on a synchronous call it is ignored. Wins over &#x60;idempotency_key&#x60;. | 
 **async** | **bool** | Query form of &#x60;Prefer: respond-async&#x60;: &#x60;true&#x60; or &#x60;1&#x60; (also &#x60;yes&#x60;, &#x60;on&#x60;; &#x60;false&#x60;, &#x60;0&#x60;, &#x60;no&#x60;, &#x60;off&#x60; leave the call synchronous). Waits 25 s unless &#x60;async_wait&#x60; is given. Not sent to the scraper. | 
 **asyncWait** | **int32** | Seconds (0-120; values outside are clamped) to wait for the result before answering &#x60;202&#x60;. Implies async. Not sent to the scraper. | 
 **callbackUrl** | **string** | Query form of &#x60;X-Callback-URL&#x60; (URL-encode it). Implies async; on its own the answer is an immediate &#x60;202&#x60; (wait 0). Not sent to the scraper. | 
 **idempotencyKey2** | **string** | Query form of &#x60;Idempotency-Key&#x60;. Not sent to the scraper. | 

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


## GooglePlayGetDeveloperApps

> interface{} GooglePlayGetDeveloperApps(ctx, developer).Country(country).Lang(lang).Num(num).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()

Get developer apps



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
	developer := "developer_example" // string | Developer name or numeric id
	country := "country_example" // string | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. 'US' (optional) (default to "US")
	lang := "lang_example" // string | Play content language (hl), e.g. 'en' or 'pt-BR' (optional) (default to "en")
	num := int32(56) // int32 | Max apps; follows rail continuations above the page's directly-rendered slice (optional) (default to 100)
	prefer := "respond-async, wait=25" // string | `respond-async[, wait=N]` (RFC 7240): run the call async. If it has not finished after `wait` seconds (0-120, default 25) the answer is `202` with a `request_id`; poll `GET /v1/requests/{request_id}`. Its `wait=` wins over `async_wait`; without one, `async_wait` sets the wait. (optional)
	xCallbackURL := "xCallbackURL_example" // string | An `https` URL that receives the signed `request.completed` webhook when the call finishes. Implies async: on its own (no `Prefer`, `async` or `async_wait`) the answer is an immediate `202`; with `Prefer: respond-async` or `async=true` the call still waits 25 s unless a wait is given. Wins over `callback_url`. (optional)
	idempotencyKey := "idempotencyKey_example" // string | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call's current state (`Idempotent-Replayed: true`) without running or billing it again; on a different call it is `409 idempotency_key_reused`. Applies to async calls only; on a synchronous call it is ignored. Wins over `idempotency_key`. (optional)
	async := true // bool | Query form of `Prefer: respond-async`: `true` or `1` (also `yes`, `on`; `false`, `0`, `no`, `off` leave the call synchronous). Waits 25 s unless `async_wait` is given. Not sent to the scraper. (optional)
	asyncWait := int32(56) // int32 | Seconds (0-120; values outside are clamped) to wait for the result before answering `202`. Implies async. Not sent to the scraper. (optional)
	callbackUrl := "callbackUrl_example" // string | Query form of `X-Callback-URL` (URL-encode it). Implies async; on its own the answer is an immediate `202` (wait 0). Not sent to the scraper. (optional)
	idempotencyKey2 := "idempotencyKey_example" // string | Query form of `Idempotency-Key`. Not sent to the scraper. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayGetDeveloperApps(context.Background(), developer).Country(country).Lang(lang).Num(num).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayGetDeveloperApps``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayGetDeveloperApps`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayGetDeveloperApps`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**developer** | **string** | Developer name or numeric id | 

### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayGetDeveloperAppsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. &#39;US&#39; | [default to &quot;US&quot;]
 **lang** | **string** | Play content language (hl), e.g. &#39;en&#39; or &#39;pt-BR&#39; | [default to &quot;en&quot;]
 **num** | **int32** | Max apps; follows rail continuations above the page&#39;s directly-rendered slice | [default to 100]
 **prefer** | **string** | &#x60;respond-async[, wait&#x3D;N]&#x60; (RFC 7240): run the call async. If it has not finished after &#x60;wait&#x60; seconds (0-120, default 25) the answer is &#x60;202&#x60; with a &#x60;request_id&#x60;; poll &#x60;GET /v1/requests/{request_id}&#x60;. Its &#x60;wait&#x3D;&#x60; wins over &#x60;async_wait&#x60;; without one, &#x60;async_wait&#x60; sets the wait. | 
 **xCallbackURL** | **string** | An &#x60;https&#x60; URL that receives the signed &#x60;request.completed&#x60; webhook when the call finishes. Implies async: on its own (no &#x60;Prefer&#x60;, &#x60;async&#x60; or &#x60;async_wait&#x60;) the answer is an immediate &#x60;202&#x60;; with &#x60;Prefer: respond-async&#x60; or &#x60;async&#x3D;true&#x60; the call still waits 25 s unless a wait is given. Wins over &#x60;callback_url&#x60;. | 
 **idempotencyKey** | **string** | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call&#39;s current state (&#x60;Idempotent-Replayed: true&#x60;) without running or billing it again; on a different call it is &#x60;409 idempotency_key_reused&#x60;. Applies to async calls only; on a synchronous call it is ignored. Wins over &#x60;idempotency_key&#x60;. | 
 **async** | **bool** | Query form of &#x60;Prefer: respond-async&#x60;: &#x60;true&#x60; or &#x60;1&#x60; (also &#x60;yes&#x60;, &#x60;on&#x60;; &#x60;false&#x60;, &#x60;0&#x60;, &#x60;no&#x60;, &#x60;off&#x60; leave the call synchronous). Waits 25 s unless &#x60;async_wait&#x60; is given. Not sent to the scraper. | 
 **asyncWait** | **int32** | Seconds (0-120; values outside are clamped) to wait for the result before answering &#x60;202&#x60;. Implies async. Not sent to the scraper. | 
 **callbackUrl** | **string** | Query form of &#x60;X-Callback-URL&#x60; (URL-encode it). Implies async; on its own the answer is an immediate &#x60;202&#x60; (wait 0). Not sent to the scraper. | 
 **idempotencyKey2** | **string** | Query form of &#x60;Idempotency-Key&#x60;. Not sent to the scraper. | 

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


## GooglePlayGetSimilarApps

> interface{} GooglePlayGetSimilarApps(ctx, appId).Country(country).Lang(lang).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()

Get similar apps



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
	appId := "appId_example" // string | Android package id, e.g. 'com.whatsapp'.
	country := "country_example" // string | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. 'US' (optional) (default to "US")
	lang := "lang_example" // string | Play content language (hl), e.g. 'en' or 'pt-BR' (optional) (default to "en")
	prefer := "respond-async, wait=25" // string | `respond-async[, wait=N]` (RFC 7240): run the call async. If it has not finished after `wait` seconds (0-120, default 25) the answer is `202` with a `request_id`; poll `GET /v1/requests/{request_id}`. Its `wait=` wins over `async_wait`; without one, `async_wait` sets the wait. (optional)
	xCallbackURL := "xCallbackURL_example" // string | An `https` URL that receives the signed `request.completed` webhook when the call finishes. Implies async: on its own (no `Prefer`, `async` or `async_wait`) the answer is an immediate `202`; with `Prefer: respond-async` or `async=true` the call still waits 25 s unless a wait is given. Wins over `callback_url`. (optional)
	idempotencyKey := "idempotencyKey_example" // string | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call's current state (`Idempotent-Replayed: true`) without running or billing it again; on a different call it is `409 idempotency_key_reused`. Applies to async calls only; on a synchronous call it is ignored. Wins over `idempotency_key`. (optional)
	async := true // bool | Query form of `Prefer: respond-async`: `true` or `1` (also `yes`, `on`; `false`, `0`, `no`, `off` leave the call synchronous). Waits 25 s unless `async_wait` is given. Not sent to the scraper. (optional)
	asyncWait := int32(56) // int32 | Seconds (0-120; values outside are clamped) to wait for the result before answering `202`. Implies async. Not sent to the scraper. (optional)
	callbackUrl := "callbackUrl_example" // string | Query form of `X-Callback-URL` (URL-encode it). Implies async; on its own the answer is an immediate `202` (wait 0). Not sent to the scraper. (optional)
	idempotencyKey2 := "idempotencyKey_example" // string | Query form of `Idempotency-Key`. Not sent to the scraper. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayGetSimilarApps(context.Background(), appId).Country(country).Lang(lang).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayGetSimilarApps``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayGetSimilarApps`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayGetSimilarApps`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**appId** | **string** | Android package id, e.g. &#39;com.whatsapp&#39;. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayGetSimilarAppsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. &#39;US&#39; | [default to &quot;US&quot;]
 **lang** | **string** | Play content language (hl), e.g. &#39;en&#39; or &#39;pt-BR&#39; | [default to &quot;en&quot;]
 **prefer** | **string** | &#x60;respond-async[, wait&#x3D;N]&#x60; (RFC 7240): run the call async. If it has not finished after &#x60;wait&#x60; seconds (0-120, default 25) the answer is &#x60;202&#x60; with a &#x60;request_id&#x60;; poll &#x60;GET /v1/requests/{request_id}&#x60;. Its &#x60;wait&#x3D;&#x60; wins over &#x60;async_wait&#x60;; without one, &#x60;async_wait&#x60; sets the wait. | 
 **xCallbackURL** | **string** | An &#x60;https&#x60; URL that receives the signed &#x60;request.completed&#x60; webhook when the call finishes. Implies async: on its own (no &#x60;Prefer&#x60;, &#x60;async&#x60; or &#x60;async_wait&#x60;) the answer is an immediate &#x60;202&#x60;; with &#x60;Prefer: respond-async&#x60; or &#x60;async&#x3D;true&#x60; the call still waits 25 s unless a wait is given. Wins over &#x60;callback_url&#x60;. | 
 **idempotencyKey** | **string** | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call&#39;s current state (&#x60;Idempotent-Replayed: true&#x60;) without running or billing it again; on a different call it is &#x60;409 idempotency_key_reused&#x60;. Applies to async calls only; on a synchronous call it is ignored. Wins over &#x60;idempotency_key&#x60;. | 
 **async** | **bool** | Query form of &#x60;Prefer: respond-async&#x60;: &#x60;true&#x60; or &#x60;1&#x60; (also &#x60;yes&#x60;, &#x60;on&#x60;; &#x60;false&#x60;, &#x60;0&#x60;, &#x60;no&#x60;, &#x60;off&#x60; leave the call synchronous). Waits 25 s unless &#x60;async_wait&#x60; is given. Not sent to the scraper. | 
 **asyncWait** | **int32** | Seconds (0-120; values outside are clamped) to wait for the result before answering &#x60;202&#x60;. Implies async. Not sent to the scraper. | 
 **callbackUrl** | **string** | Query form of &#x60;X-Callback-URL&#x60; (URL-encode it). Implies async; on its own the answer is an immediate &#x60;202&#x60; (wait 0). Not sent to the scraper. | 
 **idempotencyKey2** | **string** | Query form of &#x60;Idempotency-Key&#x60;. Not sent to the scraper. | 

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


## GooglePlayListCategories

> interface{} GooglePlayListCategories(ctx).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()

List categories



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
	prefer := "respond-async, wait=25" // string | `respond-async[, wait=N]` (RFC 7240): run the call async. If it has not finished after `wait` seconds (0-120, default 25) the answer is `202` with a `request_id`; poll `GET /v1/requests/{request_id}`. Its `wait=` wins over `async_wait`; without one, `async_wait` sets the wait. (optional)
	xCallbackURL := "xCallbackURL_example" // string | An `https` URL that receives the signed `request.completed` webhook when the call finishes. Implies async: on its own (no `Prefer`, `async` or `async_wait`) the answer is an immediate `202`; with `Prefer: respond-async` or `async=true` the call still waits 25 s unless a wait is given. Wins over `callback_url`. (optional)
	idempotencyKey := "idempotencyKey_example" // string | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call's current state (`Idempotent-Replayed: true`) without running or billing it again; on a different call it is `409 idempotency_key_reused`. Applies to async calls only; on a synchronous call it is ignored. Wins over `idempotency_key`. (optional)
	async := true // bool | Query form of `Prefer: respond-async`: `true` or `1` (also `yes`, `on`; `false`, `0`, `no`, `off` leave the call synchronous). Waits 25 s unless `async_wait` is given. Not sent to the scraper. (optional)
	asyncWait := int32(56) // int32 | Seconds (0-120; values outside are clamped) to wait for the result before answering `202`. Implies async. Not sent to the scraper. (optional)
	callbackUrl := "callbackUrl_example" // string | Query form of `X-Callback-URL` (URL-encode it). Implies async; on its own the answer is an immediate `202` (wait 0). Not sent to the scraper. (optional)
	idempotencyKey2 := "idempotencyKey_example" // string | Query form of `Idempotency-Key`. Not sent to the scraper. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayListCategories(context.Background()).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayListCategories``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayListCategories`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayListCategories`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayListCategoriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **prefer** | **string** | &#x60;respond-async[, wait&#x3D;N]&#x60; (RFC 7240): run the call async. If it has not finished after &#x60;wait&#x60; seconds (0-120, default 25) the answer is &#x60;202&#x60; with a &#x60;request_id&#x60;; poll &#x60;GET /v1/requests/{request_id}&#x60;. Its &#x60;wait&#x3D;&#x60; wins over &#x60;async_wait&#x60;; without one, &#x60;async_wait&#x60; sets the wait. | 
 **xCallbackURL** | **string** | An &#x60;https&#x60; URL that receives the signed &#x60;request.completed&#x60; webhook when the call finishes. Implies async: on its own (no &#x60;Prefer&#x60;, &#x60;async&#x60; or &#x60;async_wait&#x60;) the answer is an immediate &#x60;202&#x60;; with &#x60;Prefer: respond-async&#x60; or &#x60;async&#x3D;true&#x60; the call still waits 25 s unless a wait is given. Wins over &#x60;callback_url&#x60;. | 
 **idempotencyKey** | **string** | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call&#39;s current state (&#x60;Idempotent-Replayed: true&#x60;) without running or billing it again; on a different call it is &#x60;409 idempotency_key_reused&#x60;. Applies to async calls only; on a synchronous call it is ignored. Wins over &#x60;idempotency_key&#x60;. | 
 **async** | **bool** | Query form of &#x60;Prefer: respond-async&#x60;: &#x60;true&#x60; or &#x60;1&#x60; (also &#x60;yes&#x60;, &#x60;on&#x60;; &#x60;false&#x60;, &#x60;0&#x60;, &#x60;no&#x60;, &#x60;off&#x60; leave the call synchronous). Waits 25 s unless &#x60;async_wait&#x60; is given. Not sent to the scraper. | 
 **asyncWait** | **int32** | Seconds (0-120; values outside are clamped) to wait for the result before answering &#x60;202&#x60;. Implies async. Not sent to the scraper. | 
 **callbackUrl** | **string** | Query form of &#x60;X-Callback-URL&#x60; (URL-encode it). Implies async; on its own the answer is an immediate &#x60;202&#x60; (wait 0). Not sent to the scraper. | 
 **idempotencyKey2** | **string** | Query form of &#x60;Idempotency-Key&#x60;. Not sent to the scraper. | 

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


## GooglePlayListMarkets

> interface{} GooglePlayListMarkets(ctx).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()

List markets



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
	prefer := "respond-async, wait=25" // string | `respond-async[, wait=N]` (RFC 7240): run the call async. If it has not finished after `wait` seconds (0-120, default 25) the answer is `202` with a `request_id`; poll `GET /v1/requests/{request_id}`. Its `wait=` wins over `async_wait`; without one, `async_wait` sets the wait. (optional)
	xCallbackURL := "xCallbackURL_example" // string | An `https` URL that receives the signed `request.completed` webhook when the call finishes. Implies async: on its own (no `Prefer`, `async` or `async_wait`) the answer is an immediate `202`; with `Prefer: respond-async` or `async=true` the call still waits 25 s unless a wait is given. Wins over `callback_url`. (optional)
	idempotencyKey := "idempotencyKey_example" // string | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call's current state (`Idempotent-Replayed: true`) without running or billing it again; on a different call it is `409 idempotency_key_reused`. Applies to async calls only; on a synchronous call it is ignored. Wins over `idempotency_key`. (optional)
	async := true // bool | Query form of `Prefer: respond-async`: `true` or `1` (also `yes`, `on`; `false`, `0`, `no`, `off` leave the call synchronous). Waits 25 s unless `async_wait` is given. Not sent to the scraper. (optional)
	asyncWait := int32(56) // int32 | Seconds (0-120; values outside are clamped) to wait for the result before answering `202`. Implies async. Not sent to the scraper. (optional)
	callbackUrl := "callbackUrl_example" // string | Query form of `X-Callback-URL` (URL-encode it). Implies async; on its own the answer is an immediate `202` (wait 0). Not sent to the scraper. (optional)
	idempotencyKey2 := "idempotencyKey_example" // string | Query form of `Idempotency-Key`. Not sent to the scraper. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayListMarkets(context.Background()).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayListMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayListMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayListMarkets`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayListMarketsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **prefer** | **string** | &#x60;respond-async[, wait&#x3D;N]&#x60; (RFC 7240): run the call async. If it has not finished after &#x60;wait&#x60; seconds (0-120, default 25) the answer is &#x60;202&#x60; with a &#x60;request_id&#x60;; poll &#x60;GET /v1/requests/{request_id}&#x60;. Its &#x60;wait&#x3D;&#x60; wins over &#x60;async_wait&#x60;; without one, &#x60;async_wait&#x60; sets the wait. | 
 **xCallbackURL** | **string** | An &#x60;https&#x60; URL that receives the signed &#x60;request.completed&#x60; webhook when the call finishes. Implies async: on its own (no &#x60;Prefer&#x60;, &#x60;async&#x60; or &#x60;async_wait&#x60;) the answer is an immediate &#x60;202&#x60;; with &#x60;Prefer: respond-async&#x60; or &#x60;async&#x3D;true&#x60; the call still waits 25 s unless a wait is given. Wins over &#x60;callback_url&#x60;. | 
 **idempotencyKey** | **string** | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call&#39;s current state (&#x60;Idempotent-Replayed: true&#x60;) without running or billing it again; on a different call it is &#x60;409 idempotency_key_reused&#x60;. Applies to async calls only; on a synchronous call it is ignored. Wins over &#x60;idempotency_key&#x60;. | 
 **async** | **bool** | Query form of &#x60;Prefer: respond-async&#x60;: &#x60;true&#x60; or &#x60;1&#x60; (also &#x60;yes&#x60;, &#x60;on&#x60;; &#x60;false&#x60;, &#x60;0&#x60;, &#x60;no&#x60;, &#x60;off&#x60; leave the call synchronous). Waits 25 s unless &#x60;async_wait&#x60; is given. Not sent to the scraper. | 
 **asyncWait** | **int32** | Seconds (0-120; values outside are clamped) to wait for the result before answering &#x60;202&#x60;. Implies async. Not sent to the scraper. | 
 **callbackUrl** | **string** | Query form of &#x60;X-Callback-URL&#x60; (URL-encode it). Implies async; on its own the answer is an immediate &#x60;202&#x60; (wait 0). Not sent to the scraper. | 
 **idempotencyKey2** | **string** | Query form of &#x60;Idempotency-Key&#x60;. Not sent to the scraper. | 

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


## GooglePlaySearchApps

> interface{} GooglePlaySearchApps(ctx).Query(query).Country(country).Lang(lang).Price(price).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()

Search apps



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
	query := "query_example" // string | Search keywords, e.g. 'puzzle'
	country := "country_example" // string | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. 'US' (optional) (default to "US")
	lang := "lang_example" // string | Play content language (hl), e.g. 'en' or 'pt-BR' (optional) (default to "en")
	price := "price_example" // string | free | paid | all (optional)
	prefer := "respond-async, wait=25" // string | `respond-async[, wait=N]` (RFC 7240): run the call async. If it has not finished after `wait` seconds (0-120, default 25) the answer is `202` with a `request_id`; poll `GET /v1/requests/{request_id}`. Its `wait=` wins over `async_wait`; without one, `async_wait` sets the wait. (optional)
	xCallbackURL := "xCallbackURL_example" // string | An `https` URL that receives the signed `request.completed` webhook when the call finishes. Implies async: on its own (no `Prefer`, `async` or `async_wait`) the answer is an immediate `202`; with `Prefer: respond-async` or `async=true` the call still waits 25 s unless a wait is given. Wins over `callback_url`. (optional)
	idempotencyKey := "idempotencyKey_example" // string | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call's current state (`Idempotent-Replayed: true`) without running or billing it again; on a different call it is `409 idempotency_key_reused`. Applies to async calls only; on a synchronous call it is ignored. Wins over `idempotency_key`. (optional)
	async := true // bool | Query form of `Prefer: respond-async`: `true` or `1` (also `yes`, `on`; `false`, `0`, `no`, `off` leave the call synchronous). Waits 25 s unless `async_wait` is given. Not sent to the scraper. (optional)
	asyncWait := int32(56) // int32 | Seconds (0-120; values outside are clamped) to wait for the result before answering `202`. Implies async. Not sent to the scraper. (optional)
	callbackUrl := "callbackUrl_example" // string | Query form of `X-Callback-URL` (URL-encode it). Implies async; on its own the answer is an immediate `202` (wait 0). Not sent to the scraper. (optional)
	idempotencyKey2 := "idempotencyKey_example" // string | Query form of `Idempotency-Key`. Not sent to the scraper. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlaySearchApps(context.Background()).Query(query).Country(country).Lang(lang).Price(price).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlaySearchApps``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlaySearchApps`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlaySearchApps`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlaySearchAppsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords, e.g. &#39;puzzle&#39; | 
 **country** | **string** | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. &#39;US&#39; | [default to &quot;US&quot;]
 **lang** | **string** | Play content language (hl), e.g. &#39;en&#39; or &#39;pt-BR&#39; | [default to &quot;en&quot;]
 **price** | **string** | free | paid | all | 
 **prefer** | **string** | &#x60;respond-async[, wait&#x3D;N]&#x60; (RFC 7240): run the call async. If it has not finished after &#x60;wait&#x60; seconds (0-120, default 25) the answer is &#x60;202&#x60; with a &#x60;request_id&#x60;; poll &#x60;GET /v1/requests/{request_id}&#x60;. Its &#x60;wait&#x3D;&#x60; wins over &#x60;async_wait&#x60;; without one, &#x60;async_wait&#x60; sets the wait. | 
 **xCallbackURL** | **string** | An &#x60;https&#x60; URL that receives the signed &#x60;request.completed&#x60; webhook when the call finishes. Implies async: on its own (no &#x60;Prefer&#x60;, &#x60;async&#x60; or &#x60;async_wait&#x60;) the answer is an immediate &#x60;202&#x60;; with &#x60;Prefer: respond-async&#x60; or &#x60;async&#x3D;true&#x60; the call still waits 25 s unless a wait is given. Wins over &#x60;callback_url&#x60;. | 
 **idempotencyKey** | **string** | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call&#39;s current state (&#x60;Idempotent-Replayed: true&#x60;) without running or billing it again; on a different call it is &#x60;409 idempotency_key_reused&#x60;. Applies to async calls only; on a synchronous call it is ignored. Wins over &#x60;idempotency_key&#x60;. | 
 **async** | **bool** | Query form of &#x60;Prefer: respond-async&#x60;: &#x60;true&#x60; or &#x60;1&#x60; (also &#x60;yes&#x60;, &#x60;on&#x60;; &#x60;false&#x60;, &#x60;0&#x60;, &#x60;no&#x60;, &#x60;off&#x60; leave the call synchronous). Waits 25 s unless &#x60;async_wait&#x60; is given. Not sent to the scraper. | 
 **asyncWait** | **int32** | Seconds (0-120; values outside are clamped) to wait for the result before answering &#x60;202&#x60;. Implies async. Not sent to the scraper. | 
 **callbackUrl** | **string** | Query form of &#x60;X-Callback-URL&#x60; (URL-encode it). Implies async; on its own the answer is an immediate &#x60;202&#x60; (wait 0). Not sent to the scraper. | 
 **idempotencyKey2** | **string** | Query form of &#x60;Idempotency-Key&#x60;. Not sent to the scraper. | 

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


## GooglePlayTopCharts

> interface{} GooglePlayTopCharts(ctx, collection).Category(category).Country(country).Lang(lang).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()

Top charts



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
	collection := "collection_example" // string | topselling_free | topselling_paid | topgrossing
	category := "category_example" // string | Play category, e.g. 'GAME' (optional) (default to "APPLICATION")
	country := "country_example" // string | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. 'US' (optional) (default to "US")
	lang := "lang_example" // string | Play content language (hl), e.g. 'en' or 'pt-BR' (optional) (default to "en")
	prefer := "respond-async, wait=25" // string | `respond-async[, wait=N]` (RFC 7240): run the call async. If it has not finished after `wait` seconds (0-120, default 25) the answer is `202` with a `request_id`; poll `GET /v1/requests/{request_id}`. Its `wait=` wins over `async_wait`; without one, `async_wait` sets the wait. (optional)
	xCallbackURL := "xCallbackURL_example" // string | An `https` URL that receives the signed `request.completed` webhook when the call finishes. Implies async: on its own (no `Prefer`, `async` or `async_wait`) the answer is an immediate `202`; with `Prefer: respond-async` or `async=true` the call still waits 25 s unless a wait is given. Wins over `callback_url`. (optional)
	idempotencyKey := "idempotencyKey_example" // string | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call's current state (`Idempotent-Replayed: true`) without running or billing it again; on a different call it is `409 idempotency_key_reused`. Applies to async calls only; on a synchronous call it is ignored. Wins over `idempotency_key`. (optional)
	async := true // bool | Query form of `Prefer: respond-async`: `true` or `1` (also `yes`, `on`; `false`, `0`, `no`, `off` leave the call synchronous). Waits 25 s unless `async_wait` is given. Not sent to the scraper. (optional)
	asyncWait := int32(56) // int32 | Seconds (0-120; values outside are clamped) to wait for the result before answering `202`. Implies async. Not sent to the scraper. (optional)
	callbackUrl := "callbackUrl_example" // string | Query form of `X-Callback-URL` (URL-encode it). Implies async; on its own the answer is an immediate `202` (wait 0). Not sent to the scraper. (optional)
	idempotencyKey2 := "idempotencyKey_example" // string | Query form of `Idempotency-Key`. Not sent to the scraper. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GooglePlayAPI.GooglePlayTopCharts(context.Background(), collection).Category(category).Country(country).Lang(lang).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GooglePlayAPI.GooglePlayTopCharts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePlayTopCharts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GooglePlayAPI.GooglePlayTopCharts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**collection** | **string** | topselling_free | topselling_paid | topgrossing | 

### Other Parameters

Other parameters are passed through a pointer to a apiGooglePlayTopChartsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **category** | **string** | Play category, e.g. &#39;GAME&#39; | [default to &quot;APPLICATION&quot;]
 **country** | **string** | Play storefront country (gl), ISO 3166-1 alpha-2, e.g. &#39;US&#39; | [default to &quot;US&quot;]
 **lang** | **string** | Play content language (hl), e.g. &#39;en&#39; or &#39;pt-BR&#39; | [default to &quot;en&quot;]
 **prefer** | **string** | &#x60;respond-async[, wait&#x3D;N]&#x60; (RFC 7240): run the call async. If it has not finished after &#x60;wait&#x60; seconds (0-120, default 25) the answer is &#x60;202&#x60; with a &#x60;request_id&#x60;; poll &#x60;GET /v1/requests/{request_id}&#x60;. Its &#x60;wait&#x3D;&#x60; wins over &#x60;async_wait&#x60;; without one, &#x60;async_wait&#x60; sets the wait. | 
 **xCallbackURL** | **string** | An &#x60;https&#x60; URL that receives the signed &#x60;request.completed&#x60; webhook when the call finishes. Implies async: on its own (no &#x60;Prefer&#x60;, &#x60;async&#x60; or &#x60;async_wait&#x60;) the answer is an immediate &#x60;202&#x60;; with &#x60;Prefer: respond-async&#x60; or &#x60;async&#x3D;true&#x60; the call still waits 25 s unless a wait is given. Wins over &#x60;callback_url&#x60;. | 
 **idempotencyKey** | **string** | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call&#39;s current state (&#x60;Idempotent-Replayed: true&#x60;) without running or billing it again; on a different call it is &#x60;409 idempotency_key_reused&#x60;. Applies to async calls only; on a synchronous call it is ignored. Wins over &#x60;idempotency_key&#x60;. | 
 **async** | **bool** | Query form of &#x60;Prefer: respond-async&#x60;: &#x60;true&#x60; or &#x60;1&#x60; (also &#x60;yes&#x60;, &#x60;on&#x60;; &#x60;false&#x60;, &#x60;0&#x60;, &#x60;no&#x60;, &#x60;off&#x60; leave the call synchronous). Waits 25 s unless &#x60;async_wait&#x60; is given. Not sent to the scraper. | 
 **asyncWait** | **int32** | Seconds (0-120; values outside are clamped) to wait for the result before answering &#x60;202&#x60;. Implies async. Not sent to the scraper. | 
 **callbackUrl** | **string** | Query form of &#x60;X-Callback-URL&#x60; (URL-encode it). Implies async; on its own the answer is an immediate &#x60;202&#x60; (wait 0). Not sent to the scraper. | 
 **idempotencyKey2** | **string** | Query form of &#x60;Idempotency-Key&#x60;. Not sent to the scraper. | 

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


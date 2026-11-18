# \ASOSAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AsosGetProductDetail**](ASOSAPI.md#AsosGetProductDetail) | **Get** /v1/asos/products/{product_id} | Get product detail
[**AsosGetStockAndPrices**](ASOSAPI.md#AsosGetStockAndPrices) | **Get** /v1/asos/stock-price | Get stock and prices
[**AsosListCategories**](ASOSAPI.md#AsosListCategories) | **Get** /v1/asos/categories | List categories
[**AsosListMarkets**](ASOSAPI.md#AsosListMarkets) | **Get** /v1/asos/markets | List markets
[**AsosListSearchFilters**](ASOSAPI.md#AsosListSearchFilters) | **Get** /v1/asos/filters | List search filters
[**AsosSearchProducts**](ASOSAPI.md#AsosSearchProducts) | **Get** /v1/asos/search | Search products
[**AsosSearchSuggestions**](ASOSAPI.md#AsosSearchSuggestions) | **Get** /v1/asos/autocomplete | Search suggestions



## AsosGetProductDetail

> ProductResponse AsosGetProductDetail(ctx, productId).Market(market).Store(store).Country(country).Currency(currency).Language(language).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()

Get product detail



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
	productId := int32(56) // int32 | 
	market := "market_example" // string | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl (optional) (default to "uk")
	store := "store_example" // string | Override store, e.g. COM or US (optional)
	country := "country_example" // string | ISO country override (optional)
	currency := "currency_example" // string | Currency override (optional)
	language := "language_example" // string | Locale override, e.g. en-GB (optional)
	prefer := "respond-async, wait=25" // string | `respond-async[, wait=N]` (RFC 7240): run the call async. If it has not finished after `wait` seconds (0-120, default 25) the answer is `202` with a `request_id`; poll `GET /v1/requests/{request_id}`. Its `wait=` wins over `async_wait`; without one, `async_wait` sets the wait. (optional)
	xCallbackURL := "xCallbackURL_example" // string | An `https` URL that receives the signed `request.completed` webhook when the call finishes. Implies async: on its own (no `Prefer`, `async` or `async_wait`) the answer is an immediate `202`; with `Prefer: respond-async` or `async=true` the call still waits 25 s unless a wait is given. Wins over `callback_url`. (optional)
	idempotencyKey := "idempotencyKey_example" // string | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call's current state (`Idempotent-Replayed: true`) without running or billing it again; on a different call it is `409 idempotency_key_reused`. Applies to async calls only; on a synchronous call it is ignored. Wins over `idempotency_key`. (optional)
	async := true // bool | Query form of `Prefer: respond-async`: `true` or `1` (also `yes`, `on`; `false`, `0`, `no`, `off` leave the call synchronous). Waits 25 s unless `async_wait` is given. Not sent to the scraper. (optional)
	asyncWait := int32(56) // int32 | Seconds (0-120; values outside are clamped) to wait for the result before answering `202`. Implies async. Not sent to the scraper. (optional)
	callbackUrl := "callbackUrl_example" // string | Query form of `X-Callback-URL` (URL-encode it). Implies async; on its own the answer is an immediate `202` (wait 0). Not sent to the scraper. (optional)
	idempotencyKey2 := "idempotencyKey_example" // string | Query form of `Idempotency-Key`. Not sent to the scraper. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ASOSAPI.AsosGetProductDetail(context.Background(), productId).Market(market).Store(store).Country(country).Currency(currency).Language(language).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ASOSAPI.AsosGetProductDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AsosGetProductDetail`: ProductResponse
	fmt.Fprintf(os.Stdout, "Response from `ASOSAPI.AsosGetProductDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**productId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAsosGetProductDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl | [default to &quot;uk&quot;]
 **store** | **string** | Override store, e.g. COM or US | 
 **country** | **string** | ISO country override | 
 **currency** | **string** | Currency override | 
 **language** | **string** | Locale override, e.g. en-GB | 
 **prefer** | **string** | &#x60;respond-async[, wait&#x3D;N]&#x60; (RFC 7240): run the call async. If it has not finished after &#x60;wait&#x60; seconds (0-120, default 25) the answer is &#x60;202&#x60; with a &#x60;request_id&#x60;; poll &#x60;GET /v1/requests/{request_id}&#x60;. Its &#x60;wait&#x3D;&#x60; wins over &#x60;async_wait&#x60;; without one, &#x60;async_wait&#x60; sets the wait. | 
 **xCallbackURL** | **string** | An &#x60;https&#x60; URL that receives the signed &#x60;request.completed&#x60; webhook when the call finishes. Implies async: on its own (no &#x60;Prefer&#x60;, &#x60;async&#x60; or &#x60;async_wait&#x60;) the answer is an immediate &#x60;202&#x60;; with &#x60;Prefer: respond-async&#x60; or &#x60;async&#x3D;true&#x60; the call still waits 25 s unless a wait is given. Wins over &#x60;callback_url&#x60;. | 
 **idempotencyKey** | **string** | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call&#39;s current state (&#x60;Idempotent-Replayed: true&#x60;) without running or billing it again; on a different call it is &#x60;409 idempotency_key_reused&#x60;. Applies to async calls only; on a synchronous call it is ignored. Wins over &#x60;idempotency_key&#x60;. | 
 **async** | **bool** | Query form of &#x60;Prefer: respond-async&#x60;: &#x60;true&#x60; or &#x60;1&#x60; (also &#x60;yes&#x60;, &#x60;on&#x60;; &#x60;false&#x60;, &#x60;0&#x60;, &#x60;no&#x60;, &#x60;off&#x60; leave the call synchronous). Waits 25 s unless &#x60;async_wait&#x60; is given. Not sent to the scraper. | 
 **asyncWait** | **int32** | Seconds (0-120; values outside are clamped) to wait for the result before answering &#x60;202&#x60;. Implies async. Not sent to the scraper. | 
 **callbackUrl** | **string** | Query form of &#x60;X-Callback-URL&#x60; (URL-encode it). Implies async; on its own the answer is an immediate &#x60;202&#x60; (wait 0). Not sent to the scraper. | 
 **idempotencyKey2** | **string** | Query form of &#x60;Idempotency-Key&#x60;. Not sent to the scraper. | 

### Return type

[**ProductResponse**](ProductResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AsosGetStockAndPrices

> StockResponse AsosGetStockAndPrices(ctx).ProductIds(productIds).Market(market).Store(store).Country(country).Currency(currency).Language(language).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()

Get stock and prices



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
	productIds := "productIds_example" // string | 1–50 comma-separated product ids
	market := "market_example" // string | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl (optional) (default to "uk")
	store := "store_example" // string | Override store, e.g. COM or US (optional)
	country := "country_example" // string | ISO country override (optional)
	currency := "currency_example" // string | Currency override (optional)
	language := "language_example" // string | Locale override, e.g. en-GB (optional)
	prefer := "respond-async, wait=25" // string | `respond-async[, wait=N]` (RFC 7240): run the call async. If it has not finished after `wait` seconds (0-120, default 25) the answer is `202` with a `request_id`; poll `GET /v1/requests/{request_id}`. Its `wait=` wins over `async_wait`; without one, `async_wait` sets the wait. (optional)
	xCallbackURL := "xCallbackURL_example" // string | An `https` URL that receives the signed `request.completed` webhook when the call finishes. Implies async: on its own (no `Prefer`, `async` or `async_wait`) the answer is an immediate `202`; with `Prefer: respond-async` or `async=true` the call still waits 25 s unless a wait is given. Wins over `callback_url`. (optional)
	idempotencyKey := "idempotencyKey_example" // string | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call's current state (`Idempotent-Replayed: true`) without running or billing it again; on a different call it is `409 idempotency_key_reused`. Applies to async calls only; on a synchronous call it is ignored. Wins over `idempotency_key`. (optional)
	async := true // bool | Query form of `Prefer: respond-async`: `true` or `1` (also `yes`, `on`; `false`, `0`, `no`, `off` leave the call synchronous). Waits 25 s unless `async_wait` is given. Not sent to the scraper. (optional)
	asyncWait := int32(56) // int32 | Seconds (0-120; values outside are clamped) to wait for the result before answering `202`. Implies async. Not sent to the scraper. (optional)
	callbackUrl := "callbackUrl_example" // string | Query form of `X-Callback-URL` (URL-encode it). Implies async; on its own the answer is an immediate `202` (wait 0). Not sent to the scraper. (optional)
	idempotencyKey2 := "idempotencyKey_example" // string | Query form of `Idempotency-Key`. Not sent to the scraper. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ASOSAPI.AsosGetStockAndPrices(context.Background()).ProductIds(productIds).Market(market).Store(store).Country(country).Currency(currency).Language(language).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ASOSAPI.AsosGetStockAndPrices``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AsosGetStockAndPrices`: StockResponse
	fmt.Fprintf(os.Stdout, "Response from `ASOSAPI.AsosGetStockAndPrices`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAsosGetStockAndPricesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productIds** | **string** | 1–50 comma-separated product ids | 
 **market** | **string** | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl | [default to &quot;uk&quot;]
 **store** | **string** | Override store, e.g. COM or US | 
 **country** | **string** | ISO country override | 
 **currency** | **string** | Currency override | 
 **language** | **string** | Locale override, e.g. en-GB | 
 **prefer** | **string** | &#x60;respond-async[, wait&#x3D;N]&#x60; (RFC 7240): run the call async. If it has not finished after &#x60;wait&#x60; seconds (0-120, default 25) the answer is &#x60;202&#x60; with a &#x60;request_id&#x60;; poll &#x60;GET /v1/requests/{request_id}&#x60;. Its &#x60;wait&#x3D;&#x60; wins over &#x60;async_wait&#x60;; without one, &#x60;async_wait&#x60; sets the wait. | 
 **xCallbackURL** | **string** | An &#x60;https&#x60; URL that receives the signed &#x60;request.completed&#x60; webhook when the call finishes. Implies async: on its own (no &#x60;Prefer&#x60;, &#x60;async&#x60; or &#x60;async_wait&#x60;) the answer is an immediate &#x60;202&#x60;; with &#x60;Prefer: respond-async&#x60; or &#x60;async&#x3D;true&#x60; the call still waits 25 s unless a wait is given. Wins over &#x60;callback_url&#x60;. | 
 **idempotencyKey** | **string** | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call&#39;s current state (&#x60;Idempotent-Replayed: true&#x60;) without running or billing it again; on a different call it is &#x60;409 idempotency_key_reused&#x60;. Applies to async calls only; on a synchronous call it is ignored. Wins over &#x60;idempotency_key&#x60;. | 
 **async** | **bool** | Query form of &#x60;Prefer: respond-async&#x60;: &#x60;true&#x60; or &#x60;1&#x60; (also &#x60;yes&#x60;, &#x60;on&#x60;; &#x60;false&#x60;, &#x60;0&#x60;, &#x60;no&#x60;, &#x60;off&#x60; leave the call synchronous). Waits 25 s unless &#x60;async_wait&#x60; is given. Not sent to the scraper. | 
 **asyncWait** | **int32** | Seconds (0-120; values outside are clamped) to wait for the result before answering &#x60;202&#x60;. Implies async. Not sent to the scraper. | 
 **callbackUrl** | **string** | Query form of &#x60;X-Callback-URL&#x60; (URL-encode it). Implies async; on its own the answer is an immediate &#x60;202&#x60; (wait 0). Not sent to the scraper. | 
 **idempotencyKey2** | **string** | Query form of &#x60;Idempotency-Key&#x60;. Not sent to the scraper. | 

### Return type

[**StockResponse**](StockResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AsosListCategories

> interface{} AsosListCategories(ctx).Gender(gender).Market(market).Store(store).Country(country).Currency(currency).Language(language).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()

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
	gender := "gender_example" // string |  (optional) (default to "men")
	market := "market_example" // string | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl (optional) (default to "uk")
	store := "store_example" // string | Override store, e.g. COM or US (optional)
	country := "country_example" // string | ISO country override (optional)
	currency := "currency_example" // string | Currency override (optional)
	language := "language_example" // string | Locale override, e.g. en-GB (optional)
	prefer := "respond-async, wait=25" // string | `respond-async[, wait=N]` (RFC 7240): run the call async. If it has not finished after `wait` seconds (0-120, default 25) the answer is `202` with a `request_id`; poll `GET /v1/requests/{request_id}`. Its `wait=` wins over `async_wait`; without one, `async_wait` sets the wait. (optional)
	xCallbackURL := "xCallbackURL_example" // string | An `https` URL that receives the signed `request.completed` webhook when the call finishes. Implies async: on its own (no `Prefer`, `async` or `async_wait`) the answer is an immediate `202`; with `Prefer: respond-async` or `async=true` the call still waits 25 s unless a wait is given. Wins over `callback_url`. (optional)
	idempotencyKey := "idempotencyKey_example" // string | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call's current state (`Idempotent-Replayed: true`) without running or billing it again; on a different call it is `409 idempotency_key_reused`. Applies to async calls only; on a synchronous call it is ignored. Wins over `idempotency_key`. (optional)
	async := true // bool | Query form of `Prefer: respond-async`: `true` or `1` (also `yes`, `on`; `false`, `0`, `no`, `off` leave the call synchronous). Waits 25 s unless `async_wait` is given. Not sent to the scraper. (optional)
	asyncWait := int32(56) // int32 | Seconds (0-120; values outside are clamped) to wait for the result before answering `202`. Implies async. Not sent to the scraper. (optional)
	callbackUrl := "callbackUrl_example" // string | Query form of `X-Callback-URL` (URL-encode it). Implies async; on its own the answer is an immediate `202` (wait 0). Not sent to the scraper. (optional)
	idempotencyKey2 := "idempotencyKey_example" // string | Query form of `Idempotency-Key`. Not sent to the scraper. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ASOSAPI.AsosListCategories(context.Background()).Gender(gender).Market(market).Store(store).Country(country).Currency(currency).Language(language).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ASOSAPI.AsosListCategories``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AsosListCategories`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ASOSAPI.AsosListCategories`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAsosListCategoriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gender** | **string** |  | [default to &quot;men&quot;]
 **market** | **string** | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl | [default to &quot;uk&quot;]
 **store** | **string** | Override store, e.g. COM or US | 
 **country** | **string** | ISO country override | 
 **currency** | **string** | Currency override | 
 **language** | **string** | Locale override, e.g. en-GB | 
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


## AsosListMarkets

> interface{} AsosListMarkets(ctx).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()

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
	resp, r, err := apiClient.ASOSAPI.AsosListMarkets(context.Background()).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ASOSAPI.AsosListMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AsosListMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ASOSAPI.AsosListMarkets`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAsosListMarketsRequest struct via the builder pattern


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


## AsosListSearchFilters

> interface{} AsosListSearchFilters(ctx).Query(query).CategoryId(categoryId).Market(market).Store(store).Country(country).Currency(currency).Language(language).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()

List search filters



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
	query := "query_example" // string |  (optional)
	categoryId := int32(56) // int32 |  (optional)
	market := "market_example" // string | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl (optional) (default to "uk")
	store := "store_example" // string | Override store, e.g. COM or US (optional)
	country := "country_example" // string | ISO country override (optional)
	currency := "currency_example" // string | Currency override (optional)
	language := "language_example" // string | Locale override, e.g. en-GB (optional)
	prefer := "respond-async, wait=25" // string | `respond-async[, wait=N]` (RFC 7240): run the call async. If it has not finished after `wait` seconds (0-120, default 25) the answer is `202` with a `request_id`; poll `GET /v1/requests/{request_id}`. Its `wait=` wins over `async_wait`; without one, `async_wait` sets the wait. (optional)
	xCallbackURL := "xCallbackURL_example" // string | An `https` URL that receives the signed `request.completed` webhook when the call finishes. Implies async: on its own (no `Prefer`, `async` or `async_wait`) the answer is an immediate `202`; with `Prefer: respond-async` or `async=true` the call still waits 25 s unless a wait is given. Wins over `callback_url`. (optional)
	idempotencyKey := "idempotencyKey_example" // string | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call's current state (`Idempotent-Replayed: true`) without running or billing it again; on a different call it is `409 idempotency_key_reused`. Applies to async calls only; on a synchronous call it is ignored. Wins over `idempotency_key`. (optional)
	async := true // bool | Query form of `Prefer: respond-async`: `true` or `1` (also `yes`, `on`; `false`, `0`, `no`, `off` leave the call synchronous). Waits 25 s unless `async_wait` is given. Not sent to the scraper. (optional)
	asyncWait := int32(56) // int32 | Seconds (0-120; values outside are clamped) to wait for the result before answering `202`. Implies async. Not sent to the scraper. (optional)
	callbackUrl := "callbackUrl_example" // string | Query form of `X-Callback-URL` (URL-encode it). Implies async; on its own the answer is an immediate `202` (wait 0). Not sent to the scraper. (optional)
	idempotencyKey2 := "idempotencyKey_example" // string | Query form of `Idempotency-Key`. Not sent to the scraper. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ASOSAPI.AsosListSearchFilters(context.Background()).Query(query).CategoryId(categoryId).Market(market).Store(store).Country(country).Currency(currency).Language(language).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ASOSAPI.AsosListSearchFilters``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AsosListSearchFilters`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ASOSAPI.AsosListSearchFilters`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAsosListSearchFiltersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 
 **categoryId** | **int32** |  | 
 **market** | **string** | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl | [default to &quot;uk&quot;]
 **store** | **string** | Override store, e.g. COM or US | 
 **country** | **string** | ISO country override | 
 **currency** | **string** | Currency override | 
 **language** | **string** | Locale override, e.g. en-GB | 
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


## AsosSearchProducts

> PortalApiRoutersV1AsosSearchResponse AsosSearchProducts(ctx).Query(query).CategoryId(categoryId).Offset(offset).Limit(limit).Sort(sort).Brand(brand).Colour(colour).Size(size).MinPrice(minPrice).MaxPrice(maxPrice).Market(market).Store(store).Country(country).Currency(currency).Language(language).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()

Search products



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
	query := "query_example" // string | Keyword, e.g. shoes (optional)
	categoryId := int32(56) // int32 | Category id from navigation (optional)
	offset := int32(56) // int32 |  (optional) (default to 0)
	limit := int32(56) // int32 |  (optional) (default to 48)
	sort := "sort_example" // string |  (optional) (default to "recommended")
	brand := "brand_example" // string | Comma-separated brand facet ids (optional)
	colour := "colour_example" // string | Comma-separated colour facet ids (optional)
	size := "size_example" // string | Comma-separated size facet ids (optional)
	minPrice := float32(8.14) // float32 |  (optional)
	maxPrice := float32(8.14) // float32 |  (optional)
	market := "market_example" // string | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl (optional) (default to "uk")
	store := "store_example" // string | Override store, e.g. COM or US (optional)
	country := "country_example" // string | ISO country override (optional)
	currency := "currency_example" // string | Currency override (optional)
	language := "language_example" // string | Locale override, e.g. en-GB (optional)
	prefer := "respond-async, wait=25" // string | `respond-async[, wait=N]` (RFC 7240): run the call async. If it has not finished after `wait` seconds (0-120, default 25) the answer is `202` with a `request_id`; poll `GET /v1/requests/{request_id}`. Its `wait=` wins over `async_wait`; without one, `async_wait` sets the wait. (optional)
	xCallbackURL := "xCallbackURL_example" // string | An `https` URL that receives the signed `request.completed` webhook when the call finishes. Implies async: on its own (no `Prefer`, `async` or `async_wait`) the answer is an immediate `202`; with `Prefer: respond-async` or `async=true` the call still waits 25 s unless a wait is given. Wins over `callback_url`. (optional)
	idempotencyKey := "idempotencyKey_example" // string | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call's current state (`Idempotent-Replayed: true`) without running or billing it again; on a different call it is `409 idempotency_key_reused`. Applies to async calls only; on a synchronous call it is ignored. Wins over `idempotency_key`. (optional)
	async := true // bool | Query form of `Prefer: respond-async`: `true` or `1` (also `yes`, `on`; `false`, `0`, `no`, `off` leave the call synchronous). Waits 25 s unless `async_wait` is given. Not sent to the scraper. (optional)
	asyncWait := int32(56) // int32 | Seconds (0-120; values outside are clamped) to wait for the result before answering `202`. Implies async. Not sent to the scraper. (optional)
	callbackUrl := "callbackUrl_example" // string | Query form of `X-Callback-URL` (URL-encode it). Implies async; on its own the answer is an immediate `202` (wait 0). Not sent to the scraper. (optional)
	idempotencyKey2 := "idempotencyKey_example" // string | Query form of `Idempotency-Key`. Not sent to the scraper. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ASOSAPI.AsosSearchProducts(context.Background()).Query(query).CategoryId(categoryId).Offset(offset).Limit(limit).Sort(sort).Brand(brand).Colour(colour).Size(size).MinPrice(minPrice).MaxPrice(maxPrice).Market(market).Store(store).Country(country).Currency(currency).Language(language).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ASOSAPI.AsosSearchProducts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AsosSearchProducts`: PortalApiRoutersV1AsosSearchResponse
	fmt.Fprintf(os.Stdout, "Response from `ASOSAPI.AsosSearchProducts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAsosSearchProductsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Keyword, e.g. shoes | 
 **categoryId** | **int32** | Category id from navigation | 
 **offset** | **int32** |  | [default to 0]
 **limit** | **int32** |  | [default to 48]
 **sort** | **string** |  | [default to &quot;recommended&quot;]
 **brand** | **string** | Comma-separated brand facet ids | 
 **colour** | **string** | Comma-separated colour facet ids | 
 **size** | **string** | Comma-separated size facet ids | 
 **minPrice** | **float32** |  | 
 **maxPrice** | **float32** |  | 
 **market** | **string** | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl | [default to &quot;uk&quot;]
 **store** | **string** | Override store, e.g. COM or US | 
 **country** | **string** | ISO country override | 
 **currency** | **string** | Currency override | 
 **language** | **string** | Locale override, e.g. en-GB | 
 **prefer** | **string** | &#x60;respond-async[, wait&#x3D;N]&#x60; (RFC 7240): run the call async. If it has not finished after &#x60;wait&#x60; seconds (0-120, default 25) the answer is &#x60;202&#x60; with a &#x60;request_id&#x60;; poll &#x60;GET /v1/requests/{request_id}&#x60;. Its &#x60;wait&#x3D;&#x60; wins over &#x60;async_wait&#x60;; without one, &#x60;async_wait&#x60; sets the wait. | 
 **xCallbackURL** | **string** | An &#x60;https&#x60; URL that receives the signed &#x60;request.completed&#x60; webhook when the call finishes. Implies async: on its own (no &#x60;Prefer&#x60;, &#x60;async&#x60; or &#x60;async_wait&#x60;) the answer is an immediate &#x60;202&#x60;; with &#x60;Prefer: respond-async&#x60; or &#x60;async&#x3D;true&#x60; the call still waits 25 s unless a wait is given. Wins over &#x60;callback_url&#x60;. | 
 **idempotencyKey** | **string** | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call&#39;s current state (&#x60;Idempotent-Replayed: true&#x60;) without running or billing it again; on a different call it is &#x60;409 idempotency_key_reused&#x60;. Applies to async calls only; on a synchronous call it is ignored. Wins over &#x60;idempotency_key&#x60;. | 
 **async** | **bool** | Query form of &#x60;Prefer: respond-async&#x60;: &#x60;true&#x60; or &#x60;1&#x60; (also &#x60;yes&#x60;, &#x60;on&#x60;; &#x60;false&#x60;, &#x60;0&#x60;, &#x60;no&#x60;, &#x60;off&#x60; leave the call synchronous). Waits 25 s unless &#x60;async_wait&#x60; is given. Not sent to the scraper. | 
 **asyncWait** | **int32** | Seconds (0-120; values outside are clamped) to wait for the result before answering &#x60;202&#x60;. Implies async. Not sent to the scraper. | 
 **callbackUrl** | **string** | Query form of &#x60;X-Callback-URL&#x60; (URL-encode it). Implies async; on its own the answer is an immediate &#x60;202&#x60; (wait 0). Not sent to the scraper. | 
 **idempotencyKey2** | **string** | Query form of &#x60;Idempotency-Key&#x60;. Not sent to the scraper. | 

### Return type

[**PortalApiRoutersV1AsosSearchResponse**](PortalApiRoutersV1AsosSearchResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AsosSearchSuggestions

> interface{} AsosSearchSuggestions(ctx).Query(query).Market(market).Store(store).Country(country).Currency(currency).Language(language).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()

Search suggestions



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
	query := "query_example" // string | 
	market := "market_example" // string | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl (optional) (default to "uk")
	store := "store_example" // string | Override store, e.g. COM or US (optional)
	country := "country_example" // string | ISO country override (optional)
	currency := "currency_example" // string | Currency override (optional)
	language := "language_example" // string | Locale override, e.g. en-GB (optional)
	prefer := "respond-async, wait=25" // string | `respond-async[, wait=N]` (RFC 7240): run the call async. If it has not finished after `wait` seconds (0-120, default 25) the answer is `202` with a `request_id`; poll `GET /v1/requests/{request_id}`. Its `wait=` wins over `async_wait`; without one, `async_wait` sets the wait. (optional)
	xCallbackURL := "xCallbackURL_example" // string | An `https` URL that receives the signed `request.completed` webhook when the call finishes. Implies async: on its own (no `Prefer`, `async` or `async_wait`) the answer is an immediate `202`; with `Prefer: respond-async` or `async=true` the call still waits 25 s unless a wait is given. Wins over `callback_url`. (optional)
	idempotencyKey := "idempotencyKey_example" // string | 1-200 visible ASCII characters, per account, kept as long as the result (about 15 minutes). The same key on the same call returns that call's current state (`Idempotent-Replayed: true`) without running or billing it again; on a different call it is `409 idempotency_key_reused`. Applies to async calls only; on a synchronous call it is ignored. Wins over `idempotency_key`. (optional)
	async := true // bool | Query form of `Prefer: respond-async`: `true` or `1` (also `yes`, `on`; `false`, `0`, `no`, `off` leave the call synchronous). Waits 25 s unless `async_wait` is given. Not sent to the scraper. (optional)
	asyncWait := int32(56) // int32 | Seconds (0-120; values outside are clamped) to wait for the result before answering `202`. Implies async. Not sent to the scraper. (optional)
	callbackUrl := "callbackUrl_example" // string | Query form of `X-Callback-URL` (URL-encode it). Implies async; on its own the answer is an immediate `202` (wait 0). Not sent to the scraper. (optional)
	idempotencyKey2 := "idempotencyKey_example" // string | Query form of `Idempotency-Key`. Not sent to the scraper. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ASOSAPI.AsosSearchSuggestions(context.Background()).Query(query).Market(market).Store(store).Country(country).Currency(currency).Language(language).Prefer(prefer).XCallbackURL(xCallbackURL).IdempotencyKey(idempotencyKey).Async(async).AsyncWait(asyncWait).CallbackUrl(callbackUrl).IdempotencyKey2(idempotencyKey2).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ASOSAPI.AsosSearchSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AsosSearchSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ASOSAPI.AsosSearchSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAsosSearchSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 
 **market** | **string** | Storefront: uk, us, au, de, fr, it, es, nl, se, dk, pl | [default to &quot;uk&quot;]
 **store** | **string** | Override store, e.g. COM or US | 
 **country** | **string** | ISO country override | 
 **currency** | **string** | Currency override | 
 **language** | **string** | Locale override, e.g. en-GB | 
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


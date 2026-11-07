# \YelpAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**YelpListMarkets**](YelpAPI.md#YelpListMarkets) | **Get** /v1/yelp/markets | List markets
[**YelpSearchBusinesses**](YelpAPI.md#YelpSearchBusinesses) | **Get** /v1/yelp/search | Search businesses



## YelpListMarkets

> YelpMarketsResponse YelpListMarkets(ctx).Execute()

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YelpAPI.YelpListMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YelpAPI.YelpListMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YelpListMarkets`: YelpMarketsResponse
	fmt.Fprintf(os.Stdout, "Response from `YelpAPI.YelpListMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiYelpListMarketsRequest struct via the builder pattern


### Return type

[**YelpMarketsResponse**](YelpMarketsResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## YelpSearchBusinesses

> YelpSearchResponse YelpSearchBusinesses(ctx).Location(location).Query(query).Market(market).Category(category).SortBy(sortBy).Price(price).Features(features).Page(page).Execute()

Search businesses



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
	location := "location_example" // string | Where to search, as typed into Yelp: city, neighbourhood, address or postcode.
	query := "query_example" // string | What to search for (e.g. pizza, plumbers). Optional when category is set. (optional)
	market := "market_example" // string | Yelp site to search; see /markets. (optional) (default to "us")
	category := "category_example" // string | Yelp category alias, e.g. pizza, coffee, plumbing. (optional)
	sortBy := "sortBy_example" // string |  (optional) (default to "recommended")
	price := "price_example" // string | Comma-separated price levels 1-4 ($ to $$$$). (optional)
	features := "features_example" // string | Comma-separated refinements: delivery, takeout, reservations, outdoor_seating, good_for_kids, dogs_allowed, free_wifi, wheelchair_accessible. (optional)
	page := int32(56) // int32 | 1-based page, ten businesses each; pages 1-11. (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YelpAPI.YelpSearchBusinesses(context.Background()).Location(location).Query(query).Market(market).Category(category).SortBy(sortBy).Price(price).Features(features).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YelpAPI.YelpSearchBusinesses``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YelpSearchBusinesses`: YelpSearchResponse
	fmt.Fprintf(os.Stdout, "Response from `YelpAPI.YelpSearchBusinesses`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiYelpSearchBusinessesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **location** | **string** | Where to search, as typed into Yelp: city, neighbourhood, address or postcode. | 
 **query** | **string** | What to search for (e.g. pizza, plumbers). Optional when category is set. | 
 **market** | **string** | Yelp site to search; see /markets. | [default to &quot;us&quot;]
 **category** | **string** | Yelp category alias, e.g. pizza, coffee, plumbing. | 
 **sortBy** | **string** |  | [default to &quot;recommended&quot;]
 **price** | **string** | Comma-separated price levels 1-4 ($ to $$$$). | 
 **features** | **string** | Comma-separated refinements: delivery, takeout, reservations, outdoor_seating, good_for_kids, dogs_allowed, free_wifi, wheelchair_accessible. | 
 **page** | **int32** | 1-based page, ten businesses each; pages 1-11. | [default to 1]

### Return type

[**YelpSearchResponse**](YelpSearchResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


# \RedfinAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**RedfinGetAgentProfileListings**](RedfinAPI.md#RedfinGetAgentProfileListings) | **Get** /v1/redfin/agent | Get agent profile + listings
[**RedfinGetPropertyDetail**](RedfinAPI.md#RedfinGetPropertyDetail) | **Get** /v1/redfin/property/{property_id} | Get property detail
[**RedfinGetPropertyDetailByUrl**](RedfinAPI.md#RedfinGetPropertyDetailByUrl) | **Get** /v1/redfin/property | Get property detail by URL
[**RedfinListCoverageMarkets**](RedfinAPI.md#RedfinListCoverageMarkets) | **Get** /v1/redfin/markets | List coverage markets
[**RedfinRedfinScraperHealthCheck**](RedfinAPI.md#RedfinRedfinScraperHealthCheck) | **Get** /v1/redfin/health | Redfin scraper health check
[**RedfinRedfinScraperHealthCheckHead**](RedfinAPI.md#RedfinRedfinScraperHealthCheckHead) | **Head** /v1/redfin/health | Redfin scraper health check
[**RedfinRegionAddressSuggestions**](RedfinAPI.md#RedfinRegionAddressSuggestions) | **Get** /v1/redfin/autocomplete | Region/address suggestions
[**RedfinSearchProperties**](RedfinAPI.md#RedfinSearchProperties) | **Get** /v1/redfin/search | Search properties



## RedfinGetAgentProfileListings

> interface{} RedfinGetAgentProfileListings(ctx).Url(url).AgentId(agentId).Execute()

Get agent profile + listings



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
	url := "url_example" // string | Full Redfin /realestateagents/ URL (optional)
	agentId := "agentId_example" // string | Redfin agent id (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedfinAPI.RedfinGetAgentProfileListings(context.Background()).Url(url).AgentId(agentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedfinAPI.RedfinGetAgentProfileListings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedfinGetAgentProfileListings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedfinAPI.RedfinGetAgentProfileListings`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRedfinGetAgentProfileListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **url** | **string** | Full Redfin /realestateagents/ URL | 
 **agentId** | **string** | Redfin agent id | 

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


## RedfinGetPropertyDetail

> interface{} RedfinGetPropertyDetail(ctx, propertyId).Execute()

Get property detail



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
	propertyId := "propertyId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedfinAPI.RedfinGetPropertyDetail(context.Background(), propertyId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedfinAPI.RedfinGetPropertyDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedfinGetPropertyDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedfinAPI.RedfinGetPropertyDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**propertyId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRedfinGetPropertyDetailRequest struct via the builder pattern


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


## RedfinGetPropertyDetailByUrl

> interface{} RedfinGetPropertyDetailByUrl(ctx).Url(url).Execute()

Get property detail by URL



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
	url := "url_example" // string | Full Redfin property URL (/CA/City/.../home/12345678)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedfinAPI.RedfinGetPropertyDetailByUrl(context.Background()).Url(url).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedfinAPI.RedfinGetPropertyDetailByUrl``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedfinGetPropertyDetailByUrl`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedfinAPI.RedfinGetPropertyDetailByUrl`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRedfinGetPropertyDetailByUrlRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **url** | **string** | Full Redfin property URL (/CA/City/.../home/12345678) | 

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


## RedfinListCoverageMarkets

> interface{} RedfinListCoverageMarkets(ctx).Execute()

List coverage markets



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
	resp, r, err := apiClient.RedfinAPI.RedfinListCoverageMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedfinAPI.RedfinListCoverageMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedfinListCoverageMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedfinAPI.RedfinListCoverageMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiRedfinListCoverageMarketsRequest struct via the builder pattern


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


## RedfinRedfinScraperHealthCheck

> interface{} RedfinRedfinScraperHealthCheck(ctx).Execute()

Redfin scraper health check



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
	resp, r, err := apiClient.RedfinAPI.RedfinRedfinScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedfinAPI.RedfinRedfinScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedfinRedfinScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedfinAPI.RedfinRedfinScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiRedfinRedfinScraperHealthCheckRequest struct via the builder pattern


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


## RedfinRedfinScraperHealthCheckHead

> interface{} RedfinRedfinScraperHealthCheckHead(ctx).Execute()

Redfin scraper health check



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
	resp, r, err := apiClient.RedfinAPI.RedfinRedfinScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedfinAPI.RedfinRedfinScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedfinRedfinScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedfinAPI.RedfinRedfinScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiRedfinRedfinScraperHealthCheckHeadRequest struct via the builder pattern


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


## RedfinRegionAddressSuggestions

> interface{} RedfinRegionAddressSuggestions(ctx).Query(query).Execute()

Region/address suggestions



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
	query := "query_example" // string | Partial location — city, ZIP, address, neighborhood

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedfinAPI.RedfinRegionAddressSuggestions(context.Background()).Query(query).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedfinAPI.RedfinRegionAddressSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedfinRegionAddressSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedfinAPI.RedfinRegionAddressSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRedfinRegionAddressSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Partial location — city, ZIP, address, neighborhood | 

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


## RedfinSearchProperties

> interface{} RedfinSearchProperties(ctx).Location(location).Page(page).Sort(sort).PriceMin(priceMin).PriceMax(priceMax).BedsMin(bedsMin).BathsMin(bathsMin).HomeType(homeType).SqftMin(sqftMin).SqftMax(sqftMax).LotMin(lotMin).LotMax(lotMax).YearBuiltMin(yearBuiltMin).YearBuiltMax(yearBuiltMax).MaxDaysOnMarket(maxDaysOnMarket).North(north).South(south).East(east).West(west).Execute()

Search properties



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
	location := "location_example" // string | City/state, ZIP, address or neighborhood
	page := int32(56) // int32 |  (optional) (default to 1)
	sort := "sort_example" // string | relevant|newest|price_high_to_low|price_low_to_high|square_feet|lot_size|price_per_sqft|beds|baths (optional)
	priceMin := int32(56) // int32 |  (optional)
	priceMax := int32(56) // int32 |  (optional)
	bedsMin := int32(56) // int32 |  (optional)
	bathsMin := float32(8.14) // float32 |  (optional)
	homeType := "homeType_example" // string | house|condo|townhouse|multi_family|land|mobile|coop|other (optional)
	sqftMin := int32(56) // int32 |  (optional)
	sqftMax := int32(56) // int32 |  (optional)
	lotMin := int32(56) // int32 |  (optional)
	lotMax := int32(56) // int32 |  (optional)
	yearBuiltMin := int32(56) // int32 |  (optional)
	yearBuiltMax := int32(56) // int32 |  (optional)
	maxDaysOnMarket := int32(56) // int32 |  (optional)
	north := float32(8.14) // float32 | Map bounds for tiling past the cap (optional)
	south := float32(8.14) // float32 |  (optional)
	east := float32(8.14) // float32 |  (optional)
	west := float32(8.14) // float32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedfinAPI.RedfinSearchProperties(context.Background()).Location(location).Page(page).Sort(sort).PriceMin(priceMin).PriceMax(priceMax).BedsMin(bedsMin).BathsMin(bathsMin).HomeType(homeType).SqftMin(sqftMin).SqftMax(sqftMax).LotMin(lotMin).LotMax(lotMax).YearBuiltMin(yearBuiltMin).YearBuiltMax(yearBuiltMax).MaxDaysOnMarket(maxDaysOnMarket).North(north).South(south).East(east).West(west).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedfinAPI.RedfinSearchProperties``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedfinSearchProperties`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedfinAPI.RedfinSearchProperties`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRedfinSearchPropertiesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **location** | **string** | City/state, ZIP, address or neighborhood | 
 **page** | **int32** |  | [default to 1]
 **sort** | **string** | relevant|newest|price_high_to_low|price_low_to_high|square_feet|lot_size|price_per_sqft|beds|baths | 
 **priceMin** | **int32** |  | 
 **priceMax** | **int32** |  | 
 **bedsMin** | **int32** |  | 
 **bathsMin** | **float32** |  | 
 **homeType** | **string** | house|condo|townhouse|multi_family|land|mobile|coop|other | 
 **sqftMin** | **int32** |  | 
 **sqftMax** | **int32** |  | 
 **lotMin** | **int32** |  | 
 **lotMax** | **int32** |  | 
 **yearBuiltMin** | **int32** |  | 
 **yearBuiltMax** | **int32** |  | 
 **maxDaysOnMarket** | **int32** |  | 
 **north** | **float32** | Map bounds for tiling past the cap | 
 **south** | **float32** |  | 
 **east** | **float32** |  | 
 **west** | **float32** |  | 

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


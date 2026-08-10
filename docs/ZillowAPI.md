# \ZillowAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ZillowGetAgentProfileListings**](ZillowAPI.md#ZillowGetAgentProfileListings) | **Get** /v1/zillow/agent | Get agent profile + listings
[**ZillowGetPropertyDetail**](ZillowAPI.md#ZillowGetPropertyDetail) | **Get** /v1/zillow/property/{zpid} | Get property detail
[**ZillowGetPropertyDetailByUrl**](ZillowAPI.md#ZillowGetPropertyDetailByUrl) | **Get** /v1/zillow/property | Get property detail by URL
[**ZillowListCoverageMarkets**](ZillowAPI.md#ZillowListCoverageMarkets) | **Get** /v1/zillow/markets | List coverage markets
[**ZillowRegionAddressSuggestions**](ZillowAPI.md#ZillowRegionAddressSuggestions) | **Get** /v1/zillow/autocomplete | Region/address suggestions
[**ZillowSearchProperties**](ZillowAPI.md#ZillowSearchProperties) | **Get** /v1/zillow/search | Search properties
[**ZillowZillowScraperHealthCheck**](ZillowAPI.md#ZillowZillowScraperHealthCheck) | **Get** /v1/zillow/health | Zillow scraper health check
[**ZillowZillowScraperHealthCheckHead**](ZillowAPI.md#ZillowZillowScraperHealthCheckHead) | **Head** /v1/zillow/health | Zillow scraper health check



## ZillowGetAgentProfileListings

> interface{} ZillowGetAgentProfileListings(ctx).Username(username).Url(url).Execute()

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
	username := "username_example" // string | Zillow profile username (optional)
	url := "url_example" // string | Full Zillow /profile/... URL (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ZillowAPI.ZillowGetAgentProfileListings(context.Background()).Username(username).Url(url).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ZillowAPI.ZillowGetAgentProfileListings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ZillowGetAgentProfileListings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ZillowAPI.ZillowGetAgentProfileListings`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiZillowGetAgentProfileListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **username** | **string** | Zillow profile username | 
 **url** | **string** | Full Zillow /profile/... URL | 

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


## ZillowGetPropertyDetail

> interface{} ZillowGetPropertyDetail(ctx, zpid).Execute()

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
	zpid := "zpid_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ZillowAPI.ZillowGetPropertyDetail(context.Background(), zpid).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ZillowAPI.ZillowGetPropertyDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ZillowGetPropertyDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ZillowAPI.ZillowGetPropertyDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**zpid** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiZillowGetPropertyDetailRequest struct via the builder pattern


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


## ZillowGetPropertyDetailByUrl

> interface{} ZillowGetPropertyDetailByUrl(ctx).Url(url).Execute()

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
	url := "url_example" // string | Full Zillow /homedetails/... URL

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ZillowAPI.ZillowGetPropertyDetailByUrl(context.Background()).Url(url).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ZillowAPI.ZillowGetPropertyDetailByUrl``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ZillowGetPropertyDetailByUrl`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ZillowAPI.ZillowGetPropertyDetailByUrl`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiZillowGetPropertyDetailByUrlRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **url** | **string** | Full Zillow /homedetails/... URL | 

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


## ZillowListCoverageMarkets

> interface{} ZillowListCoverageMarkets(ctx).Execute()

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
	resp, r, err := apiClient.ZillowAPI.ZillowListCoverageMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ZillowAPI.ZillowListCoverageMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ZillowListCoverageMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ZillowAPI.ZillowListCoverageMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiZillowListCoverageMarketsRequest struct via the builder pattern


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


## ZillowRegionAddressSuggestions

> interface{} ZillowRegionAddressSuggestions(ctx).Query(query).Execute()

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
	resp, r, err := apiClient.ZillowAPI.ZillowRegionAddressSuggestions(context.Background()).Query(query).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ZillowAPI.ZillowRegionAddressSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ZillowRegionAddressSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ZillowAPI.ZillowRegionAddressSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiZillowRegionAddressSuggestionsRequest struct via the builder pattern


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


## ZillowSearchProperties

> interface{} ZillowSearchProperties(ctx).Location(location).Status(status).Page(page).Sort(sort).PriceMin(priceMin).PriceMax(priceMax).BedsMin(bedsMin).BathsMin(bathsMin).HomeType(homeType).SqftMin(sqftMin).SqftMax(sqftMax).LotMin(lotMin).LotMax(lotMax).YearBuiltMin(yearBuiltMin).YearBuiltMax(yearBuiltMax).HoaMax(hoaMax).Keywords(keywords).DaysOn(daysOn).North(north).South(south).East(east).West(west).Execute()

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
	status := "status_example" // string | for_sale|for_rent|sold (optional) (default to "for_sale")
	page := int32(56) // int32 |  (optional) (default to 1)
	sort := "sort_example" // string | homes_for_you|newest|price_high_to_low|price_low_to_high|bedrooms|bathrooms|square_feet|lot_size|year_built (optional)
	priceMin := int32(56) // int32 |  (optional)
	priceMax := int32(56) // int32 |  (optional)
	bedsMin := int32(56) // int32 |  (optional)
	bathsMin := float32(8.14) // float32 |  (optional)
	homeType := "homeType_example" // string | houses|condos|townhomes|apartments|manufactured|lots|multi_family (optional)
	sqftMin := int32(56) // int32 |  (optional)
	sqftMax := int32(56) // int32 |  (optional)
	lotMin := int32(56) // int32 |  (optional)
	lotMax := int32(56) // int32 |  (optional)
	yearBuiltMin := int32(56) // int32 |  (optional)
	yearBuiltMax := int32(56) // int32 |  (optional)
	hoaMax := int32(56) // int32 |  (optional)
	keywords := "keywords_example" // string |  (optional)
	daysOn := "daysOn_example" // string |  (optional)
	north := float32(8.14) // float32 | Map bounds for tiling past the 820 cap (optional)
	south := float32(8.14) // float32 |  (optional)
	east := float32(8.14) // float32 |  (optional)
	west := float32(8.14) // float32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ZillowAPI.ZillowSearchProperties(context.Background()).Location(location).Status(status).Page(page).Sort(sort).PriceMin(priceMin).PriceMax(priceMax).BedsMin(bedsMin).BathsMin(bathsMin).HomeType(homeType).SqftMin(sqftMin).SqftMax(sqftMax).LotMin(lotMin).LotMax(lotMax).YearBuiltMin(yearBuiltMin).YearBuiltMax(yearBuiltMax).HoaMax(hoaMax).Keywords(keywords).DaysOn(daysOn).North(north).South(south).East(east).West(west).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ZillowAPI.ZillowSearchProperties``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ZillowSearchProperties`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ZillowAPI.ZillowSearchProperties`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiZillowSearchPropertiesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **location** | **string** | City/state, ZIP, address or neighborhood | 
 **status** | **string** | for_sale|for_rent|sold | [default to &quot;for_sale&quot;]
 **page** | **int32** |  | [default to 1]
 **sort** | **string** | homes_for_you|newest|price_high_to_low|price_low_to_high|bedrooms|bathrooms|square_feet|lot_size|year_built | 
 **priceMin** | **int32** |  | 
 **priceMax** | **int32** |  | 
 **bedsMin** | **int32** |  | 
 **bathsMin** | **float32** |  | 
 **homeType** | **string** | houses|condos|townhomes|apartments|manufactured|lots|multi_family | 
 **sqftMin** | **int32** |  | 
 **sqftMax** | **int32** |  | 
 **lotMin** | **int32** |  | 
 **lotMax** | **int32** |  | 
 **yearBuiltMin** | **int32** |  | 
 **yearBuiltMax** | **int32** |  | 
 **hoaMax** | **int32** |  | 
 **keywords** | **string** |  | 
 **daysOn** | **string** |  | 
 **north** | **float32** | Map bounds for tiling past the 820 cap | 
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


## ZillowZillowScraperHealthCheck

> interface{} ZillowZillowScraperHealthCheck(ctx).Execute()

Zillow scraper health check



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
	resp, r, err := apiClient.ZillowAPI.ZillowZillowScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ZillowAPI.ZillowZillowScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ZillowZillowScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ZillowAPI.ZillowZillowScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiZillowZillowScraperHealthCheckRequest struct via the builder pattern


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


## ZillowZillowScraperHealthCheckHead

> interface{} ZillowZillowScraperHealthCheckHead(ctx).Execute()

Zillow scraper health check



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
	resp, r, err := apiClient.ZillowAPI.ZillowZillowScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ZillowAPI.ZillowZillowScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ZillowZillowScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ZillowAPI.ZillowZillowScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiZillowZillowScraperHealthCheckHeadRequest struct via the builder pattern


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


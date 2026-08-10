# \ImmobiliareAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ImmobiliareGetAgencyProfile**](ImmobiliareAPI.md#ImmobiliareGetAgencyProfile) | **Get** /v1/immobiliare/agencies/{agency_id} | Get agency profile
[**ImmobiliareGetAnAgencySListings**](ImmobiliareAPI.md#ImmobiliareGetAnAgencySListings) | **Get** /v1/immobiliare/agencies/{agency_id}/listings | Get an agency&#39;s listings
[**ImmobiliareGetListingDetail**](ImmobiliareAPI.md#ImmobiliareGetListingDetail) | **Get** /v1/immobiliare/listings/{listing_id} | Get listing detail
[**ImmobiliareImmobiliareScraperHealthCheck**](ImmobiliareAPI.md#ImmobiliareImmobiliareScraperHealthCheck) | **Get** /v1/immobiliare/health | Immobiliare scraper health check
[**ImmobiliareImmobiliareScraperHealthCheckHead**](ImmobiliareAPI.md#ImmobiliareImmobiliareScraperHealthCheckHead) | **Head** /v1/immobiliare/health | Immobiliare scraper health check
[**ImmobiliareListFilterEnums**](ImmobiliareAPI.md#ImmobiliareListFilterEnums) | **Get** /v1/immobiliare/reference | List filter enums
[**ImmobiliareListMarkets**](ImmobiliareAPI.md#ImmobiliareListMarkets) | **Get** /v1/immobiliare/markets | List markets
[**ImmobiliareLocationAutocomplete**](ImmobiliareAPI.md#ImmobiliareLocationAutocomplete) | **Get** /v1/immobiliare/autocomplete | Location autocomplete
[**ImmobiliarePriceMTimeSeries**](ImmobiliareAPI.md#ImmobiliarePriceMTimeSeries) | **Get** /v1/immobiliare/market-insights/prices | Price €/m² time series
[**ImmobiliareSearchListings**](ImmobiliareAPI.md#ImmobiliareSearchListings) | **Get** /v1/immobiliare/search | Search listings



## ImmobiliareGetAgencyProfile

> interface{} ImmobiliareGetAgencyProfile(ctx, agencyId).Market(market).Execute()

Get agency profile



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
	agencyId := int32(56) // int32 | 
	market := "market_example" // string | it | es | gr | lu (optional) (default to "it")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ImmobiliareAPI.ImmobiliareGetAgencyProfile(context.Background(), agencyId).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImmobiliareAPI.ImmobiliareGetAgencyProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ImmobiliareGetAgencyProfile`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ImmobiliareAPI.ImmobiliareGetAgencyProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**agencyId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiImmobiliareGetAgencyProfileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | it | es | gr | lu | [default to &quot;it&quot;]

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


## ImmobiliareGetAnAgencySListings

> interface{} ImmobiliareGetAnAgencySListings(ctx, agencyId).Market(market).Contract(contract).Page(page).Execute()

Get an agency's listings



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
	agencyId := int32(56) // int32 | 
	market := "market_example" // string | it | es | gr | lu (optional) (default to "it")
	contract := "contract_example" // string | sale | rent (optional) (default to "sale")
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ImmobiliareAPI.ImmobiliareGetAnAgencySListings(context.Background(), agencyId).Market(market).Contract(contract).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImmobiliareAPI.ImmobiliareGetAnAgencySListings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ImmobiliareGetAnAgencySListings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ImmobiliareAPI.ImmobiliareGetAnAgencySListings`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**agencyId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiImmobiliareGetAnAgencySListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | it | es | gr | lu | [default to &quot;it&quot;]
 **contract** | **string** | sale | rent | [default to &quot;sale&quot;]
 **page** | **int32** |  | [default to 1]

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


## ImmobiliareGetListingDetail

> interface{} ImmobiliareGetListingDetail(ctx, listingId).Market(market).Execute()

Get listing detail



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
	listingId := int32(56) // int32 | 
	market := "market_example" // string | it | es | gr | lu (optional) (default to "it")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ImmobiliareAPI.ImmobiliareGetListingDetail(context.Background(), listingId).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImmobiliareAPI.ImmobiliareGetListingDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ImmobiliareGetListingDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ImmobiliareAPI.ImmobiliareGetListingDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listingId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiImmobiliareGetListingDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **market** | **string** | it | es | gr | lu | [default to &quot;it&quot;]

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


## ImmobiliareImmobiliareScraperHealthCheck

> interface{} ImmobiliareImmobiliareScraperHealthCheck(ctx).Execute()

Immobiliare scraper health check



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
	resp, r, err := apiClient.ImmobiliareAPI.ImmobiliareImmobiliareScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImmobiliareAPI.ImmobiliareImmobiliareScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ImmobiliareImmobiliareScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ImmobiliareAPI.ImmobiliareImmobiliareScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiImmobiliareImmobiliareScraperHealthCheckRequest struct via the builder pattern


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


## ImmobiliareImmobiliareScraperHealthCheckHead

> interface{} ImmobiliareImmobiliareScraperHealthCheckHead(ctx).Execute()

Immobiliare scraper health check



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
	resp, r, err := apiClient.ImmobiliareAPI.ImmobiliareImmobiliareScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImmobiliareAPI.ImmobiliareImmobiliareScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ImmobiliareImmobiliareScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ImmobiliareAPI.ImmobiliareImmobiliareScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiImmobiliareImmobiliareScraperHealthCheckHeadRequest struct via the builder pattern


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


## ImmobiliareListFilterEnums

> interface{} ImmobiliareListFilterEnums(ctx).Execute()

List filter enums

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
	resp, r, err := apiClient.ImmobiliareAPI.ImmobiliareListFilterEnums(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImmobiliareAPI.ImmobiliareListFilterEnums``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ImmobiliareListFilterEnums`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ImmobiliareAPI.ImmobiliareListFilterEnums`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiImmobiliareListFilterEnumsRequest struct via the builder pattern


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


## ImmobiliareListMarkets

> interface{} ImmobiliareListMarkets(ctx).Execute()

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
	resp, r, err := apiClient.ImmobiliareAPI.ImmobiliareListMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImmobiliareAPI.ImmobiliareListMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ImmobiliareListMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ImmobiliareAPI.ImmobiliareListMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiImmobiliareListMarketsRequest struct via the builder pattern


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


## ImmobiliareLocationAutocomplete

> interface{} ImmobiliareLocationAutocomplete(ctx).Query(query).Market(market).Execute()

Location autocomplete



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
	query := "query_example" // string | Free-text place name, e.g. 'Milano'
	market := "market_example" // string | it | es | gr | lu (optional) (default to "it")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ImmobiliareAPI.ImmobiliareLocationAutocomplete(context.Background()).Query(query).Market(market).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImmobiliareAPI.ImmobiliareLocationAutocomplete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ImmobiliareLocationAutocomplete`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ImmobiliareAPI.ImmobiliareLocationAutocomplete`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiImmobiliareLocationAutocompleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Free-text place name, e.g. &#39;Milano&#39; | 
 **market** | **string** | it | es | gr | lu | [default to &quot;it&quot;]

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


## ImmobiliarePriceMTimeSeries

> interface{} ImmobiliarePriceMTimeSeries(ctx).RegionId(regionId).Market(market).ProvinceId(provinceId).CityId(cityId).Contract(contract).Execute()

Price €/m² time series



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
	regionId := "regionId_example" // string | Region id, e.g. 'lom'
	market := "market_example" // string | it | es | gr | lu (optional) (default to "it")
	provinceId := "provinceId_example" // string | Province id, e.g. 'MI' (optional)
	cityId := "cityId_example" // string | City id (idComune) (optional)
	contract := "contract_example" // string | sale | rent (optional) (default to "sale")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ImmobiliareAPI.ImmobiliarePriceMTimeSeries(context.Background()).RegionId(regionId).Market(market).ProvinceId(provinceId).CityId(cityId).Contract(contract).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImmobiliareAPI.ImmobiliarePriceMTimeSeries``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ImmobiliarePriceMTimeSeries`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ImmobiliareAPI.ImmobiliarePriceMTimeSeries`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiImmobiliarePriceMTimeSeriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **regionId** | **string** | Region id, e.g. &#39;lom&#39; | 
 **market** | **string** | it | es | gr | lu | [default to &quot;it&quot;]
 **provinceId** | **string** | Province id, e.g. &#39;MI&#39; | 
 **cityId** | **string** | City id (idComune) | 
 **contract** | **string** | sale | rent | [default to &quot;sale&quot;]

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


## ImmobiliareSearchListings

> interface{} ImmobiliareSearchListings(ctx).Market(market).Location(location).RegionId(regionId).ProvinceId(provinceId).CityId(cityId).Contract(contract).Category(category).PriceMin(priceMin).PriceMax(priceMax).SurfaceMin(surfaceMin).SurfaceMax(surfaceMax).RoomsMin(roomsMin).RoomsMax(roomsMax).BathroomsMin(bathroomsMin).Sort(sort).Page(page).Execute()

Search listings



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
	market := "market_example" // string | it | es | gr | lu (optional) (default to "it")
	location := "location_example" // string | Free-text place (auto-resolved) (optional)
	regionId := "regionId_example" // string | fkRegione (from /autocomplete) (optional)
	provinceId := "provinceId_example" // string | idProvincia (from /autocomplete) (optional)
	cityId := "cityId_example" // string | idComune (from /autocomplete) (optional)
	contract := "contract_example" // string | sale | rent (optional) (default to "sale")
	category := "category_example" // string | see /reference (optional) (default to "residential")
	priceMin := int32(56) // int32 |  (optional)
	priceMax := int32(56) // int32 |  (optional)
	surfaceMin := int32(56) // int32 |  (optional)
	surfaceMax := int32(56) // int32 |  (optional)
	roomsMin := int32(56) // int32 |  (optional)
	roomsMax := int32(56) // int32 |  (optional)
	bathroomsMin := int32(56) // int32 |  (optional)
	sort := "sort_example" // string | see /reference (optional) (default to "relevance")
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ImmobiliareAPI.ImmobiliareSearchListings(context.Background()).Market(market).Location(location).RegionId(regionId).ProvinceId(provinceId).CityId(cityId).Contract(contract).Category(category).PriceMin(priceMin).PriceMax(priceMax).SurfaceMin(surfaceMin).SurfaceMax(surfaceMax).RoomsMin(roomsMin).RoomsMax(roomsMax).BathroomsMin(bathroomsMin).Sort(sort).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImmobiliareAPI.ImmobiliareSearchListings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ImmobiliareSearchListings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ImmobiliareAPI.ImmobiliareSearchListings`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiImmobiliareSearchListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **market** | **string** | it | es | gr | lu | [default to &quot;it&quot;]
 **location** | **string** | Free-text place (auto-resolved) | 
 **regionId** | **string** | fkRegione (from /autocomplete) | 
 **provinceId** | **string** | idProvincia (from /autocomplete) | 
 **cityId** | **string** | idComune (from /autocomplete) | 
 **contract** | **string** | sale | rent | [default to &quot;sale&quot;]
 **category** | **string** | see /reference | [default to &quot;residential&quot;]
 **priceMin** | **int32** |  | 
 **priceMax** | **int32** |  | 
 **surfaceMin** | **int32** |  | 
 **surfaceMax** | **int32** |  | 
 **roomsMin** | **int32** |  | 
 **roomsMax** | **int32** |  | 
 **bathroomsMin** | **int32** |  | 
 **sort** | **string** | see /reference | [default to &quot;relevance&quot;]
 **page** | **int32** |  | [default to 1]

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


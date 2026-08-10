# \ApartmentsAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApartmentsApartmentsScraperHealthCheck**](ApartmentsAPI.md#ApartmentsApartmentsScraperHealthCheck) | **Get** /v1/apartments/health | Apartments scraper health check
[**ApartmentsApartmentsScraperHealthCheckHead**](ApartmentsAPI.md#ApartmentsApartmentsScraperHealthCheckHead) | **Head** /v1/apartments/health | Apartments scraper health check
[**ApartmentsGetPropertyDetailBySlugId**](ApartmentsAPI.md#ApartmentsGetPropertyDetailBySlugId) | **Get** /v1/apartments/properties/{slug}/{property_id} | Get property detail by slug + id
[**ApartmentsGetPropertyDetailByUrl**](ApartmentsAPI.md#ApartmentsGetPropertyDetailByUrl) | **Get** /v1/apartments/property | Get property detail by URL
[**ApartmentsSearchRentalListings**](ApartmentsAPI.md#ApartmentsSearchRentalListings) | **Get** /v1/apartments/search | Search rental listings



## ApartmentsApartmentsScraperHealthCheck

> interface{} ApartmentsApartmentsScraperHealthCheck(ctx).Execute()

Apartments scraper health check



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
	resp, r, err := apiClient.ApartmentsAPI.ApartmentsApartmentsScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApartmentsAPI.ApartmentsApartmentsScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApartmentsApartmentsScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ApartmentsAPI.ApartmentsApartmentsScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApartmentsApartmentsScraperHealthCheckRequest struct via the builder pattern


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


## ApartmentsApartmentsScraperHealthCheckHead

> interface{} ApartmentsApartmentsScraperHealthCheckHead(ctx).Execute()

Apartments scraper health check



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
	resp, r, err := apiClient.ApartmentsAPI.ApartmentsApartmentsScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApartmentsAPI.ApartmentsApartmentsScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApartmentsApartmentsScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ApartmentsAPI.ApartmentsApartmentsScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiApartmentsApartmentsScraperHealthCheckHeadRequest struct via the builder pattern


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


## ApartmentsGetPropertyDetailBySlugId

> interface{} ApartmentsGetPropertyDetailBySlugId(ctx, slug, propertyId).Execute()

Get property detail by slug + id



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
	slug := "slug_example" // string | 
	propertyId := "propertyId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApartmentsAPI.ApartmentsGetPropertyDetailBySlugId(context.Background(), slug, propertyId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApartmentsAPI.ApartmentsGetPropertyDetailBySlugId``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApartmentsGetPropertyDetailBySlugId`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ApartmentsAPI.ApartmentsGetPropertyDetailBySlugId`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** |  | 
**propertyId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiApartmentsGetPropertyDetailBySlugIdRequest struct via the builder pattern


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


## ApartmentsGetPropertyDetailByUrl

> interface{} ApartmentsGetPropertyDetailByUrl(ctx).Url(url).Execute()

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
	url := "url_example" // string | Full apartments.com property URL, e.g. https://www.apartments.com/urbane-kansas-city-mo/wcd6e5k/

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApartmentsAPI.ApartmentsGetPropertyDetailByUrl(context.Background()).Url(url).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApartmentsAPI.ApartmentsGetPropertyDetailByUrl``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApartmentsGetPropertyDetailByUrl`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ApartmentsAPI.ApartmentsGetPropertyDetailByUrl`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApartmentsGetPropertyDetailByUrlRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **url** | **string** | Full apartments.com property URL, e.g. https://www.apartments.com/urbane-kansas-city-mo/wcd6e5k/ | 

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


## ApartmentsSearchRentalListings

> interface{} ApartmentsSearchRentalListings(ctx).Location(location).Page(page).Beds(beds).MinPrice(minPrice).MaxPrice(maxPrice).Execute()

Search rental listings



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
	location := "location_example" // string | apartments.com location slug, e.g. 'kansas-city-mo'
	page := int32(56) // int32 |  (optional) (default to 1)
	beds := int32(56) // int32 | 0=studio, 1-4 bedrooms (optional)
	minPrice := int32(56) // int32 |  (optional)
	maxPrice := int32(56) // int32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApartmentsAPI.ApartmentsSearchRentalListings(context.Background()).Location(location).Page(page).Beds(beds).MinPrice(minPrice).MaxPrice(maxPrice).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApartmentsAPI.ApartmentsSearchRentalListings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApartmentsSearchRentalListings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ApartmentsAPI.ApartmentsSearchRentalListings`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApartmentsSearchRentalListingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **location** | **string** | apartments.com location slug, e.g. &#39;kansas-city-mo&#39; | 
 **page** | **int32** |  | [default to 1]
 **beds** | **int32** | 0&#x3D;studio, 1-4 bedrooms | 
 **minPrice** | **int32** |  | 
 **maxPrice** | **int32** |  | 

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


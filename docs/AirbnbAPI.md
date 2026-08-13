# \AirbnbAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AirbnbAirbnbScraperHealthCheck**](AirbnbAPI.md#AirbnbAirbnbScraperHealthCheck) | **Get** /v1/airbnb/health | Airbnb scraper health check
[**AirbnbAirbnbScraperHealthCheckHead**](AirbnbAPI.md#AirbnbAirbnbScraperHealthCheckHead) | **Head** /v1/airbnb/health | Airbnb scraper health check
[**AirbnbGetAvailabilityCalendar**](AirbnbAPI.md#AirbnbGetAvailabilityCalendar) | **Get** /v1/airbnb/listings/{room_id}/calendar | Get availability calendar
[**AirbnbGetExperienceDetail**](AirbnbAPI.md#AirbnbGetExperienceDetail) | **Get** /v1/airbnb/experiences/{experience_id} | Get experience detail
[**AirbnbGetListingDetail**](AirbnbAPI.md#AirbnbGetListingDetail) | **Get** /v1/airbnb/listings/{room_id} | Get listing detail
[**AirbnbGetListingReviews**](AirbnbAPI.md#AirbnbGetListingReviews) | **Get** /v1/airbnb/listings/{room_id}/reviews | Get listing reviews
[**AirbnbSearchExperiences**](AirbnbAPI.md#AirbnbSearchExperiences) | **Get** /v1/airbnb/experiences | Search experiences
[**AirbnbSearchStays**](AirbnbAPI.md#AirbnbSearchStays) | **Get** /v1/airbnb/search | Search stays



## AirbnbAirbnbScraperHealthCheck

> interface{} AirbnbAirbnbScraperHealthCheck(ctx).Execute()

Airbnb scraper health check



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
	resp, r, err := apiClient.AirbnbAPI.AirbnbAirbnbScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AirbnbAPI.AirbnbAirbnbScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AirbnbAirbnbScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AirbnbAPI.AirbnbAirbnbScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAirbnbAirbnbScraperHealthCheckRequest struct via the builder pattern


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


## AirbnbAirbnbScraperHealthCheckHead

> interface{} AirbnbAirbnbScraperHealthCheckHead(ctx).Execute()

Airbnb scraper health check



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
	resp, r, err := apiClient.AirbnbAPI.AirbnbAirbnbScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AirbnbAPI.AirbnbAirbnbScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AirbnbAirbnbScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AirbnbAPI.AirbnbAirbnbScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiAirbnbAirbnbScraperHealthCheckHeadRequest struct via the builder pattern


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


## AirbnbGetAvailabilityCalendar

> interface{} AirbnbGetAvailabilityCalendar(ctx, roomId).Month(month).Year(year).Months(months).Currency(currency).Locale(locale).Execute()

Get availability calendar



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
	roomId := "roomId_example" // string | 
	month := int32(56) // int32 | Start month (1-12) (optional) (default to 1)
	year := int32(56) // int32 | Start year (optional) (default to 2026)
	months := int32(56) // int32 | Number of months (max 12) (optional) (default to 12)
	currency := "currency_example" // string |  (optional)
	locale := "locale_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AirbnbAPI.AirbnbGetAvailabilityCalendar(context.Background(), roomId).Month(month).Year(year).Months(months).Currency(currency).Locale(locale).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AirbnbAPI.AirbnbGetAvailabilityCalendar``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AirbnbGetAvailabilityCalendar`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AirbnbAPI.AirbnbGetAvailabilityCalendar`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**roomId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAirbnbGetAvailabilityCalendarRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **month** | **int32** | Start month (1-12) | [default to 1]
 **year** | **int32** | Start year | [default to 2026]
 **months** | **int32** | Number of months (max 12) | [default to 12]
 **currency** | **string** |  | 
 **locale** | **string** |  | 

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


## AirbnbGetExperienceDetail

> interface{} AirbnbGetExperienceDetail(ctx, experienceId).Adults(adults).Children(children).Infants(infants).Currency(currency).Locale(locale).Execute()

Get experience detail



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
	experienceId := "experienceId_example" // string | 
	adults := int32(56) // int32 |  (optional) (default to 1)
	children := int32(56) // int32 |  (optional) (default to 0)
	infants := int32(56) // int32 |  (optional) (default to 0)
	currency := "currency_example" // string |  (optional)
	locale := "locale_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AirbnbAPI.AirbnbGetExperienceDetail(context.Background(), experienceId).Adults(adults).Children(children).Infants(infants).Currency(currency).Locale(locale).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AirbnbAPI.AirbnbGetExperienceDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AirbnbGetExperienceDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AirbnbAPI.AirbnbGetExperienceDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**experienceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAirbnbGetExperienceDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **adults** | **int32** |  | [default to 1]
 **children** | **int32** |  | [default to 0]
 **infants** | **int32** |  | [default to 0]
 **currency** | **string** |  | 
 **locale** | **string** |  | 

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


## AirbnbGetListingDetail

> interface{} AirbnbGetListingDetail(ctx, roomId).Adults(adults).Currency(currency).Locale(locale).Execute()

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
	roomId := "roomId_example" // string | 
	adults := int32(56) // int32 |  (optional) (default to 1)
	currency := "currency_example" // string |  (optional)
	locale := "locale_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AirbnbAPI.AirbnbGetListingDetail(context.Background(), roomId).Adults(adults).Currency(currency).Locale(locale).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AirbnbAPI.AirbnbGetListingDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AirbnbGetListingDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AirbnbAPI.AirbnbGetListingDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**roomId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAirbnbGetListingDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **adults** | **int32** |  | [default to 1]
 **currency** | **string** |  | 
 **locale** | **string** |  | 

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


## AirbnbGetListingReviews

> interface{} AirbnbGetListingReviews(ctx, roomId).Limit(limit).Offset(offset).Sort(sort).Currency(currency).Locale(locale).Execute()

Get listing reviews



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
	roomId := "roomId_example" // string | 
	limit := int32(56) // int32 |  (optional) (default to 24)
	offset := int32(56) // int32 |  (optional) (default to 0)
	sort := "sort_example" // string | MOST_RECENT | RATING_DESC | RATING_ASC (optional) (default to "MOST_RECENT")
	currency := "currency_example" // string |  (optional)
	locale := "locale_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AirbnbAPI.AirbnbGetListingReviews(context.Background(), roomId).Limit(limit).Offset(offset).Sort(sort).Currency(currency).Locale(locale).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AirbnbAPI.AirbnbGetListingReviews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AirbnbGetListingReviews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AirbnbAPI.AirbnbGetListingReviews`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**roomId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAirbnbGetListingReviewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int32** |  | [default to 24]
 **offset** | **int32** |  | [default to 0]
 **sort** | **string** | MOST_RECENT | RATING_DESC | RATING_ASC | [default to &quot;MOST_RECENT&quot;]
 **currency** | **string** |  | 
 **locale** | **string** |  | 

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


## AirbnbSearchExperiences

> interface{} AirbnbSearchExperiences(ctx).Location(location).Cursor(cursor).Currency(currency).Locale(locale).Execute()

Search experiences



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
	location := "location_example" // string | Free-text place, e.g. 'Rome, Italy'
	cursor := "cursor_example" // string | next_page_cursor from a prior response (optional)
	currency := "currency_example" // string |  (optional)
	locale := "locale_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AirbnbAPI.AirbnbSearchExperiences(context.Background()).Location(location).Cursor(cursor).Currency(currency).Locale(locale).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AirbnbAPI.AirbnbSearchExperiences``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AirbnbSearchExperiences`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AirbnbAPI.AirbnbSearchExperiences`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAirbnbSearchExperiencesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **location** | **string** | Free-text place, e.g. &#39;Rome, Italy&#39; | 
 **cursor** | **string** | next_page_cursor from a prior response | 
 **currency** | **string** |  | 
 **locale** | **string** |  | 

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


## AirbnbSearchStays

> interface{} AirbnbSearchStays(ctx).Location(location).NeLat(neLat).NeLng(neLng).SwLat(swLat).SwLng(swLng).CheckIn(checkIn).CheckOut(checkOut).Adults(adults).Children(children).Infants(infants).Pets(pets).PriceMin(priceMin).PriceMax(priceMax).MinBedrooms(minBedrooms).MinBeds(minBeds).MinBathrooms(minBathrooms).RoomType(roomType).Cursor(cursor).Limit(limit).Currency(currency).Locale(locale).Execute()

Search stays



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
	location := "location_example" // string | Free-text place, e.g. 'Paris, France' (optional)
	neLat := float32(8.14) // float32 | Map bounding-box NE latitude (optional)
	neLng := float32(8.14) // float32 | Map bounding-box NE longitude (optional)
	swLat := float32(8.14) // float32 | Map bounding-box SW latitude (optional)
	swLng := float32(8.14) // float32 | Map bounding-box SW longitude (optional)
	checkIn := "checkIn_example" // string | Check-in date YYYY-MM-DD (optional)
	checkOut := "checkOut_example" // string | Check-out date YYYY-MM-DD (optional)
	adults := int32(56) // int32 |  (optional) (default to 1)
	children := int32(56) // int32 |  (optional) (default to 0)
	infants := int32(56) // int32 |  (optional) (default to 0)
	pets := int32(56) // int32 |  (optional) (default to 0)
	priceMin := int32(56) // int32 |  (optional)
	priceMax := int32(56) // int32 |  (optional)
	minBedrooms := int32(56) // int32 |  (optional)
	minBeds := int32(56) // int32 |  (optional)
	minBathrooms := int32(56) // int32 |  (optional)
	roomType := "roomType_example" // string | e.g. 'Entire home/apt', 'Private room' (optional)
	cursor := "cursor_example" // string | next_page_cursor from a prior response (optional)
	limit := int32(56) // int32 |  (optional) (default to 18)
	currency := "currency_example" // string | ISO currency, e.g. USD, EUR (optional)
	locale := "locale_example" // string | Locale, e.g. en, fr (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AirbnbAPI.AirbnbSearchStays(context.Background()).Location(location).NeLat(neLat).NeLng(neLng).SwLat(swLat).SwLng(swLng).CheckIn(checkIn).CheckOut(checkOut).Adults(adults).Children(children).Infants(infants).Pets(pets).PriceMin(priceMin).PriceMax(priceMax).MinBedrooms(minBedrooms).MinBeds(minBeds).MinBathrooms(minBathrooms).RoomType(roomType).Cursor(cursor).Limit(limit).Currency(currency).Locale(locale).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AirbnbAPI.AirbnbSearchStays``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AirbnbSearchStays`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AirbnbAPI.AirbnbSearchStays`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAirbnbSearchStaysRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **location** | **string** | Free-text place, e.g. &#39;Paris, France&#39; | 
 **neLat** | **float32** | Map bounding-box NE latitude | 
 **neLng** | **float32** | Map bounding-box NE longitude | 
 **swLat** | **float32** | Map bounding-box SW latitude | 
 **swLng** | **float32** | Map bounding-box SW longitude | 
 **checkIn** | **string** | Check-in date YYYY-MM-DD | 
 **checkOut** | **string** | Check-out date YYYY-MM-DD | 
 **adults** | **int32** |  | [default to 1]
 **children** | **int32** |  | [default to 0]
 **infants** | **int32** |  | [default to 0]
 **pets** | **int32** |  | [default to 0]
 **priceMin** | **int32** |  | 
 **priceMax** | **int32** |  | 
 **minBedrooms** | **int32** |  | 
 **minBeds** | **int32** |  | 
 **minBathrooms** | **int32** |  | 
 **roomType** | **string** | e.g. &#39;Entire home/apt&#39;, &#39;Private room&#39; | 
 **cursor** | **string** | next_page_cursor from a prior response | 
 **limit** | **int32** |  | [default to 18]
 **currency** | **string** | ISO currency, e.g. USD, EUR | 
 **locale** | **string** | Locale, e.g. en, fr | 

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


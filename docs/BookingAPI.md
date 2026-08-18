# \BookingAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**BookingBookingScraperHealthCheck**](BookingAPI.md#BookingBookingScraperHealthCheck) | **Get** /v1/booking/health | Booking scraper health check
[**BookingBookingScraperHealthCheckHead**](BookingAPI.md#BookingBookingScraperHealthCheckHead) | **Head** /v1/booking/health | Booking scraper health check
[**BookingGetPropertyDetail**](BookingAPI.md#BookingGetPropertyDetail) | **Get** /v1/booking/properties/{country_code}/{slug} | Get property detail
[**BookingGetPropertyReviews**](BookingAPI.md#BookingGetPropertyReviews) | **Get** /v1/booking/properties/{country_code}/{slug}/reviews | Get property reviews
[**BookingGetRoomTypesAndLiveRates**](BookingAPI.md#BookingGetRoomTypesAndLiveRates) | **Get** /v1/booking/properties/{country_code}/{slug}/rooms | Get room types and live rates
[**BookingSearchDestinations**](BookingAPI.md#BookingSearchDestinations) | **Get** /v1/booking/destinations | Search destinations
[**BookingSearchProperties**](BookingAPI.md#BookingSearchProperties) | **Get** /v1/booking/search | Search properties



## BookingBookingScraperHealthCheck

> interface{} BookingBookingScraperHealthCheck(ctx).Execute()

Booking scraper health check



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
	resp, r, err := apiClient.BookingAPI.BookingBookingScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BookingAPI.BookingBookingScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BookingBookingScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BookingAPI.BookingBookingScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiBookingBookingScraperHealthCheckRequest struct via the builder pattern


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


## BookingBookingScraperHealthCheckHead

> interface{} BookingBookingScraperHealthCheckHead(ctx).Execute()

Booking scraper health check



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
	resp, r, err := apiClient.BookingAPI.BookingBookingScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BookingAPI.BookingBookingScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BookingBookingScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BookingAPI.BookingBookingScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiBookingBookingScraperHealthCheckHeadRequest struct via the builder pattern


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


## BookingGetPropertyDetail

> interface{} BookingGetPropertyDetail(ctx, countryCode, slug).Photos(photos).Questions(questions).Language(language).Execute()

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
	countryCode := "countryCode_example" // string | Two-letter country code, e.g. 'it'
	slug := "slug_example" // string | Booking page name, e.g. 'hotel-artemide'
	photos := int32(56) // int32 | Gallery photos to return (optional) (default to 40)
	questions := int32(56) // int32 | Guest Q&A pairs to return (optional) (default to 10)
	language := "language_example" // string | Locale, e.g. en-us, fr (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BookingAPI.BookingGetPropertyDetail(context.Background(), countryCode, slug).Photos(photos).Questions(questions).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BookingAPI.BookingGetPropertyDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BookingGetPropertyDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BookingAPI.BookingGetPropertyDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**countryCode** | **string** | Two-letter country code, e.g. &#39;it&#39; | 
**slug** | **string** | Booking page name, e.g. &#39;hotel-artemide&#39; | 

### Other Parameters

Other parameters are passed through a pointer to a apiBookingGetPropertyDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **photos** | **int32** | Gallery photos to return | [default to 40]
 **questions** | **int32** | Guest Q&amp;A pairs to return | [default to 10]
 **language** | **string** | Locale, e.g. en-us, fr | 

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


## BookingGetPropertyReviews

> interface{} BookingGetPropertyReviews(ctx, countryCode, slug).Limit(limit).Offset(offset).Sort(sort).ReviewLanguage(reviewLanguage).GuestType(guestType).Language(language).Execute()

Get property reviews



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
	countryCode := "countryCode_example" // string | Two-letter country code, e.g. 'it'
	slug := "slug_example" // string | Booking page name, e.g. 'hotel-artemide'
	limit := int32(56) // int32 |  (optional) (default to 25)
	offset := int32(56) // int32 |  (optional) (default to 0)
	sort := "sort_example" // string | MOST_RELEVANT | NEWEST_FIRST | OLDEST_FIRST | SCORE_DESC | SCORE_ASC (optional) (default to "MOST_RELEVANT")
	reviewLanguage := "reviewLanguage_example" // string | Only reviews written in this language, e.g. 'fr' (optional)
	guestType := "guestType_example" // string | FAMILIES | COUPLES | GROUP_OF_FRIENDS | SOLO_TRAVELLERS | BUSINESS_TRAVELLERS (optional)
	language := "language_example" // string | Locale for labels, e.g. en-us (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BookingAPI.BookingGetPropertyReviews(context.Background(), countryCode, slug).Limit(limit).Offset(offset).Sort(sort).ReviewLanguage(reviewLanguage).GuestType(guestType).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BookingAPI.BookingGetPropertyReviews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BookingGetPropertyReviews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BookingAPI.BookingGetPropertyReviews`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**countryCode** | **string** | Two-letter country code, e.g. &#39;it&#39; | 
**slug** | **string** | Booking page name, e.g. &#39;hotel-artemide&#39; | 

### Other Parameters

Other parameters are passed through a pointer to a apiBookingGetPropertyReviewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **limit** | **int32** |  | [default to 25]
 **offset** | **int32** |  | [default to 0]
 **sort** | **string** | MOST_RELEVANT | NEWEST_FIRST | OLDEST_FIRST | SCORE_DESC | SCORE_ASC | [default to &quot;MOST_RELEVANT&quot;]
 **reviewLanguage** | **string** | Only reviews written in this language, e.g. &#39;fr&#39; | 
 **guestType** | **string** | FAMILIES | COUPLES | GROUP_OF_FRIENDS | SOLO_TRAVELLERS | BUSINESS_TRAVELLERS | 
 **language** | **string** | Locale for labels, e.g. en-us | 

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


## BookingGetRoomTypesAndLiveRates

> interface{} BookingGetRoomTypesAndLiveRates(ctx, countryCode, slug).Checkin(checkin).Checkout(checkout).Adults(adults).Children(children).Rooms(rooms).Currency(currency).Language(language).Execute()

Get room types and live rates



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
	countryCode := "countryCode_example" // string | Two-letter country code, e.g. 'it'
	slug := "slug_example" // string | Booking page name, e.g. 'hotel-artemide'
	checkin := "checkin_example" // string | Check-in date YYYY-MM-DD
	checkout := "checkout_example" // string | Check-out date YYYY-MM-DD
	adults := int32(56) // int32 |  (optional) (default to 2)
	children := "children_example" // string | Comma-separated children ages, e.g. '4,9' (optional)
	rooms := int32(56) // int32 |  (optional) (default to 1)
	currency := "currency_example" // string | ISO currency, e.g. EUR, USD, GBP (optional)
	language := "language_example" // string | Locale, e.g. en-us, fr, de (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BookingAPI.BookingGetRoomTypesAndLiveRates(context.Background(), countryCode, slug).Checkin(checkin).Checkout(checkout).Adults(adults).Children(children).Rooms(rooms).Currency(currency).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BookingAPI.BookingGetRoomTypesAndLiveRates``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BookingGetRoomTypesAndLiveRates`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BookingAPI.BookingGetRoomTypesAndLiveRates`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**countryCode** | **string** | Two-letter country code, e.g. &#39;it&#39; | 
**slug** | **string** | Booking page name, e.g. &#39;hotel-artemide&#39; | 

### Other Parameters

Other parameters are passed through a pointer to a apiBookingGetRoomTypesAndLiveRatesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **checkin** | **string** | Check-in date YYYY-MM-DD | 
 **checkout** | **string** | Check-out date YYYY-MM-DD | 
 **adults** | **int32** |  | [default to 2]
 **children** | **string** | Comma-separated children ages, e.g. &#39;4,9&#39; | 
 **rooms** | **int32** |  | [default to 1]
 **currency** | **string** | ISO currency, e.g. EUR, USD, GBP | 
 **language** | **string** | Locale, e.g. en-us, fr, de | 

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


## BookingSearchDestinations

> interface{} BookingSearchDestinations(ctx).Query(query).Limit(limit).Language(language).Execute()

Search destinations



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
	query := "query_example" // string | Free-text place, e.g. 'amsterd'
	limit := int32(56) // int32 |  (optional) (default to 8)
	language := "language_example" // string | Locale, e.g. en-us, fr (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BookingAPI.BookingSearchDestinations(context.Background()).Query(query).Limit(limit).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BookingAPI.BookingSearchDestinations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BookingSearchDestinations`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BookingAPI.BookingSearchDestinations`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBookingSearchDestinationsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Free-text place, e.g. &#39;amsterd&#39; | 
 **limit** | **int32** |  | [default to 8]
 **language** | **string** | Locale, e.g. en-us, fr | 

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


## BookingSearchProperties

> interface{} BookingSearchProperties(ctx).Location(location).DestId(destId).DestType(destType).Checkin(checkin).Checkout(checkout).Adults(adults).Children(children).Rooms(rooms).Offset(offset).Limit(limit).Sort(sort).Filters(filters).Currency(currency).Language(language).Execute()

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
	location := "location_example" // string | Free-text destination, e.g. 'Rome' (optional)
	destId := int32(56) // int32 | Exact destination id (ufi) from /destinations (optional)
	destType := "destType_example" // string | Destination type, e.g. CITY (optional) (default to "NO_DEST_TYPE")
	checkin := "checkin_example" // string | Check-in date YYYY-MM-DD (optional)
	checkout := "checkout_example" // string | Check-out date YYYY-MM-DD (optional)
	adults := int32(56) // int32 |  (optional) (default to 2)
	children := "children_example" // string | Comma-separated children ages, e.g. '4,9' (optional)
	rooms := int32(56) // int32 |  (optional) (default to 1)
	offset := int32(56) // int32 | Result offset for pagination (optional) (default to 0)
	limit := int32(56) // int32 |  (optional) (default to 25)
	sort := "sort_example" // string | popularity | price | class_descending | class_ascending | distance_from_search | bayesian_review_score | review_score_and_price | upsort_bh (optional)
	filters := "filters_example" // string | Semicolon-separated Booking filter ids, e.g. 'class=4' (optional)
	currency := "currency_example" // string | ISO currency, e.g. EUR, USD, GBP (optional)
	language := "language_example" // string | Locale, e.g. en-us, fr, de, es (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BookingAPI.BookingSearchProperties(context.Background()).Location(location).DestId(destId).DestType(destType).Checkin(checkin).Checkout(checkout).Adults(adults).Children(children).Rooms(rooms).Offset(offset).Limit(limit).Sort(sort).Filters(filters).Currency(currency).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BookingAPI.BookingSearchProperties``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BookingSearchProperties`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `BookingAPI.BookingSearchProperties`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBookingSearchPropertiesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **location** | **string** | Free-text destination, e.g. &#39;Rome&#39; | 
 **destId** | **int32** | Exact destination id (ufi) from /destinations | 
 **destType** | **string** | Destination type, e.g. CITY | [default to &quot;NO_DEST_TYPE&quot;]
 **checkin** | **string** | Check-in date YYYY-MM-DD | 
 **checkout** | **string** | Check-out date YYYY-MM-DD | 
 **adults** | **int32** |  | [default to 2]
 **children** | **string** | Comma-separated children ages, e.g. &#39;4,9&#39; | 
 **rooms** | **int32** |  | [default to 1]
 **offset** | **int32** | Result offset for pagination | [default to 0]
 **limit** | **int32** |  | [default to 25]
 **sort** | **string** | popularity | price | class_descending | class_ascending | distance_from_search | bayesian_review_score | review_score_and_price | upsort_bh | 
 **filters** | **string** | Semicolon-separated Booking filter ids, e.g. &#39;class&#x3D;4&#39; | 
 **currency** | **string** | ISO currency, e.g. EUR, USD, GBP | 
 **language** | **string** | Locale, e.g. en-us, fr, de, es | 

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


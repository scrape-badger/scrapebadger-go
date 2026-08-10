# \GoogleAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GoogleGetAuthorCitationsPerYearChart**](GoogleAPI.md#GoogleGetAuthorCitationsPerYearChart) | **Get** /v1/google/scholar/author/citation | Get author citations-per-year chart
[**GoogleGetBusinessPosts**](GoogleAPI.md#GoogleGetBusinessPosts) | **Get** /v1/google/maps/posts | Get business posts
[**GoogleGetCitationFormatsForAScholarPaper**](GoogleAPI.md#GoogleGetCitationFormatsForAScholarPaper) | **Get** /v1/google/scholar/cite | Get citation formats for a Scholar paper
[**GoogleGetPlaceDetails**](GoogleAPI.md#GoogleGetPlaceDetails) | **Get** /v1/google/maps/place | Get place details
[**GoogleGetPlacePhotos**](GoogleAPI.md#GoogleGetPlacePhotos) | **Get** /v1/google/maps/photos | Get place photos
[**GoogleGetPlaceReviews**](GoogleAPI.md#GoogleGetPlaceReviews) | **Get** /v1/google/maps/reviews | Get place reviews
[**GoogleGetScholarAuthorProfile**](GoogleAPI.md#GoogleGetScholarAuthorProfile) | **Get** /v1/google/scholar/author | Get Scholar author profile
[**GoogleGetStockIndexQuote**](GoogleAPI.md#GoogleGetStockIndexQuote) | **Get** /v1/google/finance/quote | Get stock/index quote
[**GoogleGoogleAiModeSearch**](GoogleAPI.md#GoogleGoogleAiModeSearch) | **Get** /v1/google/ai-mode/search | Google AI Mode search
[**GoogleGoogleAiOverviewInlineSerpBlock**](GoogleAPI.md#GoogleGoogleAiOverviewInlineSerpBlock) | **Get** /v1/google/ai-overview | Google AI Overview (inline SERP block)
[**GoogleGoogleFlightsCalendarCheapestFarePerDate**](GoogleAPI.md#GoogleGoogleFlightsCalendarCheapestFarePerDate) | **Get** /v1/google/flights/calendar | Google Flights calendar — cheapest fare per date
[**GoogleGoogleFlightsSearch**](GoogleAPI.md#GoogleGoogleFlightsSearch) | **Get** /v1/google/flights/search | Google Flights search
[**GoogleGoogleLensVisualSearch**](GoogleAPI.md#GoogleGoogleLensVisualSearch) | **Get** /v1/google/lens/search | Google Lens visual search
[**GoogleGoogleScraperHealthCheck**](GoogleAPI.md#GoogleGoogleScraperHealthCheck) | **Get** /v1/google/health | Google scraper health check
[**GoogleGoogleScraperHealthCheckHead**](GoogleAPI.md#GoogleGoogleScraperHealthCheckHead) | **Head** /v1/google/health | Google scraper health check
[**GoogleGoogleSearchSuggestions**](GoogleAPI.md#GoogleGoogleSearchSuggestions) | **Get** /v1/google/autocomplete | Google search suggestions
[**GoogleGoogleShortsSearch**](GoogleAPI.md#GoogleGoogleShortsSearch) | **Get** /v1/google/shorts/search | Google Shorts search
[**GoogleGoogleWebSearch**](GoogleAPI.md#GoogleGoogleWebSearch) | **Get** /v1/google/search | Google web search
[**GoogleHotelDetails**](GoogleAPI.md#GoogleHotelDetails) | **Get** /v1/google/hotels/details | Hotel details
[**GoogleImmersiveProductDetail**](GoogleAPI.md#GoogleImmersiveProductDetail) | **Get** /v1/google/products/detail | Immersive product detail
[**GoogleInterestByRegion**](GoogleAPI.md#GoogleInterestByRegion) | **Get** /v1/google/trends/regions | Interest by region
[**GoogleInterestOverTime**](GoogleAPI.md#GoogleInterestOverTime) | **Get** /v1/google/trends/interest | Interest over time
[**GoogleMultiSellerOffersByBarcode**](GoogleAPI.md#GoogleMultiSellerOffersByBarcode) | **Get** /v1/google/shopping/offers | Multi-seller offers by barcode
[**GoogleNewsByTopic**](GoogleAPI.md#GoogleNewsByTopic) | **Get** /v1/google/news/topics | News by topic
[**GooglePatentDetails**](GoogleAPI.md#GooglePatentDetails) | **Get** /v1/google/patents/detail | Patent details
[**GoogleRelatedTopicsQueries**](GoogleAPI.md#GoogleRelatedTopicsQueries) | **Get** /v1/google/trends/related | Related topics &amp; queries
[**GoogleSearchGoogleImages**](GoogleAPI.md#GoogleSearchGoogleImages) | **Get** /v1/google/images/search | Search Google Images
[**GoogleSearchGoogleJobs**](GoogleAPI.md#GoogleSearchGoogleJobs) | **Get** /v1/google/jobs/search | Search Google Jobs
[**GoogleSearchGoogleMapsPlaces**](GoogleAPI.md#GoogleSearchGoogleMapsPlaces) | **Get** /v1/google/maps/search | Search Google Maps places
[**GoogleSearchGoogleNews**](GoogleAPI.md#GoogleSearchGoogleNews) | **Get** /v1/google/news/search | Search Google News
[**GoogleSearchGoogleScholar**](GoogleAPI.md#GoogleSearchGoogleScholar) | **Get** /v1/google/scholar/search | Search Google Scholar
[**GoogleSearchGoogleVideos**](GoogleAPI.md#GoogleSearchGoogleVideos) | **Get** /v1/google/videos/search | Search Google Videos
[**GoogleSearchHotels**](GoogleAPI.md#GoogleSearchHotels) | **Get** /v1/google/hotels/search | Search hotels
[**GoogleSearchPatents**](GoogleAPI.md#GoogleSearchPatents) | **Get** /v1/google/patents/search | Search patents
[**GoogleSearchProducts**](GoogleAPI.md#GoogleSearchProducts) | **Get** /v1/google/shopping/search | Search products
[**GoogleSearchScholarAuthorProfiles**](GoogleAPI.md#GoogleSearchScholarAuthorProfiles) | **Get** /v1/google/scholar/profiles | Search Scholar author profiles
[**GoogleTrendingNews**](GoogleAPI.md#GoogleTrendingNews) | **Get** /v1/google/news/trending | Trending news
[**GoogleTrendingSearches**](GoogleAPI.md#GoogleTrendingSearches) | **Get** /v1/google/trends/trending | Trending searches
[**GoogleTrendsTopicAutocomplete**](GoogleAPI.md#GoogleTrendsTopicAutocomplete) | **Get** /v1/google/trends/autocomplete | Trends topic autocomplete



## GoogleGetAuthorCitationsPerYearChart

> interface{} GoogleGetAuthorCitationsPerYearChart(ctx).AuthorId(authorId).Hl(hl).Execute()

Get author citations-per-year chart



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
	authorId := "authorId_example" // string | Scholar user ID
	hl := "hl_example" // string | Language code (optional) (default to "en")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleGetAuthorCitationsPerYearChart(context.Background()).AuthorId(authorId).Hl(hl).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGetAuthorCitationsPerYearChart``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGetAuthorCitationsPerYearChart`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGetAuthorCitationsPerYearChart`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGetAuthorCitationsPerYearChartRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorId** | **string** | Scholar user ID | 
 **hl** | **string** | Language code | [default to &quot;en&quot;]

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


## GoogleGetBusinessPosts

> interface{} GoogleGetBusinessPosts(ctx).DataId(dataId).NextPageToken(nextPageToken).Execute()

Get business posts

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
	dataId := "dataId_example" // string | Maps data ID
	nextPageToken := "nextPageToken_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleGetBusinessPosts(context.Background()).DataId(dataId).NextPageToken(nextPageToken).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGetBusinessPosts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGetBusinessPosts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGetBusinessPosts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGetBusinessPostsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dataId** | **string** | Maps data ID | 
 **nextPageToken** | **string** |  | 

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


## GoogleGetCitationFormatsForAScholarPaper

> interface{} GoogleGetCitationFormatsForAScholarPaper(ctx).Q(q).Hl(hl).Execute()

Get citation formats for a Scholar paper



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
	q := "q_example" // string | Cluster ID from a search result
	hl := "hl_example" // string | Language code (optional) (default to "en")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleGetCitationFormatsForAScholarPaper(context.Background()).Q(q).Hl(hl).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGetCitationFormatsForAScholarPaper``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGetCitationFormatsForAScholarPaper`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGetCitationFormatsForAScholarPaper`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGetCitationFormatsForAScholarPaperRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Cluster ID from a search result | 
 **hl** | **string** | Language code | [default to &quot;en&quot;]

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


## GoogleGetPlaceDetails

> interface{} GoogleGetPlaceDetails(ctx).PlaceId(placeId).DataId(dataId).Hl(hl).Gl(gl).Execute()

Get place details

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
	placeId := "placeId_example" // string |  (optional)
	dataId := "dataId_example" // string |  (optional)
	hl := "hl_example" // string |  (optional) (default to "en")
	gl := "gl_example" // string |  (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleGetPlaceDetails(context.Background()).PlaceId(placeId).DataId(dataId).Hl(hl).Gl(gl).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGetPlaceDetails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGetPlaceDetails`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGetPlaceDetails`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGetPlaceDetailsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **placeId** | **string** |  | 
 **dataId** | **string** |  | 
 **hl** | **string** |  | [default to &quot;en&quot;]
 **gl** | **string** |  | [default to &quot;us&quot;]

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


## GoogleGetPlacePhotos

> interface{} GoogleGetPlacePhotos(ctx).DataId(dataId).Hl(hl).NextPageToken(nextPageToken).Execute()

Get place photos

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
	dataId := "dataId_example" // string | Maps data ID
	hl := "hl_example" // string |  (optional) (default to "en")
	nextPageToken := "nextPageToken_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleGetPlacePhotos(context.Background()).DataId(dataId).Hl(hl).NextPageToken(nextPageToken).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGetPlacePhotos``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGetPlacePhotos`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGetPlacePhotos`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGetPlacePhotosRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dataId** | **string** | Maps data ID | 
 **hl** | **string** |  | [default to &quot;en&quot;]
 **nextPageToken** | **string** |  | 

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


## GoogleGetPlaceReviews

> interface{} GoogleGetPlaceReviews(ctx).DataId(dataId).SortBy(sortBy).Hl(hl).NextPageToken(nextPageToken).Results(results).Execute()

Get place reviews

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
	dataId := "dataId_example" // string | Maps data ID
	sortBy := "sortBy_example" // string |  (optional) (default to "qualityScore")
	hl := "hl_example" // string |  (optional) (default to "en")
	nextPageToken := "nextPageToken_example" // string |  (optional)
	results := int32(56) // int32 |  (optional) (default to 10)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleGetPlaceReviews(context.Background()).DataId(dataId).SortBy(sortBy).Hl(hl).NextPageToken(nextPageToken).Results(results).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGetPlaceReviews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGetPlaceReviews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGetPlaceReviews`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGetPlaceReviewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dataId** | **string** | Maps data ID | 
 **sortBy** | **string** |  | [default to &quot;qualityScore&quot;]
 **hl** | **string** |  | [default to &quot;en&quot;]
 **nextPageToken** | **string** |  | 
 **results** | **int32** |  | [default to 10]

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


## GoogleGetScholarAuthorProfile

> interface{} GoogleGetScholarAuthorProfile(ctx).AuthorId(authorId).Hl(hl).Cstart(cstart).Pagesize(pagesize).Execute()

Get Scholar author profile



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
	authorId := "authorId_example" // string | Scholar user ID (the `user` query parameter)
	hl := "hl_example" // string | Language code (optional) (default to "en")
	cstart := int32(56) // int32 | Articles pagination offset (optional) (default to 0)
	pagesize := int32(56) // int32 | Articles per page (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleGetScholarAuthorProfile(context.Background()).AuthorId(authorId).Hl(hl).Cstart(cstart).Pagesize(pagesize).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGetScholarAuthorProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGetScholarAuthorProfile`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGetScholarAuthorProfile`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGetScholarAuthorProfileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorId** | **string** | Scholar user ID (the &#x60;user&#x60; query parameter) | 
 **hl** | **string** | Language code | [default to &quot;en&quot;]
 **cstart** | **int32** | Articles pagination offset | [default to 0]
 **pagesize** | **int32** | Articles per page | [default to 20]

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


## GoogleGetStockIndexQuote

> interface{} GoogleGetStockIndexQuote(ctx).Q(q).Hl(hl).Execute()

Get stock/index quote



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
	q := "q_example" // string | Ticker and exchange (e.g. \"AAPL:NASDAQ\", \"BTC-USD\")
	hl := "hl_example" // string | Language code (optional) (default to "en")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleGetStockIndexQuote(context.Background()).Q(q).Hl(hl).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGetStockIndexQuote``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGetStockIndexQuote`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGetStockIndexQuote`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGetStockIndexQuoteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Ticker and exchange (e.g. \&quot;AAPL:NASDAQ\&quot;, \&quot;BTC-USD\&quot;) | 
 **hl** | **string** | Language code | [default to &quot;en&quot;]

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


## GoogleGoogleAiModeSearch

> interface{} GoogleGoogleAiModeSearch(ctx).Q(q).Gl(gl).Hl(hl).IncludeHtml(includeHtml).Execute()

Google AI Mode search



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
	q := "q_example" // string | Search query for AI-generated response
	gl := "gl_example" // string | Country code (optional) (default to "us")
	hl := "hl_example" // string | Language code (optional) (default to "en")
	includeHtml := true // bool | Include the raw `answer_html` (full answer body HTML) in the response for maximum parity. It can be 100s of KB — set false when you only need the structured `text_blocks` + `markdown`. (optional) (default to true)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleGoogleAiModeSearch(context.Background()).Q(q).Gl(gl).Hl(hl).IncludeHtml(includeHtml).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGoogleAiModeSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGoogleAiModeSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGoogleAiModeSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGoogleAiModeSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search query for AI-generated response | 
 **gl** | **string** | Country code | [default to &quot;us&quot;]
 **hl** | **string** | Language code | [default to &quot;en&quot;]
 **includeHtml** | **bool** | Include the raw &#x60;answer_html&#x60; (full answer body HTML) in the response for maximum parity. It can be 100s of KB — set false when you only need the structured &#x60;text_blocks&#x60; + &#x60;markdown&#x60;. | [default to true]

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


## GoogleGoogleAiOverviewInlineSerpBlock

> interface{} GoogleGoogleAiOverviewInlineSerpBlock(ctx).Q(q).Gl(gl).Hl(hl).Execute()

Google AI Overview (inline SERP block)



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
	q := "q_example" // string | Search query — same shape as a Google Search query
	gl := "gl_example" // string | Country code (optional) (default to "us")
	hl := "hl_example" // string | Language code (optional) (default to "en")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleGoogleAiOverviewInlineSerpBlock(context.Background()).Q(q).Gl(gl).Hl(hl).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGoogleAiOverviewInlineSerpBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGoogleAiOverviewInlineSerpBlock`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGoogleAiOverviewInlineSerpBlock`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGoogleAiOverviewInlineSerpBlockRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search query — same shape as a Google Search query | 
 **gl** | **string** | Country code | [default to &quot;us&quot;]
 **hl** | **string** | Language code | [default to &quot;en&quot;]

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


## GoogleGoogleFlightsCalendarCheapestFarePerDate

> interface{} GoogleGoogleFlightsCalendarCheapestFarePerDate(ctx).DepartureId(departureId).ArrivalId(arrivalId).OutboundDateFrom(outboundDateFrom).OutboundDateTo(outboundDateTo).TripType(tripType).TripLengthDays(tripLengthDays).ReturnDateFrom(returnDateFrom).ReturnDateTo(returnDateTo).Adults(adults).Children(children).InfantsInSeat(infantsInSeat).InfantsOnLap(infantsOnLap).TravelClass(travelClass).Currency(currency).Gl(gl).Hl(hl).Execute()

Google Flights calendar — cheapest fare per date



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
	departureId := "departureId_example" // string | Departure airport IATA code or location ID
	arrivalId := "arrivalId_example" // string | Arrival airport IATA code or location ID
	outboundDateFrom := "outboundDateFrom_example" // string | First outbound date to price (YYYY-MM-DD)
	outboundDateTo := "outboundDateTo_example" // string | Last outbound date to price (YYYY-MM-DD). At most 200 days from outbound_date_from, or 14 in date-grid mode.
	tripType := "tripType_example" // string | one_way | round_trip (optional) (default to "one_way")
	tripLengthDays := int32(56) // int32 | Round-trip stay length in nights (price-graph mode). Defaults to 7. (optional)
	returnDateFrom := "returnDateFrom_example" // string | Date-grid mode: first return date. With return_date_to, returns the full outbound x return matrix (each range at most 14 days). Round-trip only. (optional)
	returnDateTo := "returnDateTo_example" // string | Date-grid mode: last return date (optional)
	adults := int32(56) // int32 |  (optional) (default to 1)
	children := int32(56) // int32 |  (optional) (default to 0)
	infantsInSeat := int32(56) // int32 |  (optional) (default to 0)
	infantsOnLap := int32(56) // int32 |  (optional) (default to 0)
	travelClass := "travelClass_example" // string |  (optional) (default to "economy")
	currency := "currency_example" // string | ISO-4217 currency (optional) (default to "USD")
	gl := "gl_example" // string |  (optional) (default to "us")
	hl := "hl_example" // string |  (optional) (default to "en")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleGoogleFlightsCalendarCheapestFarePerDate(context.Background()).DepartureId(departureId).ArrivalId(arrivalId).OutboundDateFrom(outboundDateFrom).OutboundDateTo(outboundDateTo).TripType(tripType).TripLengthDays(tripLengthDays).ReturnDateFrom(returnDateFrom).ReturnDateTo(returnDateTo).Adults(adults).Children(children).InfantsInSeat(infantsInSeat).InfantsOnLap(infantsOnLap).TravelClass(travelClass).Currency(currency).Gl(gl).Hl(hl).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGoogleFlightsCalendarCheapestFarePerDate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGoogleFlightsCalendarCheapestFarePerDate`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGoogleFlightsCalendarCheapestFarePerDate`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGoogleFlightsCalendarCheapestFarePerDateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **departureId** | **string** | Departure airport IATA code or location ID | 
 **arrivalId** | **string** | Arrival airport IATA code or location ID | 
 **outboundDateFrom** | **string** | First outbound date to price (YYYY-MM-DD) | 
 **outboundDateTo** | **string** | Last outbound date to price (YYYY-MM-DD). At most 200 days from outbound_date_from, or 14 in date-grid mode. | 
 **tripType** | **string** | one_way | round_trip | [default to &quot;one_way&quot;]
 **tripLengthDays** | **int32** | Round-trip stay length in nights (price-graph mode). Defaults to 7. | 
 **returnDateFrom** | **string** | Date-grid mode: first return date. With return_date_to, returns the full outbound x return matrix (each range at most 14 days). Round-trip only. | 
 **returnDateTo** | **string** | Date-grid mode: last return date | 
 **adults** | **int32** |  | [default to 1]
 **children** | **int32** |  | [default to 0]
 **infantsInSeat** | **int32** |  | [default to 0]
 **infantsOnLap** | **int32** |  | [default to 0]
 **travelClass** | **string** |  | [default to &quot;economy&quot;]
 **currency** | **string** | ISO-4217 currency | [default to &quot;USD&quot;]
 **gl** | **string** |  | [default to &quot;us&quot;]
 **hl** | **string** |  | [default to &quot;en&quot;]

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


## GoogleGoogleFlightsSearch

> interface{} GoogleGoogleFlightsSearch(ctx).DepartureId(departureId).ArrivalId(arrivalId).OutboundDate(outboundDate).ReturnDate(returnDate).TripType(tripType).Adults(adults).Children(children).InfantsInSeat(infantsInSeat).InfantsOnLap(infantsOnLap).TravelClass(travelClass).Currency(currency).Gl(gl).Hl(hl).Stops(stops).MaxPrice(maxPrice).DepartureToken(departureToken).Execute()

Google Flights search



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
	departureId := "departureId_example" // string | Departure airport IATA code or location ID
	arrivalId := "arrivalId_example" // string | Arrival airport IATA code or location ID
	outboundDate := "outboundDate_example" // string | Outbound date (YYYY-MM-DD)
	returnDate := "returnDate_example" // string | Return date (round-trip only) (optional)
	tripType := "tripType_example" // string | round_trip | one_way | multi_city (optional) (default to "round_trip")
	adults := int32(56) // int32 |  (optional) (default to 1)
	children := int32(56) // int32 |  (optional) (default to 0)
	infantsInSeat := int32(56) // int32 |  (optional) (default to 0)
	infantsOnLap := int32(56) // int32 |  (optional) (default to 0)
	travelClass := "travelClass_example" // string |  (optional) (default to "economy")
	currency := "currency_example" // string | ISO-4217 currency (optional) (default to "USD")
	gl := "gl_example" // string |  (optional) (default to "us")
	hl := "hl_example" // string |  (optional) (default to "en")
	stops := "stops_example" // string |  (optional) (default to "any")
	maxPrice := int32(56) // int32 |  (optional)
	departureToken := "departureToken_example" // string | A round-trip offer's departure_token; returns the return-leg flights for that selected outbound (round-trip only). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleGoogleFlightsSearch(context.Background()).DepartureId(departureId).ArrivalId(arrivalId).OutboundDate(outboundDate).ReturnDate(returnDate).TripType(tripType).Adults(adults).Children(children).InfantsInSeat(infantsInSeat).InfantsOnLap(infantsOnLap).TravelClass(travelClass).Currency(currency).Gl(gl).Hl(hl).Stops(stops).MaxPrice(maxPrice).DepartureToken(departureToken).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGoogleFlightsSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGoogleFlightsSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGoogleFlightsSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGoogleFlightsSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **departureId** | **string** | Departure airport IATA code or location ID | 
 **arrivalId** | **string** | Arrival airport IATA code or location ID | 
 **outboundDate** | **string** | Outbound date (YYYY-MM-DD) | 
 **returnDate** | **string** | Return date (round-trip only) | 
 **tripType** | **string** | round_trip | one_way | multi_city | [default to &quot;round_trip&quot;]
 **adults** | **int32** |  | [default to 1]
 **children** | **int32** |  | [default to 0]
 **infantsInSeat** | **int32** |  | [default to 0]
 **infantsOnLap** | **int32** |  | [default to 0]
 **travelClass** | **string** |  | [default to &quot;economy&quot;]
 **currency** | **string** | ISO-4217 currency | [default to &quot;USD&quot;]
 **gl** | **string** |  | [default to &quot;us&quot;]
 **hl** | **string** |  | [default to &quot;en&quot;]
 **stops** | **string** |  | [default to &quot;any&quot;]
 **maxPrice** | **int32** |  | 
 **departureToken** | **string** | A round-trip offer&#39;s departure_token; returns the return-leg flights for that selected outbound (round-trip only). | 

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


## GoogleGoogleLensVisualSearch

> interface{} GoogleGoogleLensVisualSearch(ctx).Url(url).Query(query).Country(country).Language(language).Gl(gl).Hl(hl).Product(product).VisualMatches(visualMatches).ExactMatches(exactMatches).Execute()

Google Lens visual search



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
	url := "url_example" // string | Public URL of the image to search visually
	query := "query_example" // string | Optional text refinement (e.g. 'pizza') (optional)
	country := "country_example" // string | ISO country code (alias for gl) (optional)
	language := "language_example" // string | Language code (alias for hl) (optional)
	gl := "gl_example" // string | Country code (optional) (default to "us")
	hl := "hl_example" // string | Language code (optional) (default to "en")
	product := true // bool | Bias towards shoppable product matches (optional) (default to false)
	visualMatches := true // bool | Include the visual-matches carousel (optional) (default to true)
	exactMatches := true // bool | Restrict to exact-match results (optional) (default to false)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleGoogleLensVisualSearch(context.Background()).Url(url).Query(query).Country(country).Language(language).Gl(gl).Hl(hl).Product(product).VisualMatches(visualMatches).ExactMatches(exactMatches).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGoogleLensVisualSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGoogleLensVisualSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGoogleLensVisualSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGoogleLensVisualSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **url** | **string** | Public URL of the image to search visually | 
 **query** | **string** | Optional text refinement (e.g. &#39;pizza&#39;) | 
 **country** | **string** | ISO country code (alias for gl) | 
 **language** | **string** | Language code (alias for hl) | 
 **gl** | **string** | Country code | [default to &quot;us&quot;]
 **hl** | **string** | Language code | [default to &quot;en&quot;]
 **product** | **bool** | Bias towards shoppable product matches | [default to false]
 **visualMatches** | **bool** | Include the visual-matches carousel | [default to true]
 **exactMatches** | **bool** | Restrict to exact-match results | [default to false]

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


## GoogleGoogleScraperHealthCheck

> interface{} GoogleGoogleScraperHealthCheck(ctx).Execute()

Google scraper health check



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
	resp, r, err := apiClient.GoogleAPI.GoogleGoogleScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGoogleScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGoogleScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGoogleScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGoogleScraperHealthCheckRequest struct via the builder pattern


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


## GoogleGoogleScraperHealthCheckHead

> interface{} GoogleGoogleScraperHealthCheckHead(ctx).Execute()

Google scraper health check



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
	resp, r, err := apiClient.GoogleAPI.GoogleGoogleScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGoogleScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGoogleScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGoogleScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGoogleScraperHealthCheckHeadRequest struct via the builder pattern


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


## GoogleGoogleSearchSuggestions

> interface{} GoogleGoogleSearchSuggestions(ctx).Q(q).Hl(hl).Gl(gl).Execute()

Google search suggestions



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
	q := "q_example" // string | Search query to get suggestions for
	hl := "hl_example" // string | Language code (optional) (default to "en")
	gl := "gl_example" // string | Country code (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleGoogleSearchSuggestions(context.Background()).Q(q).Hl(hl).Gl(gl).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGoogleSearchSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGoogleSearchSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGoogleSearchSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGoogleSearchSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search query to get suggestions for | 
 **hl** | **string** | Language code | [default to &quot;en&quot;]
 **gl** | **string** | Country code | [default to &quot;us&quot;]

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


## GoogleGoogleShortsSearch

> interface{} GoogleGoogleShortsSearch(ctx).Q(q).Gl(gl).Hl(hl).Domain(domain).Num(num).Start(start).Execute()

Google Shorts search



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
	q := "q_example" // string | Search query
	gl := "gl_example" // string | Country code (optional) (default to "us")
	hl := "hl_example" // string | Language code (optional) (default to "en")
	domain := "domain_example" // string | Google domain (optional) (default to "google.com")
	num := int32(56) // int32 | Results per page (optional) (default to 20)
	start := int32(56) // int32 | Pagination offset (optional) (default to 0)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleGoogleShortsSearch(context.Background()).Q(q).Gl(gl).Hl(hl).Domain(domain).Num(num).Start(start).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGoogleShortsSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGoogleShortsSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGoogleShortsSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGoogleShortsSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search query | 
 **gl** | **string** | Country code | [default to &quot;us&quot;]
 **hl** | **string** | Language code | [default to &quot;en&quot;]
 **domain** | **string** | Google domain | [default to &quot;google.com&quot;]
 **num** | **int32** | Results per page | [default to 20]
 **start** | **int32** | Pagination offset | [default to 0]

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


## GoogleGoogleWebSearch

> interface{} GoogleGoogleWebSearch(ctx).Q(q).Gl(gl).Hl(hl).Num(num).Start(start).Domain(domain).Device(device).UserAgent(userAgent).Output(output).Location(location).Lr(lr).Tbs(tbs).Safe(safe).Uule(uule).Filter(filter).Nfpr(nfpr).Cr(cr).Ludocid(ludocid).Lsig(lsig).Kgmid(kgmid).Si(si).Ibp(ibp).Uds(uds).AiOverview(aiOverview).Execute()

Google web search



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
	q := "q_example" // string | Search query (supports Google operators)
	gl := "gl_example" // string | Country code (optional) (default to "us")
	hl := "hl_example" // string | Language code (optional) (default to "en")
	num := int32(56) // int32 |  (optional) (default to 10)
	start := int32(56) // int32 | Page offset (0, 10, 20...) (optional) (default to 0)
	domain := "domain_example" // string | Google domain (optional) (default to "google.com")
	device := "device_example" // string | Device target: desktop, mobile, iphone, android, tablet (optional) (default to "desktop")
	userAgent := "userAgent_example" // string | Custom User-Agent (overrides device) (optional)
	output := "output_example" // string | Response format: json (parsed) or html (raw SERP) (optional) (default to "json")
	location := "location_example" // string | City-level geo-targeting (optional)
	lr := "lr_example" // string | Language restrict (e.g. lang_en) (optional)
	tbs := "tbs_example" // string | Time filter (e.g. qdr:d) (optional)
	safe := "safe_example" // string |  (optional) (default to "off")
	uule := "uule_example" // string | UULE encoded location (optional)
	filter := int32(56) // int32 | Show omitted results (optional)
	nfpr := int32(56) // int32 | Disable auto-correction (optional) (default to 0)
	cr := "cr_example" // string | Country restrict (optional)
	ludocid := "ludocid_example" // string | Google Place CID (optional)
	lsig := "lsig_example" // string | Knowledge Graph map ID (optional)
	kgmid := "kgmid_example" // string | Knowledge Graph entity ID (optional)
	si := "si_example" // string | Cached search params (optional)
	ibp := "ibp_example" // string | Layout control (optional)
	uds := "uds_example" // string | Google filter string (optional)
	aiOverview := true // bool | Chase deferred AI Overview page_token with a follow-up fetch and merge the result. Adds ~1s and 1 credit when the SERP defers the overview. (optional) (default to false)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleGoogleWebSearch(context.Background()).Q(q).Gl(gl).Hl(hl).Num(num).Start(start).Domain(domain).Device(device).UserAgent(userAgent).Output(output).Location(location).Lr(lr).Tbs(tbs).Safe(safe).Uule(uule).Filter(filter).Nfpr(nfpr).Cr(cr).Ludocid(ludocid).Lsig(lsig).Kgmid(kgmid).Si(si).Ibp(ibp).Uds(uds).AiOverview(aiOverview).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleGoogleWebSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleGoogleWebSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleGoogleWebSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleGoogleWebSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search query (supports Google operators) | 
 **gl** | **string** | Country code | [default to &quot;us&quot;]
 **hl** | **string** | Language code | [default to &quot;en&quot;]
 **num** | **int32** |  | [default to 10]
 **start** | **int32** | Page offset (0, 10, 20...) | [default to 0]
 **domain** | **string** | Google domain | [default to &quot;google.com&quot;]
 **device** | **string** | Device target: desktop, mobile, iphone, android, tablet | [default to &quot;desktop&quot;]
 **userAgent** | **string** | Custom User-Agent (overrides device) | 
 **output** | **string** | Response format: json (parsed) or html (raw SERP) | [default to &quot;json&quot;]
 **location** | **string** | City-level geo-targeting | 
 **lr** | **string** | Language restrict (e.g. lang_en) | 
 **tbs** | **string** | Time filter (e.g. qdr:d) | 
 **safe** | **string** |  | [default to &quot;off&quot;]
 **uule** | **string** | UULE encoded location | 
 **filter** | **int32** | Show omitted results | 
 **nfpr** | **int32** | Disable auto-correction | [default to 0]
 **cr** | **string** | Country restrict | 
 **ludocid** | **string** | Google Place CID | 
 **lsig** | **string** | Knowledge Graph map ID | 
 **kgmid** | **string** | Knowledge Graph entity ID | 
 **si** | **string** | Cached search params | 
 **ibp** | **string** | Layout control | 
 **uds** | **string** | Google filter string | 
 **aiOverview** | **bool** | Chase deferred AI Overview page_token with a follow-up fetch and merge the result. Adds ~1s and 1 credit when the SERP defers the overview. | [default to false]

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


## GoogleHotelDetails

> interface{} GoogleHotelDetails(ctx).PropertyToken(propertyToken).CheckIn(checkIn).CheckOut(checkOut).Execute()

Hotel details

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
	propertyToken := "propertyToken_example" // string | Property token
	checkIn := "checkIn_example" // string | YYYY-MM-DD
	checkOut := "checkOut_example" // string | YYYY-MM-DD

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleHotelDetails(context.Background()).PropertyToken(propertyToken).CheckIn(checkIn).CheckOut(checkOut).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleHotelDetails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleHotelDetails`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleHotelDetails`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleHotelDetailsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **propertyToken** | **string** | Property token | 
 **checkIn** | **string** | YYYY-MM-DD | 
 **checkOut** | **string** | YYYY-MM-DD | 

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


## GoogleImmersiveProductDetail

> interface{} GoogleImmersiveProductDetail(ctx).ProductId(productId).Q(q).Gl(gl).Hl(hl).CatalogId(catalogId).ImageDocid(imageDocid).HeadlineOfferDocid(headlineOfferDocid).Mid(mid).IncludeOffers(includeOffers).IncludeVariants(includeVariants).Execute()

Immersive product detail



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
	productId := "productId_example" // string | Google Shopping ``gpcid`` — the product_id returned on ``/shopping/search`` tiles. Scrapingdog-compatible.
	q := "q_example" // string | Original search query that surfaced the product. Required by Google's ``/async/oapv`` RPC.
	gl := "gl_example" // string | Country code (ISO 3166 alpha-2) (optional) (default to "us")
	hl := "hl_example" // string | Language code (optional) (default to "en")
	catalogId := "catalogId_example" // string | Optional ``catalogid`` from the Shopping tile (improves parity). (optional)
	imageDocid := "imageDocid_example" // string | Optional ``imageDocid`` for higher-fidelity images. (optional)
	headlineOfferDocid := "headlineOfferDocid_example" // string | Optional ``headlineOfferDocid`` to pin the featured seller. (optional)
	mid := "mid_example" // string | Optional Google Knowledge-Graph ``mid``. (optional)
	includeOffers := true // bool | When true, fetch the full merchant-offer list via a secondary RPC (``/async/piu_ps``). Adds ~1 s. (optional) (default to false)
	includeVariants := true // bool | When true, fetch size/colour variants via a secondary RPC (``/async/toy_v``). Adds ~1 s. (optional) (default to false)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleImmersiveProductDetail(context.Background()).ProductId(productId).Q(q).Gl(gl).Hl(hl).CatalogId(catalogId).ImageDocid(imageDocid).HeadlineOfferDocid(headlineOfferDocid).Mid(mid).IncludeOffers(includeOffers).IncludeVariants(includeVariants).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleImmersiveProductDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleImmersiveProductDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleImmersiveProductDetail`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleImmersiveProductDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productId** | **string** | Google Shopping &#x60;&#x60;gpcid&#x60;&#x60; — the product_id returned on &#x60;&#x60;/shopping/search&#x60;&#x60; tiles. Scrapingdog-compatible. | 
 **q** | **string** | Original search query that surfaced the product. Required by Google&#39;s &#x60;&#x60;/async/oapv&#x60;&#x60; RPC. | 
 **gl** | **string** | Country code (ISO 3166 alpha-2) | [default to &quot;us&quot;]
 **hl** | **string** | Language code | [default to &quot;en&quot;]
 **catalogId** | **string** | Optional &#x60;&#x60;catalogid&#x60;&#x60; from the Shopping tile (improves parity). | 
 **imageDocid** | **string** | Optional &#x60;&#x60;imageDocid&#x60;&#x60; for higher-fidelity images. | 
 **headlineOfferDocid** | **string** | Optional &#x60;&#x60;headlineOfferDocid&#x60;&#x60; to pin the featured seller. | 
 **mid** | **string** | Optional Google Knowledge-Graph &#x60;&#x60;mid&#x60;&#x60;. | 
 **includeOffers** | **bool** | When true, fetch the full merchant-offer list via a secondary RPC (&#x60;&#x60;/async/piu_ps&#x60;&#x60;). Adds ~1 s. | [default to false]
 **includeVariants** | **bool** | When true, fetch size/colour variants via a secondary RPC (&#x60;&#x60;/async/toy_v&#x60;&#x60;). Adds ~1 s. | [default to false]

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


## GoogleInterestByRegion

> interface{} GoogleInterestByRegion(ctx).Q(q).Geo(geo).Execute()

Interest by region

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
	q := "q_example" // string | Search term
	geo := "geo_example" // string |  (optional) (default to "")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleInterestByRegion(context.Background()).Q(q).Geo(geo).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleInterestByRegion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleInterestByRegion`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleInterestByRegion`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleInterestByRegionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search term | 
 **geo** | **string** |  | [default to &quot;&quot;]

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


## GoogleInterestOverTime

> interface{} GoogleInterestOverTime(ctx).Q(q).Geo(geo).Date(date).Execute()

Interest over time

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
	q := "q_example" // string | Search terms
	geo := "geo_example" // string |  (optional) (default to "")
	date := "date_example" // string |  (optional) (default to "today 12-m")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleInterestOverTime(context.Background()).Q(q).Geo(geo).Date(date).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleInterestOverTime``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleInterestOverTime`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleInterestOverTime`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleInterestOverTimeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search terms | 
 **geo** | **string** |  | [default to &quot;&quot;]
 **date** | **string** |  | [default to &quot;today 12-m&quot;]

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


## GoogleMultiSellerOffersByBarcode

> interface{} GoogleMultiSellerOffersByBarcode(ctx).Barcode(barcode).Gl(gl).Hl(hl).Execute()

Multi-seller offers by barcode



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
	barcode := "barcode_example" // string | Product barcode — GTIN-8 / UPC-A / EAN-13 / GTIN-14
	gl := "gl_example" // string | Country code (ISO 3166 alpha-2) (optional)
	hl := "hl_example" // string | Language code (optional) (default to "en")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleMultiSellerOffersByBarcode(context.Background()).Barcode(barcode).Gl(gl).Hl(hl).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleMultiSellerOffersByBarcode``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleMultiSellerOffersByBarcode`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleMultiSellerOffersByBarcode`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleMultiSellerOffersByBarcodeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **barcode** | **string** | Product barcode — GTIN-8 / UPC-A / EAN-13 / GTIN-14 | 
 **gl** | **string** | Country code (ISO 3166 alpha-2) | 
 **hl** | **string** | Language code | [default to &quot;en&quot;]

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


## GoogleNewsByTopic

> interface{} GoogleNewsByTopic(ctx).Topic(topic).Hl(hl).Gl(gl).MaxResults(maxResults).Execute()

News by topic

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
	topic := "topic_example" // string | Topic name
	hl := "hl_example" // string |  (optional) (default to "en")
	gl := "gl_example" // string |  (optional) (default to "US")
	maxResults := int32(56) // int32 |  (optional) (default to 10)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleNewsByTopic(context.Background()).Topic(topic).Hl(hl).Gl(gl).MaxResults(maxResults).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleNewsByTopic``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleNewsByTopic`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleNewsByTopic`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleNewsByTopicRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **topic** | **string** | Topic name | 
 **hl** | **string** |  | [default to &quot;en&quot;]
 **gl** | **string** |  | [default to &quot;US&quot;]
 **maxResults** | **int32** |  | [default to 10]

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


## GooglePatentDetails

> interface{} GooglePatentDetails(ctx).PatentId(patentId).Execute()

Patent details

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
	patentId := "patentId_example" // string | Patent number

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GooglePatentDetails(context.Background()).PatentId(patentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GooglePatentDetails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GooglePatentDetails`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GooglePatentDetails`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGooglePatentDetailsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **patentId** | **string** | Patent number | 

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


## GoogleRelatedTopicsQueries

> interface{} GoogleRelatedTopicsQueries(ctx).Q(q).Geo(geo).Execute()

Related topics & queries

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
	q := "q_example" // string | Search term
	geo := "geo_example" // string |  (optional) (default to "")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleRelatedTopicsQueries(context.Background()).Q(q).Geo(geo).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleRelatedTopicsQueries``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleRelatedTopicsQueries`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleRelatedTopicsQueries`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleRelatedTopicsQueriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search term | 
 **geo** | **string** |  | [default to &quot;&quot;]

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


## GoogleSearchGoogleImages

> interface{} GoogleSearchGoogleImages(ctx).Q(q).Gl(gl).Hl(hl).Tbs(tbs).Imgsz(imgsz).Imgcolor(imgcolor).Imgtype(imgtype).Safe(safe).Page(page).Execute()

Search Google Images



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
	q := "q_example" // string | Image search query
	gl := "gl_example" // string | Country code (optional) (default to "us")
	hl := "hl_example" // string | Language code (optional) (default to "en")
	tbs := "tbs_example" // string | Time/filter string (e.g. qdr:d) (optional)
	imgsz := "imgsz_example" // string | Image size: l, m, i, xXl (optional)
	imgcolor := "imgcolor_example" // string | Image color filter (optional)
	imgtype := "imgtype_example" // string | Image type: face, photo, clipart (optional)
	safe := "safe_example" // string | Safe search (optional) (default to "off")
	page := int32(56) // int32 | Page number (optional) (default to 0)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleSearchGoogleImages(context.Background()).Q(q).Gl(gl).Hl(hl).Tbs(tbs).Imgsz(imgsz).Imgcolor(imgcolor).Imgtype(imgtype).Safe(safe).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleSearchGoogleImages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleSearchGoogleImages`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleSearchGoogleImages`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleSearchGoogleImagesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Image search query | 
 **gl** | **string** | Country code | [default to &quot;us&quot;]
 **hl** | **string** | Language code | [default to &quot;en&quot;]
 **tbs** | **string** | Time/filter string (e.g. qdr:d) | 
 **imgsz** | **string** | Image size: l, m, i, xXl | 
 **imgcolor** | **string** | Image color filter | 
 **imgtype** | **string** | Image type: face, photo, clipart | 
 **safe** | **string** | Safe search | [default to &quot;off&quot;]
 **page** | **int32** | Page number | [default to 0]

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


## GoogleSearchGoogleJobs

> interface{} GoogleSearchGoogleJobs(ctx).Q(q).Location(location).Gl(gl).JobType(jobType).DatePosted(datePosted).Execute()

Search Google Jobs

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
	q := "q_example" // string | Job title, keywords
	location := "location_example" // string |  (optional)
	gl := "gl_example" // string |  (optional) (default to "us")
	jobType := "jobType_example" // string |  (optional)
	datePosted := "datePosted_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleSearchGoogleJobs(context.Background()).Q(q).Location(location).Gl(gl).JobType(jobType).DatePosted(datePosted).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleSearchGoogleJobs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleSearchGoogleJobs`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleSearchGoogleJobs`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleSearchGoogleJobsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Job title, keywords | 
 **location** | **string** |  | 
 **gl** | **string** |  | [default to &quot;us&quot;]
 **jobType** | **string** |  | 
 **datePosted** | **string** |  | 

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


## GoogleSearchGoogleMapsPlaces

> interface{} GoogleSearchGoogleMapsPlaces(ctx).Q(q).Ll(ll).Gl(gl).Hl(hl).Start(start).Execute()

Search Google Maps places

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
	q := "q_example" // string | Search query
	ll := "ll_example" // string |  (optional)
	gl := "gl_example" // string |  (optional) (default to "us")
	hl := "hl_example" // string |  (optional) (default to "en")
	start := int32(56) // int32 |  (optional) (default to 0)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleSearchGoogleMapsPlaces(context.Background()).Q(q).Ll(ll).Gl(gl).Hl(hl).Start(start).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleSearchGoogleMapsPlaces``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleSearchGoogleMapsPlaces`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleSearchGoogleMapsPlaces`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleSearchGoogleMapsPlacesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search query | 
 **ll** | **string** |  | 
 **gl** | **string** |  | [default to &quot;us&quot;]
 **hl** | **string** |  | [default to &quot;en&quot;]
 **start** | **int32** |  | [default to 0]

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


## GoogleSearchGoogleNews

> interface{} GoogleSearchGoogleNews(ctx).Q(q).Hl(hl).Gl(gl).MaxResults(maxResults).Execute()

Search Google News

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
	q := "q_example" // string | Search query
	hl := "hl_example" // string |  (optional) (default to "en")
	gl := "gl_example" // string |  (optional) (default to "US")
	maxResults := int32(56) // int32 |  (optional) (default to 10)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleSearchGoogleNews(context.Background()).Q(q).Hl(hl).Gl(gl).MaxResults(maxResults).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleSearchGoogleNews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleSearchGoogleNews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleSearchGoogleNews`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleSearchGoogleNewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search query | 
 **hl** | **string** |  | [default to &quot;en&quot;]
 **gl** | **string** |  | [default to &quot;US&quot;]
 **maxResults** | **int32** |  | [default to 10]

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


## GoogleSearchGoogleScholar

> interface{} GoogleSearchGoogleScholar(ctx).Q(q).Hl(hl).AsYlo(asYlo).AsYhi(asYhi).AsSdt(asSdt).Page(page).Num(num).Execute()

Search Google Scholar



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
	q := "q_example" // string | Search query for scholarly articles
	hl := "hl_example" // string | Language code (optional) (default to "en")
	asYlo := int32(56) // int32 | Year from (e.g. 2020) (optional)
	asYhi := int32(56) // int32 | Year to (e.g. 2024) (optional)
	asSdt := "asSdt_example" // string | Search type: 0=exclude patents, 7=include (optional) (default to "0")
	page := int32(56) // int32 | Page number (0-based) (optional) (default to 0)
	num := int32(56) // int32 | Results per page (max 20) (optional) (default to 10)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleSearchGoogleScholar(context.Background()).Q(q).Hl(hl).AsYlo(asYlo).AsYhi(asYhi).AsSdt(asSdt).Page(page).Num(num).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleSearchGoogleScholar``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleSearchGoogleScholar`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleSearchGoogleScholar`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleSearchGoogleScholarRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search query for scholarly articles | 
 **hl** | **string** | Language code | [default to &quot;en&quot;]
 **asYlo** | **int32** | Year from (e.g. 2020) | 
 **asYhi** | **int32** | Year to (e.g. 2024) | 
 **asSdt** | **string** | Search type: 0&#x3D;exclude patents, 7&#x3D;include | [default to &quot;0&quot;]
 **page** | **int32** | Page number (0-based) | [default to 0]
 **num** | **int32** | Results per page (max 20) | [default to 10]

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


## GoogleSearchGoogleVideos

> interface{} GoogleSearchGoogleVideos(ctx).Q(q).Gl(gl).Hl(hl).Tbs(tbs).Safe(safe).Page(page).Execute()

Search Google Videos



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
	q := "q_example" // string | Video search query
	gl := "gl_example" // string | Country code (optional) (default to "us")
	hl := "hl_example" // string | Language code (optional) (default to "en")
	tbs := "tbs_example" // string | Time filter (e.g. qdr:d) (optional)
	safe := "safe_example" // string | Safe search (optional) (default to "off")
	page := int32(56) // int32 | Page number (optional) (default to 0)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleSearchGoogleVideos(context.Background()).Q(q).Gl(gl).Hl(hl).Tbs(tbs).Safe(safe).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleSearchGoogleVideos``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleSearchGoogleVideos`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleSearchGoogleVideos`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleSearchGoogleVideosRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Video search query | 
 **gl** | **string** | Country code | [default to &quot;us&quot;]
 **hl** | **string** | Language code | [default to &quot;en&quot;]
 **tbs** | **string** | Time filter (e.g. qdr:d) | 
 **safe** | **string** | Safe search | [default to &quot;off&quot;]
 **page** | **int32** | Page number | [default to 0]

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


## GoogleSearchHotels

> interface{} GoogleSearchHotels(ctx).Q(q).CheckIn(checkIn).CheckOut(checkOut).Adults(adults).Currency(currency).Gl(gl).Execute()

Search hotels

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
	q := "q_example" // string | Location or hotel name
	checkIn := "checkIn_example" // string | YYYY-MM-DD
	checkOut := "checkOut_example" // string | YYYY-MM-DD
	adults := int32(56) // int32 |  (optional) (default to 2)
	currency := "currency_example" // string |  (optional) (default to "USD")
	gl := "gl_example" // string |  (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleSearchHotels(context.Background()).Q(q).CheckIn(checkIn).CheckOut(checkOut).Adults(adults).Currency(currency).Gl(gl).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleSearchHotels``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleSearchHotels`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleSearchHotels`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleSearchHotelsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Location or hotel name | 
 **checkIn** | **string** | YYYY-MM-DD | 
 **checkOut** | **string** | YYYY-MM-DD | 
 **adults** | **int32** |  | [default to 2]
 **currency** | **string** |  | [default to &quot;USD&quot;]
 **gl** | **string** |  | [default to &quot;us&quot;]

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


## GoogleSearchPatents

> interface{} GoogleSearchPatents(ctx).Q(q).Page(page).Num(num).Sort(sort).Inventor(inventor).Assignee(assignee).Country(country).Language(language).Status(status).PatentType(patentType).Before(before).After(after).Execute()

Search patents

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
	q := "q_example" // string | Search query (Boolean logic supported)
	page := int32(56) // int32 |  (optional) (default to 0)
	num := int32(56) // int32 |  (optional) (default to 10)
	sort := "sort_example" // string | 'new' or 'old' (optional)
	inventor := "inventor_example" // string | Inventor name(s) (optional)
	assignee := "assignee_example" // string | Assignee / company name(s) (optional)
	country := "country_example" // string | Country code (US, EP, WO, …) (optional)
	language := "language_example" // string | Patent language: ENGLISH, GERMAN, CHINESE, FRENCH, JAPANESE, KOREAN, SPANISH (optional)
	status := "status_example" // string | GRANT or APPLICATION (optional)
	patentType := "patentType_example" // string | PATENT or DESIGN (optional)
	before := "before_example" // string | Before date YYYYMMDD (optional)
	after := "after_example" // string | After date YYYYMMDD (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleSearchPatents(context.Background()).Q(q).Page(page).Num(num).Sort(sort).Inventor(inventor).Assignee(assignee).Country(country).Language(language).Status(status).PatentType(patentType).Before(before).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleSearchPatents``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleSearchPatents`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleSearchPatents`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleSearchPatentsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search query (Boolean logic supported) | 
 **page** | **int32** |  | [default to 0]
 **num** | **int32** |  | [default to 10]
 **sort** | **string** | &#39;new&#39; or &#39;old&#39; | 
 **inventor** | **string** | Inventor name(s) | 
 **assignee** | **string** | Assignee / company name(s) | 
 **country** | **string** | Country code (US, EP, WO, …) | 
 **language** | **string** | Patent language: ENGLISH, GERMAN, CHINESE, FRENCH, JAPANESE, KOREAN, SPANISH | 
 **status** | **string** | GRANT or APPLICATION | 
 **patentType** | **string** | PATENT or DESIGN | 
 **before** | **string** | Before date YYYYMMDD | 
 **after** | **string** | After date YYYYMMDD | 

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


## GoogleSearchProducts

> interface{} GoogleSearchProducts(ctx).Q(q).Gl(gl).MinPrice(minPrice).MaxPrice(maxPrice).SortBy(sortBy).Execute()

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
	q := "q_example" // string | Product search query
	gl := "gl_example" // string |  (optional) (default to "us")
	minPrice := int32(56) // int32 |  (optional)
	maxPrice := int32(56) // int32 |  (optional)
	sortBy := "sortBy_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleSearchProducts(context.Background()).Q(q).Gl(gl).MinPrice(minPrice).MaxPrice(maxPrice).SortBy(sortBy).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleSearchProducts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleSearchProducts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleSearchProducts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleSearchProductsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Product search query | 
 **gl** | **string** |  | [default to &quot;us&quot;]
 **minPrice** | **int32** |  | 
 **maxPrice** | **int32** |  | 
 **sortBy** | **string** |  | 

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


## GoogleSearchScholarAuthorProfiles

> interface{} GoogleSearchScholarAuthorProfiles(ctx).Mauthors(mauthors).Hl(hl).AfterAuthor(afterAuthor).BeforeAuthor(beforeAuthor).Execute()

Search Scholar author profiles



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
	mauthors := "mauthors_example" // string | Author name query (e.g. 'Geoffrey Hinton')
	hl := "hl_example" // string | Language code (optional) (default to "en")
	afterAuthor := "afterAuthor_example" // string | Pagination token (next page) (optional)
	beforeAuthor := "beforeAuthor_example" // string | Pagination token (previous page) (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleSearchScholarAuthorProfiles(context.Background()).Mauthors(mauthors).Hl(hl).AfterAuthor(afterAuthor).BeforeAuthor(beforeAuthor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleSearchScholarAuthorProfiles``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleSearchScholarAuthorProfiles`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleSearchScholarAuthorProfiles`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleSearchScholarAuthorProfilesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mauthors** | **string** | Author name query (e.g. &#39;Geoffrey Hinton&#39;) | 
 **hl** | **string** | Language code | [default to &quot;en&quot;]
 **afterAuthor** | **string** | Pagination token (next page) | 
 **beforeAuthor** | **string** | Pagination token (previous page) | 

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


## GoogleTrendingNews

> interface{} GoogleTrendingNews(ctx).Hl(hl).Gl(gl).MaxResults(maxResults).Execute()

Trending news

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
	hl := "hl_example" // string |  (optional) (default to "en")
	gl := "gl_example" // string |  (optional) (default to "US")
	maxResults := int32(56) // int32 |  (optional) (default to 10)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleTrendingNews(context.Background()).Hl(hl).Gl(gl).MaxResults(maxResults).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleTrendingNews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleTrendingNews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleTrendingNews`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleTrendingNewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **hl** | **string** |  | [default to &quot;en&quot;]
 **gl** | **string** |  | [default to &quot;US&quot;]
 **maxResults** | **int32** |  | [default to 10]

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


## GoogleTrendingSearches

> interface{} GoogleTrendingSearches(ctx).Geo(geo).Execute()

Trending searches

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
	geo := "geo_example" // string |  (optional) (default to "US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleTrendingSearches(context.Background()).Geo(geo).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleTrendingSearches``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleTrendingSearches`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleTrendingSearches`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleTrendingSearchesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **geo** | **string** |  | [default to &quot;US&quot;]

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


## GoogleTrendsTopicAutocomplete

> interface{} GoogleTrendsTopicAutocomplete(ctx).Q(q).Hl(hl).Tz(tz).Execute()

Trends topic autocomplete



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
	q := "q_example" // string | Query prefix to resolve into Trends topics
	hl := "hl_example" // string | Language code (optional) (default to "en-US")
	tz := "tz_example" // string | Timezone offset in minutes (optional) (default to "0")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GoogleAPI.GoogleTrendsTopicAutocomplete(context.Background()).Q(q).Hl(hl).Tz(tz).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GoogleAPI.GoogleTrendsTopicAutocomplete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleTrendsTopicAutocomplete`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `GoogleAPI.GoogleTrendsTopicAutocomplete`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleTrendsTopicAutocompleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Query prefix to resolve into Trends topics | 
 **hl** | **string** | Language code | [default to &quot;en-US&quot;]
 **tz** | **string** | Timezone offset in minutes | [default to &quot;0&quot;]

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


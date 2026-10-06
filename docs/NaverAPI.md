# \NaverAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**NaverNaverBlogSearch**](NaverAPI.md#NaverNaverBlogSearch) | **Get** /v1/naver/blog | Naver blog search
[**NaverNaverDatalabShoppingKeywordInsight**](NaverAPI.md#NaverNaverDatalabShoppingKeywordInsight) | **Get** /v1/naver/shopping/insight | Naver DataLab shopping keyword insight
[**NaverNaverNewsSearch**](NaverAPI.md#NaverNaverNewsSearch) | **Get** /v1/naver/news | Naver news search
[**NaverNaverPlaceDetail**](NaverAPI.md#NaverNaverPlaceDetail) | **Get** /v1/naver/place/{place_id} | Naver place detail
[**NaverNaverPlaceLocalSearch**](NaverAPI.md#NaverNaverPlaceLocalSearch) | **Get** /v1/naver/local | Naver Place/Local search
[**NaverNaverPlaceVisitorReviews**](NaverAPI.md#NaverNaverPlaceVisitorReviews) | **Get** /v1/naver/place/{place_id}/reviews | Naver place visitor reviews
[**NaverNaverScraperHealthCheck**](NaverAPI.md#NaverNaverScraperHealthCheck) | **Get** /v1/naver/health | Naver scraper health check
[**NaverNaverScraperHealthCheckHead**](NaverAPI.md#NaverNaverScraperHealthCheckHead) | **Head** /v1/naver/health | Naver scraper health check
[**NaverNaverShoppingBestsellerRankings**](NaverAPI.md#NaverNaverShoppingBestsellerRankings) | **Get** /v1/naver/shopping/bestsellers | Naver Shopping bestseller rankings
[**NaverNaverShoppingCategoryReference**](NaverAPI.md#NaverNaverShoppingCategoryReference) | **Get** /v1/naver/shopping/categories | Naver Shopping category reference
[**NaverNaverShoppingTrendingKeywordRankings**](NaverAPI.md#NaverNaverShoppingTrendingKeywordRankings) | **Get** /v1/naver/shopping/keywords | Naver Shopping trending keyword rankings
[**NaverNaverWebSearch**](NaverAPI.md#NaverNaverWebSearch) | **Get** /v1/naver/search | Naver web search
[**NaverSearchSuggestions**](NaverAPI.md#NaverSearchSuggestions) | **Get** /v1/naver/autocomplete | Search suggestions



## NaverNaverBlogSearch

> interface{} NaverNaverBlogSearch(ctx).Query(query).Page(page).Execute()

Naver blog search



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
	query := "query_example" // string | 검색어
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NaverAPI.NaverNaverBlogSearch(context.Background()).Query(query).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NaverAPI.NaverNaverBlogSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `NaverNaverBlogSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `NaverAPI.NaverNaverBlogSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiNaverNaverBlogSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | 검색어 | 
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


## NaverNaverDatalabShoppingKeywordInsight

> interface{} NaverNaverDatalabShoppingKeywordInsight(ctx).CategoryId(categoryId).StartDate(startDate).EndDate(endDate).TimeUnit(timeUnit).Count(count).Execute()

Naver DataLab shopping keyword insight



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
	categoryId := "categoryId_example" // string | DataLab category id (cid), e.g. 50000000
	startDate := "startDate_example" // string | YYYY-MM-DD
	endDate := "endDate_example" // string | YYYY-MM-DD
	timeUnit := "timeUnit_example" // string | date | week | month (optional) (default to "date")
	count := int32(56) // int32 | Keywords to return (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NaverAPI.NaverNaverDatalabShoppingKeywordInsight(context.Background()).CategoryId(categoryId).StartDate(startDate).EndDate(endDate).TimeUnit(timeUnit).Count(count).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NaverAPI.NaverNaverDatalabShoppingKeywordInsight``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `NaverNaverDatalabShoppingKeywordInsight`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `NaverAPI.NaverNaverDatalabShoppingKeywordInsight`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiNaverNaverDatalabShoppingKeywordInsightRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **categoryId** | **string** | DataLab category id (cid), e.g. 50000000 | 
 **startDate** | **string** | YYYY-MM-DD | 
 **endDate** | **string** | YYYY-MM-DD | 
 **timeUnit** | **string** | date | week | month | [default to &quot;date&quot;]
 **count** | **int32** | Keywords to return | [default to 20]

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


## NaverNaverNewsSearch

> interface{} NaverNaverNewsSearch(ctx).Query(query).Page(page).Execute()

Naver news search



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
	query := "query_example" // string | 검색어
	page := int32(56) // int32 |  (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NaverAPI.NaverNaverNewsSearch(context.Background()).Query(query).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NaverAPI.NaverNaverNewsSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `NaverNaverNewsSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `NaverAPI.NaverNaverNewsSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiNaverNaverNewsSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | 검색어 | 
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


## NaverNaverPlaceDetail

> interface{} NaverNaverPlaceDetail(ctx, placeId).Execute()

Naver place detail



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
	placeId := "placeId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NaverAPI.NaverNaverPlaceDetail(context.Background(), placeId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NaverAPI.NaverNaverPlaceDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `NaverNaverPlaceDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `NaverAPI.NaverNaverPlaceDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**placeId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiNaverNaverPlaceDetailRequest struct via the builder pattern


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


## NaverNaverPlaceLocalSearch

> interface{} NaverNaverPlaceLocalSearch(ctx).Query(query).Execute()

Naver Place/Local search



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
	query := "query_example" // string | Place query, e.g. '성남 카페'

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NaverAPI.NaverNaverPlaceLocalSearch(context.Background()).Query(query).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NaverAPI.NaverNaverPlaceLocalSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `NaverNaverPlaceLocalSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `NaverAPI.NaverNaverPlaceLocalSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiNaverNaverPlaceLocalSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Place query, e.g. &#39;성남 카페&#39; | 

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


## NaverNaverPlaceVisitorReviews

> interface{} NaverNaverPlaceVisitorReviews(ctx, placeId).Execute()

Naver place visitor reviews



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
	placeId := "placeId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NaverAPI.NaverNaverPlaceVisitorReviews(context.Background(), placeId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NaverAPI.NaverNaverPlaceVisitorReviews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `NaverNaverPlaceVisitorReviews`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `NaverAPI.NaverNaverPlaceVisitorReviews`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**placeId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiNaverNaverPlaceVisitorReviewsRequest struct via the builder pattern


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


## NaverNaverScraperHealthCheck

> interface{} NaverNaverScraperHealthCheck(ctx).Execute()

Naver scraper health check



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
	resp, r, err := apiClient.NaverAPI.NaverNaverScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NaverAPI.NaverNaverScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `NaverNaverScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `NaverAPI.NaverNaverScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiNaverNaverScraperHealthCheckRequest struct via the builder pattern


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


## NaverNaverScraperHealthCheckHead

> interface{} NaverNaverScraperHealthCheckHead(ctx).Execute()

Naver scraper health check



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
	resp, r, err := apiClient.NaverAPI.NaverNaverScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NaverAPI.NaverNaverScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `NaverNaverScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `NaverAPI.NaverNaverScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiNaverNaverScraperHealthCheckHeadRequest struct via the builder pattern


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


## NaverNaverShoppingBestsellerRankings

> interface{} NaverNaverShoppingBestsellerRankings(ctx).CategoryId(categoryId).AgeType(ageType).SortType(sortType).PeriodType(periodType).Execute()

Naver Shopping bestseller rankings



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
	categoryId := "categoryId_example" // string | Naver shopping category id, or ALL (optional) (default to "ALL")
	ageType := "ageType_example" // string | ALL | MEN_20 | WOMEN_20 | ... (optional) (default to "ALL")
	sortType := "sortType_example" // string | PRODUCT_CLICK | PRODUCT_BUY (optional) (default to "PRODUCT_CLICK")
	periodType := "periodType_example" // string | DAILY | WEEKLY (optional) (default to "DAILY")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NaverAPI.NaverNaverShoppingBestsellerRankings(context.Background()).CategoryId(categoryId).AgeType(ageType).SortType(sortType).PeriodType(periodType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NaverAPI.NaverNaverShoppingBestsellerRankings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `NaverNaverShoppingBestsellerRankings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `NaverAPI.NaverNaverShoppingBestsellerRankings`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiNaverNaverShoppingBestsellerRankingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **categoryId** | **string** | Naver shopping category id, or ALL | [default to &quot;ALL&quot;]
 **ageType** | **string** | ALL | MEN_20 | WOMEN_20 | ... | [default to &quot;ALL&quot;]
 **sortType** | **string** | PRODUCT_CLICK | PRODUCT_BUY | [default to &quot;PRODUCT_CLICK&quot;]
 **periodType** | **string** | DAILY | WEEKLY | [default to &quot;DAILY&quot;]

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


## NaverNaverShoppingCategoryReference

> interface{} NaverNaverShoppingCategoryReference(ctx).Execute()

Naver Shopping category reference



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
	resp, r, err := apiClient.NaverAPI.NaverNaverShoppingCategoryReference(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NaverAPI.NaverNaverShoppingCategoryReference``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `NaverNaverShoppingCategoryReference`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `NaverAPI.NaverNaverShoppingCategoryReference`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiNaverNaverShoppingCategoryReferenceRequest struct via the builder pattern


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


## NaverNaverShoppingTrendingKeywordRankings

> interface{} NaverNaverShoppingTrendingKeywordRankings(ctx).CategoryId(categoryId).AgeType(ageType).SortType(sortType).PeriodType(periodType).Execute()

Naver Shopping trending keyword rankings



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
	categoryId := "categoryId_example" // string | Naver shopping category id (see /shopping/categories)
	ageType := "ageType_example" // string | ALL | MEN_20 | WOMEN_20 | ... (optional) (default to "ALL")
	sortType := "sortType_example" // string |  (optional) (default to "KEYWORD_POPULAR")
	periodType := "periodType_example" // string | DAILY | WEEKLY (optional) (default to "WEEKLY")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NaverAPI.NaverNaverShoppingTrendingKeywordRankings(context.Background()).CategoryId(categoryId).AgeType(ageType).SortType(sortType).PeriodType(periodType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NaverAPI.NaverNaverShoppingTrendingKeywordRankings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `NaverNaverShoppingTrendingKeywordRankings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `NaverAPI.NaverNaverShoppingTrendingKeywordRankings`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiNaverNaverShoppingTrendingKeywordRankingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **categoryId** | **string** | Naver shopping category id (see /shopping/categories) | 
 **ageType** | **string** | ALL | MEN_20 | WOMEN_20 | ... | [default to &quot;ALL&quot;]
 **sortType** | **string** |  | [default to &quot;KEYWORD_POPULAR&quot;]
 **periodType** | **string** | DAILY | WEEKLY | [default to &quot;WEEKLY&quot;]

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


## NaverNaverWebSearch

> interface{} NaverNaverWebSearch(ctx).Query(query).Page(page).Execute()

Naver web search



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
	query := "query_example" // string | 검색어, e.g. '성남 카페'
	page := int32(56) // int32 | Result page (optional) (default to 1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NaverAPI.NaverNaverWebSearch(context.Background()).Query(query).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NaverAPI.NaverNaverWebSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `NaverNaverWebSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `NaverAPI.NaverNaverWebSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiNaverNaverWebSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | 검색어, e.g. &#39;성남 카페&#39; | 
 **page** | **int32** | Result page | [default to 1]

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


## NaverSearchSuggestions

> interface{} NaverSearchSuggestions(ctx).Query(query).Execute()

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
	query := "query_example" // string | Partial search term

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NaverAPI.NaverSearchSuggestions(context.Background()).Query(query).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NaverAPI.NaverSearchSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `NaverSearchSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `NaverAPI.NaverSearchSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiNaverSearchSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Partial search term | 

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


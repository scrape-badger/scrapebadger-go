# \LeboncoinAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**LeboncoinGetASellerSAds**](LeboncoinAPI.md#LeboncoinGetASellerSAds) | **Get** /v1/leboncoin/sellers/{user_id}/listings | Get a seller&#39;s ads
[**LeboncoinGetAdDetail**](LeboncoinAPI.md#LeboncoinGetAdDetail) | **Get** /v1/leboncoin/ads/{list_id} | Get ad detail
[**LeboncoinGetSellerProfile**](LeboncoinAPI.md#LeboncoinGetSellerProfile) | **Get** /v1/leboncoin/sellers/{user_id} | Get seller profile
[**LeboncoinGetSimilarAds**](LeboncoinAPI.md#LeboncoinGetSimilarAds) | **Get** /v1/leboncoin/ads/{list_id}/similar | Get similar ads
[**LeboncoinLeboncoinScraperHealthCheck**](LeboncoinAPI.md#LeboncoinLeboncoinScraperHealthCheck) | **Get** /v1/leboncoin/health | Leboncoin scraper health check
[**LeboncoinLeboncoinScraperHealthCheckHead**](LeboncoinAPI.md#LeboncoinLeboncoinScraperHealthCheckHead) | **Head** /v1/leboncoin/health | Leboncoin scraper health check
[**LeboncoinListCategories**](LeboncoinAPI.md#LeboncoinListCategories) | **Get** /v1/leboncoin/categories | List categories
[**LeboncoinListDepartments**](LeboncoinAPI.md#LeboncoinListDepartments) | **Get** /v1/leboncoin/departments | List departments
[**LeboncoinListMarkets**](LeboncoinAPI.md#LeboncoinListMarkets) | **Get** /v1/leboncoin/markets | List markets
[**LeboncoinListRegions**](LeboncoinAPI.md#LeboncoinListRegions) | **Get** /v1/leboncoin/regions | List regions
[**LeboncoinLocationAutocomplete**](LeboncoinAPI.md#LeboncoinLocationAutocomplete) | **Get** /v1/leboncoin/locations/search | Location autocomplete
[**LeboncoinSearchLeboncoinAds**](LeboncoinAPI.md#LeboncoinSearchLeboncoinAds) | **Get** /v1/leboncoin/search | Search Leboncoin ads



## LeboncoinGetASellerSAds

> interface{} LeboncoinGetASellerSAds(ctx, userId).Page(page).Limit(limit).Execute()

Get a seller's ads



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
	userId := "userId_example" // string | 
	page := int32(56) // int32 |  (optional) (default to 1)
	limit := int32(56) // int32 |  (optional) (default to 35)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LeboncoinAPI.LeboncoinGetASellerSAds(context.Background(), userId).Page(page).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LeboncoinAPI.LeboncoinGetASellerSAds``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LeboncoinGetASellerSAds`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LeboncoinAPI.LeboncoinGetASellerSAds`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiLeboncoinGetASellerSAdsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** |  | [default to 1]
 **limit** | **int32** |  | [default to 35]

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


## LeboncoinGetAdDetail

> interface{} LeboncoinGetAdDetail(ctx, listId).Execute()

Get ad detail



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
	listId := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LeboncoinAPI.LeboncoinGetAdDetail(context.Background(), listId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LeboncoinAPI.LeboncoinGetAdDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LeboncoinGetAdDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LeboncoinAPI.LeboncoinGetAdDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiLeboncoinGetAdDetailRequest struct via the builder pattern


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


## LeboncoinGetSellerProfile

> interface{} LeboncoinGetSellerProfile(ctx, userId).Execute()

Get seller profile



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
	userId := "userId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LeboncoinAPI.LeboncoinGetSellerProfile(context.Background(), userId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LeboncoinAPI.LeboncoinGetSellerProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LeboncoinGetSellerProfile`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LeboncoinAPI.LeboncoinGetSellerProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiLeboncoinGetSellerProfileRequest struct via the builder pattern


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


## LeboncoinGetSimilarAds

> interface{} LeboncoinGetSimilarAds(ctx, listId).Limit(limit).Execute()

Get similar ads



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
	listId := int32(56) // int32 | 
	limit := int32(56) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LeboncoinAPI.LeboncoinGetSimilarAds(context.Background(), listId).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LeboncoinAPI.LeboncoinGetSimilarAds``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LeboncoinGetSimilarAds`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LeboncoinAPI.LeboncoinGetSimilarAds`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiLeboncoinGetSimilarAdsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int32** |  | [default to 20]

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


## LeboncoinLeboncoinScraperHealthCheck

> interface{} LeboncoinLeboncoinScraperHealthCheck(ctx).Execute()

Leboncoin scraper health check



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
	resp, r, err := apiClient.LeboncoinAPI.LeboncoinLeboncoinScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LeboncoinAPI.LeboncoinLeboncoinScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LeboncoinLeboncoinScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LeboncoinAPI.LeboncoinLeboncoinScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiLeboncoinLeboncoinScraperHealthCheckRequest struct via the builder pattern


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


## LeboncoinLeboncoinScraperHealthCheckHead

> interface{} LeboncoinLeboncoinScraperHealthCheckHead(ctx).Execute()

Leboncoin scraper health check



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
	resp, r, err := apiClient.LeboncoinAPI.LeboncoinLeboncoinScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LeboncoinAPI.LeboncoinLeboncoinScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LeboncoinLeboncoinScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LeboncoinAPI.LeboncoinLeboncoinScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiLeboncoinLeboncoinScraperHealthCheckHeadRequest struct via the builder pattern


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


## LeboncoinListCategories

> interface{} LeboncoinListCategories(ctx).Execute()

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LeboncoinAPI.LeboncoinListCategories(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LeboncoinAPI.LeboncoinListCategories``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LeboncoinListCategories`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LeboncoinAPI.LeboncoinListCategories`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiLeboncoinListCategoriesRequest struct via the builder pattern


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


## LeboncoinListDepartments

> interface{} LeboncoinListDepartments(ctx).RegionId(regionId).Execute()

List departments

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
	regionId := "regionId_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LeboncoinAPI.LeboncoinListDepartments(context.Background()).RegionId(regionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LeboncoinAPI.LeboncoinListDepartments``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LeboncoinListDepartments`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LeboncoinAPI.LeboncoinListDepartments`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiLeboncoinListDepartmentsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **regionId** | **string** |  | 

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


## LeboncoinListMarkets

> interface{} LeboncoinListMarkets(ctx).Execute()

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
	resp, r, err := apiClient.LeboncoinAPI.LeboncoinListMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LeboncoinAPI.LeboncoinListMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LeboncoinListMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LeboncoinAPI.LeboncoinListMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiLeboncoinListMarketsRequest struct via the builder pattern


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


## LeboncoinListRegions

> interface{} LeboncoinListRegions(ctx).Execute()

List regions

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
	resp, r, err := apiClient.LeboncoinAPI.LeboncoinListRegions(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LeboncoinAPI.LeboncoinListRegions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LeboncoinListRegions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LeboncoinAPI.LeboncoinListRegions`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiLeboncoinListRegionsRequest struct via the builder pattern


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


## LeboncoinLocationAutocomplete

> interface{} LeboncoinLocationAutocomplete(ctx).Q(q).Execute()

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
	q := "q_example" // string | Place name

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LeboncoinAPI.LeboncoinLocationAutocomplete(context.Background()).Q(q).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LeboncoinAPI.LeboncoinLocationAutocomplete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LeboncoinLocationAutocomplete`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LeboncoinAPI.LeboncoinLocationAutocomplete`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiLeboncoinLocationAutocompleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Place name | 

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


## LeboncoinSearchLeboncoinAds

> interface{} LeboncoinSearchLeboncoinAds(ctx).Text(text).Category(category).RegionId(regionId).DepartmentId(departmentId).City(city).Zipcode(zipcode).PriceMin(priceMin).PriceMax(priceMax).OwnerType(ownerType).AdType(adType).Sort(sort).Page(page).Limit(limit).Execute()

Search Leboncoin ads



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
	text := "text_example" // string | Free-text query (optional)
	category := "category_example" // string | Category id (see /categories) (optional)
	regionId := "regionId_example" // string | Region id (see /regions) (optional)
	departmentId := "departmentId_example" // string | Department id, e.g. 75 (optional)
	city := "city_example" // string |  (optional)
	zipcode := "zipcode_example" // string |  (optional)
	priceMin := int32(56) // int32 |  (optional)
	priceMax := int32(56) // int32 |  (optional)
	ownerType := "ownerType_example" // string | all | pro | private (optional) (default to "all")
	adType := "adType_example" // string | offer | demand (optional) (default to "offer")
	sort := "sort_example" // string | relevance|newest|oldest|price_low|price_high (optional) (default to "relevance")
	page := int32(56) // int32 |  (optional) (default to 1)
	limit := int32(56) // int32 |  (optional) (default to 35)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LeboncoinAPI.LeboncoinSearchLeboncoinAds(context.Background()).Text(text).Category(category).RegionId(regionId).DepartmentId(departmentId).City(city).Zipcode(zipcode).PriceMin(priceMin).PriceMax(priceMax).OwnerType(ownerType).AdType(adType).Sort(sort).Page(page).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LeboncoinAPI.LeboncoinSearchLeboncoinAds``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LeboncoinSearchLeboncoinAds`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LeboncoinAPI.LeboncoinSearchLeboncoinAds`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiLeboncoinSearchLeboncoinAdsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **text** | **string** | Free-text query | 
 **category** | **string** | Category id (see /categories) | 
 **regionId** | **string** | Region id (see /regions) | 
 **departmentId** | **string** | Department id, e.g. 75 | 
 **city** | **string** |  | 
 **zipcode** | **string** |  | 
 **priceMin** | **int32** |  | 
 **priceMax** | **int32** |  | 
 **ownerType** | **string** | all | pro | private | [default to &quot;all&quot;]
 **adType** | **string** | offer | demand | [default to &quot;offer&quot;]
 **sort** | **string** | relevance|newest|oldest|price_low|price_high | [default to &quot;relevance&quot;]
 **page** | **int32** |  | [default to 1]
 **limit** | **int32** |  | [default to 35]

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


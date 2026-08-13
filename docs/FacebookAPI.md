# \FacebookAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**FacebookBrowseAMarketplaceCategory**](FacebookAPI.md#FacebookBrowseAMarketplaceCategory) | **Get** /v1/facebook/marketplace/category/{category} | Browse a Marketplace category
[**FacebookGetAMarketplaceItem**](FacebookAPI.md#FacebookGetAMarketplaceItem) | **Get** /v1/facebook/marketplace/item/{item_id} | Get a Marketplace item
[**FacebookGetAdvertiserPageInfo**](FacebookAPI.md#FacebookGetAdvertiserPageInfo) | **Get** /v1/facebook/ads/pages/{page_id} | Get advertiser page info
[**FacebookGetAnAd**](FacebookAPI.md#FacebookGetAnAd) | **Get** /v1/facebook/ads/{ad_archive_id} | Get an ad
[**FacebookGetGroupDetail**](FacebookAPI.md#FacebookGetGroupDetail) | **Get** /v1/facebook/groups/{group_id} | Get group detail
[**FacebookGetGroupPosts**](FacebookAPI.md#FacebookGetGroupPosts) | **Get** /v1/facebook/groups/{group_id}/posts | Get group posts
[**FacebookGetPageDetail**](FacebookAPI.md#FacebookGetPageDetail) | **Get** /v1/facebook/pages/{identifier} | Get page detail
[**FacebookGetPagePosts**](FacebookAPI.md#FacebookGetPagePosts) | **Get** /v1/facebook/pages/{identifier}/posts | Get page posts
[**FacebookGetPostComments**](FacebookAPI.md#FacebookGetPostComments) | **Get** /v1/facebook/posts/{post_id}/comments | Get post comments
[**FacebookGetPostDetail**](FacebookAPI.md#FacebookGetPostDetail) | **Get** /v1/facebook/posts/{post_id} | Get post detail
[**FacebookGetProfileDetail**](FacebookAPI.md#FacebookGetProfileDetail) | **Get** /v1/facebook/profiles/{identifier} | Get profile detail
[**FacebookGetProfilePosts**](FacebookAPI.md#FacebookGetProfilePosts) | **Get** /v1/facebook/profiles/{identifier}/posts | Get profile posts
[**FacebookListCategories**](FacebookAPI.md#FacebookListCategories) | **Get** /v1/facebook/marketplace/categories | List categories
[**FacebookListLocations**](FacebookAPI.md#FacebookListLocations) | **Get** /v1/facebook/marketplace/locations | List locations
[**FacebookSearchAdvertiserPages**](FacebookAPI.md#FacebookSearchAdvertiserPages) | **Get** /v1/facebook/ads/pages/search | Search advertiser pages
[**FacebookSearchEvents**](FacebookAPI.md#FacebookSearchEvents) | **Get** /v1/facebook/search/events | Search events
[**FacebookSearchEverything**](FacebookAPI.md#FacebookSearchEverything) | **Get** /v1/facebook/search | Search everything
[**FacebookSearchGroups**](FacebookAPI.md#FacebookSearchGroups) | **Get** /v1/facebook/search/groups | Search groups
[**FacebookSearchMarketplace**](FacebookAPI.md#FacebookSearchMarketplace) | **Get** /v1/facebook/marketplace/search | Search Marketplace
[**FacebookSearchPages**](FacebookAPI.md#FacebookSearchPages) | **Get** /v1/facebook/search/pages | Search Pages
[**FacebookSearchPeople**](FacebookAPI.md#FacebookSearchPeople) | **Get** /v1/facebook/search/people | Search people
[**FacebookSearchPlaces**](FacebookAPI.md#FacebookSearchPlaces) | **Get** /v1/facebook/search/places | Search places
[**FacebookSearchPosts**](FacebookAPI.md#FacebookSearchPosts) | **Get** /v1/facebook/search/posts | Search posts
[**FacebookSearchTheAdLibrary**](FacebookAPI.md#FacebookSearchTheAdLibrary) | **Get** /v1/facebook/ads/search | Search the Ad Library



## FacebookBrowseAMarketplaceCategory

> interface{} FacebookBrowseAMarketplaceCategory(ctx, category).Location(location).MinPrice(minPrice).MaxPrice(maxPrice).SortBy(sortBy).After(after).Execute()

Browse a Marketplace category



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
	category := "category_example" // string | 
	location := "location_example" // string |  (optional) (default to "nyc")
	minPrice := int32(56) // int32 |  (optional)
	maxPrice := int32(56) // int32 |  (optional)
	sortBy := "sortBy_example" // string |  (optional)
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookBrowseAMarketplaceCategory(context.Background(), category).Location(location).MinPrice(minPrice).MaxPrice(maxPrice).SortBy(sortBy).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookBrowseAMarketplaceCategory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookBrowseAMarketplaceCategory`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookBrowseAMarketplaceCategory`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**category** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiFacebookBrowseAMarketplaceCategoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **location** | **string** |  | [default to &quot;nyc&quot;]
 **minPrice** | **int32** |  | 
 **maxPrice** | **int32** |  | 
 **sortBy** | **string** |  | 
 **after** | **string** |  | 

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


## FacebookGetAMarketplaceItem

> interface{} FacebookGetAMarketplaceItem(ctx, itemId).Execute()

Get a Marketplace item



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
	itemId := "itemId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookGetAMarketplaceItem(context.Background(), itemId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookGetAMarketplaceItem``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookGetAMarketplaceItem`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookGetAMarketplaceItem`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**itemId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiFacebookGetAMarketplaceItemRequest struct via the builder pattern


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


## FacebookGetAdvertiserPageInfo

> interface{} FacebookGetAdvertiserPageInfo(ctx, pageId).Country(country).Execute()

Get advertiser page info



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
	pageId := "pageId_example" // string | 
	country := "country_example" // string |  (optional) (default to "US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookGetAdvertiserPageInfo(context.Background(), pageId).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookGetAdvertiserPageInfo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookGetAdvertiserPageInfo`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookGetAdvertiserPageInfo`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**pageId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiFacebookGetAdvertiserPageInfoRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** |  | [default to &quot;US&quot;]

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


## FacebookGetAnAd

> interface{} FacebookGetAnAd(ctx, adArchiveId).Country(country).Execute()

Get an ad



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
	adArchiveId := "adArchiveId_example" // string | 
	country := "country_example" // string | ISO country code (an EU code returns EU transparency) (optional) (default to "US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookGetAnAd(context.Background(), adArchiveId).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookGetAnAd``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookGetAnAd`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookGetAnAd`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**adArchiveId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiFacebookGetAnAdRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | ISO country code (an EU code returns EU transparency) | [default to &quot;US&quot;]

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


## FacebookGetGroupDetail

> interface{} FacebookGetGroupDetail(ctx, groupId).Execute()

Get group detail



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
	groupId := "groupId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookGetGroupDetail(context.Background(), groupId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookGetGroupDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookGetGroupDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookGetGroupDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**groupId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiFacebookGetGroupDetailRequest struct via the builder pattern


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


## FacebookGetGroupPosts

> interface{} FacebookGetGroupPosts(ctx, groupId).After(after).Execute()

Get group posts



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
	groupId := "groupId_example" // string | 
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookGetGroupPosts(context.Background(), groupId).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookGetGroupPosts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookGetGroupPosts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookGetGroupPosts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**groupId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiFacebookGetGroupPostsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **after** | **string** |  | 

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


## FacebookGetPageDetail

> interface{} FacebookGetPageDetail(ctx, identifier).Execute()

Get page detail



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
	identifier := "identifier_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookGetPageDetail(context.Background(), identifier).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookGetPageDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookGetPageDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookGetPageDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**identifier** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiFacebookGetPageDetailRequest struct via the builder pattern


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


## FacebookGetPagePosts

> interface{} FacebookGetPagePosts(ctx, identifier).After(after).Execute()

Get page posts



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
	identifier := "identifier_example" // string | 
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookGetPagePosts(context.Background(), identifier).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookGetPagePosts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookGetPagePosts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookGetPagePosts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**identifier** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiFacebookGetPagePostsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **after** | **string** |  | 

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


## FacebookGetPostComments

> interface{} FacebookGetPostComments(ctx, postId).After(after).Sort(sort).Execute()

Get post comments



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
	postId := "postId_example" // string | 
	after := "after_example" // string |  (optional)
	sort := "sort_example" // string |  (optional) (default to "relevance")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookGetPostComments(context.Background(), postId).After(after).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookGetPostComments``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookGetPostComments`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookGetPostComments`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**postId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiFacebookGetPostCommentsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **after** | **string** |  | 
 **sort** | **string** |  | [default to &quot;relevance&quot;]

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


## FacebookGetPostDetail

> interface{} FacebookGetPostDetail(ctx, postId).Execute()

Get post detail



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
	postId := "postId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookGetPostDetail(context.Background(), postId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookGetPostDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookGetPostDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookGetPostDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**postId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiFacebookGetPostDetailRequest struct via the builder pattern


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


## FacebookGetProfileDetail

> interface{} FacebookGetProfileDetail(ctx, identifier).Execute()

Get profile detail



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
	identifier := "identifier_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookGetProfileDetail(context.Background(), identifier).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookGetProfileDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookGetProfileDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookGetProfileDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**identifier** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiFacebookGetProfileDetailRequest struct via the builder pattern


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


## FacebookGetProfilePosts

> interface{} FacebookGetProfilePosts(ctx, identifier).After(after).Execute()

Get profile posts



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
	identifier := "identifier_example" // string | 
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookGetProfilePosts(context.Background(), identifier).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookGetProfilePosts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookGetProfilePosts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookGetProfilePosts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**identifier** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiFacebookGetProfilePostsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **after** | **string** |  | 

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


## FacebookListCategories

> interface{} FacebookListCategories(ctx).Execute()

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
	resp, r, err := apiClient.FacebookAPI.FacebookListCategories(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookListCategories``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookListCategories`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookListCategories`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiFacebookListCategoriesRequest struct via the builder pattern


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


## FacebookListLocations

> interface{} FacebookListLocations(ctx).Execute()

List locations



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
	resp, r, err := apiClient.FacebookAPI.FacebookListLocations(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookListLocations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookListLocations`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookListLocations`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiFacebookListLocationsRequest struct via the builder pattern


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


## FacebookSearchAdvertiserPages

> interface{} FacebookSearchAdvertiserPages(ctx).Query(query).Country(country).Execute()

Search advertiser pages



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
	query := "query_example" // string | Advertiser name or keyword
	country := "country_example" // string |  (optional) (default to "US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookSearchAdvertiserPages(context.Background()).Query(query).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookSearchAdvertiserPages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookSearchAdvertiserPages`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookSearchAdvertiserPages`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiFacebookSearchAdvertiserPagesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Advertiser name or keyword | 
 **country** | **string** |  | [default to &quot;US&quot;]

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


## FacebookSearchEvents

> interface{} FacebookSearchEvents(ctx).Q(q).After(after).Execute()

Search events



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
	q := "q_example" // string | 
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookSearchEvents(context.Background()).Q(q).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookSearchEvents``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookSearchEvents`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookSearchEvents`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiFacebookSearchEventsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** |  | 
 **after** | **string** |  | 

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


## FacebookSearchEverything

> interface{} FacebookSearchEverything(ctx).Q(q).After(after).Execute()

Search everything



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
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookSearchEverything(context.Background()).Q(q).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookSearchEverything``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookSearchEverything`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookSearchEverything`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiFacebookSearchEverythingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search query | 
 **after** | **string** |  | 

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


## FacebookSearchGroups

> interface{} FacebookSearchGroups(ctx).Q(q).After(after).Execute()

Search groups



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
	q := "q_example" // string | 
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookSearchGroups(context.Background()).Q(q).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookSearchGroups``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookSearchGroups`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookSearchGroups`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiFacebookSearchGroupsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** |  | 
 **after** | **string** |  | 

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


## FacebookSearchMarketplace

> interface{} FacebookSearchMarketplace(ctx).Query(query).Location(location).MinPrice(minPrice).MaxPrice(maxPrice).DaysSinceListed(daysSinceListed).SortBy(sortBy).ItemCondition(itemCondition).DeliveryMethod(deliveryMethod).After(after).Execute()

Search Marketplace



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
	query := "query_example" // string | Search keywords
	location := "location_example" // string | Marketplace location slug (optional) (default to "nyc")
	minPrice := int32(56) // int32 |  (optional)
	maxPrice := int32(56) // int32 |  (optional)
	daysSinceListed := int32(56) // int32 |  (optional)
	sortBy := "sortBy_example" // string |  (optional)
	itemCondition := "itemCondition_example" // string |  (optional)
	deliveryMethod := "deliveryMethod_example" // string |  (optional)
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookSearchMarketplace(context.Background()).Query(query).Location(location).MinPrice(minPrice).MaxPrice(maxPrice).DaysSinceListed(daysSinceListed).SortBy(sortBy).ItemCondition(itemCondition).DeliveryMethod(deliveryMethod).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookSearchMarketplace``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookSearchMarketplace`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookSearchMarketplace`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiFacebookSearchMarketplaceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords | 
 **location** | **string** | Marketplace location slug | [default to &quot;nyc&quot;]
 **minPrice** | **int32** |  | 
 **maxPrice** | **int32** |  | 
 **daysSinceListed** | **int32** |  | 
 **sortBy** | **string** |  | 
 **itemCondition** | **string** |  | 
 **deliveryMethod** | **string** |  | 
 **after** | **string** |  | 

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


## FacebookSearchPages

> interface{} FacebookSearchPages(ctx).Q(q).After(after).Execute()

Search Pages



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
	q := "q_example" // string | 
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookSearchPages(context.Background()).Q(q).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookSearchPages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookSearchPages`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookSearchPages`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiFacebookSearchPagesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** |  | 
 **after** | **string** |  | 

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


## FacebookSearchPeople

> interface{} FacebookSearchPeople(ctx).Q(q).After(after).Execute()

Search people



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
	q := "q_example" // string | 
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookSearchPeople(context.Background()).Q(q).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookSearchPeople``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookSearchPeople`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookSearchPeople`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiFacebookSearchPeopleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** |  | 
 **after** | **string** |  | 

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


## FacebookSearchPlaces

> interface{} FacebookSearchPlaces(ctx).Q(q).After(after).Execute()

Search places



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
	q := "q_example" // string | 
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookSearchPlaces(context.Background()).Q(q).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookSearchPlaces``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookSearchPlaces`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookSearchPlaces`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiFacebookSearchPlacesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** |  | 
 **after** | **string** |  | 

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


## FacebookSearchPosts

> interface{} FacebookSearchPosts(ctx).Q(q).After(after).Execute()

Search posts



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
	q := "q_example" // string | 
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookSearchPosts(context.Background()).Q(q).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookSearchPosts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookSearchPosts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookSearchPosts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiFacebookSearchPostsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** |  | 
 **after** | **string** |  | 

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


## FacebookSearchTheAdLibrary

> interface{} FacebookSearchTheAdLibrary(ctx).Query(query).Country(country).AdType(adType).ActiveStatus(activeStatus).After(after).Execute()

Search the Ad Library



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
	query := "query_example" // string | Advertiser or keyword
	country := "country_example" // string |  (optional) (default to "US")
	adType := "adType_example" // string |  (optional) (default to "all")
	activeStatus := "activeStatus_example" // string |  (optional) (default to "active")
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FacebookAPI.FacebookSearchTheAdLibrary(context.Background()).Query(query).Country(country).AdType(adType).ActiveStatus(activeStatus).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FacebookAPI.FacebookSearchTheAdLibrary``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FacebookSearchTheAdLibrary`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `FacebookAPI.FacebookSearchTheAdLibrary`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiFacebookSearchTheAdLibraryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Advertiser or keyword | 
 **country** | **string** |  | [default to &quot;US&quot;]
 **adType** | **string** |  | [default to &quot;all&quot;]
 **activeStatus** | **string** |  | [default to &quot;active&quot;]
 **after** | **string** |  | 

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


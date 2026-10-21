# \InstagramAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**InstagramAboutThisAccount**](InstagramAPI.md#InstagramAboutThisAccount) | **Get** /v1/instagram/users/{username}/about | About this account
[**InstagramBlendedTopSearch**](InstagramAPI.md#InstagramBlendedTopSearch) | **Get** /v1/instagram/search/top | Blended top search
[**InstagramGetActiveStories**](InstagramAPI.md#InstagramGetActiveStories) | **Get** /v1/instagram/users/{username}/stories | Get active stories
[**InstagramGetAudioTrack**](InstagramAPI.md#InstagramGetAudioTrack) | **Get** /v1/instagram/audio/{audio_id} | Get audio track
[**InstagramGetComments**](InstagramAPI.md#InstagramGetComments) | **Get** /v1/instagram/media/{code}/comments | Get comments
[**InstagramGetFollowers**](InstagramAPI.md#InstagramGetFollowers) | **Get** /v1/instagram/users/{username}/followers | Get followers
[**InstagramGetFollowing**](InstagramAPI.md#InstagramGetFollowing) | **Get** /v1/instagram/users/{username}/following | Get following
[**InstagramGetHashtagInfo**](InstagramAPI.md#InstagramGetHashtagInfo) | **Get** /v1/instagram/hashtags/{tag} | Get hashtag info
[**InstagramGetHighlights**](InstagramAPI.md#InstagramGetHighlights) | **Get** /v1/instagram/users/{username}/highlights | Get highlights
[**InstagramGetLikers**](InstagramAPI.md#InstagramGetLikers) | **Get** /v1/instagram/media/{code}/likers | Get likers
[**InstagramGetLocation**](InstagramAPI.md#InstagramGetLocation) | **Get** /v1/instagram/locations/{location_pk} | Get location
[**InstagramGetPostReelDetail**](InstagramAPI.md#InstagramGetPostReelDetail) | **Get** /v1/instagram/media/{code} | Get post/reel detail
[**InstagramGetProfile**](InstagramAPI.md#InstagramGetProfile) | **Get** /v1/instagram/users/{username} | Get profile
[**InstagramGetTaggedPosts**](InstagramAPI.md#InstagramGetTaggedPosts) | **Get** /v1/instagram/users/{username}/tagged | Get tagged posts
[**InstagramGetUserPosts**](InstagramAPI.md#InstagramGetUserPosts) | **Get** /v1/instagram/users/{username}/posts | Get user posts
[**InstagramGetUserReels**](InstagramAPI.md#InstagramGetUserReels) | **Get** /v1/instagram/users/{username}/reels | Get user reels
[**InstagramHealth**](InstagramAPI.md#InstagramHealth) | **Get** /v1/instagram/health | Health
[**InstagramHealthHead**](InstagramAPI.md#InstagramHealthHead) | **Head** /v1/instagram/health | Health
[**InstagramRecentHashtagPosts**](InstagramAPI.md#InstagramRecentHashtagPosts) | **Get** /v1/instagram/hashtags/{tag}/recent | Recent hashtag posts
[**InstagramRelatedProfiles**](InstagramAPI.md#InstagramRelatedProfiles) | **Get** /v1/instagram/users/{username}/related | Related profiles
[**InstagramSearchHashtags**](InstagramAPI.md#InstagramSearchHashtags) | **Get** /v1/instagram/search/hashtags | Search hashtags
[**InstagramSearchUsers**](InstagramAPI.md#InstagramSearchUsers) | **Get** /v1/instagram/search/users | Search users
[**InstagramTopHashtagPosts**](InstagramAPI.md#InstagramTopHashtagPosts) | **Get** /v1/instagram/hashtags/{tag}/top | Top hashtag posts



## InstagramAboutThisAccount

> interface{} InstagramAboutThisAccount(ctx, username).Execute()

About this account



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
	username := "username_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramAboutThisAccount(context.Background(), username).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramAboutThisAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramAboutThisAccount`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramAboutThisAccount`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramAboutThisAccountRequest struct via the builder pattern


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


## InstagramBlendedTopSearch

> interface{} InstagramBlendedTopSearch(ctx).Query(query).Execute()

Blended top search

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
	query := "query_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramBlendedTopSearch(context.Background()).Query(query).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramBlendedTopSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramBlendedTopSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramBlendedTopSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiInstagramBlendedTopSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 

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


## InstagramGetActiveStories

> interface{} InstagramGetActiveStories(ctx, username).Execute()

Get active stories



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
	username := "username_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramGetActiveStories(context.Background(), username).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramGetActiveStories``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramGetActiveStories`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramGetActiveStories`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramGetActiveStoriesRequest struct via the builder pattern


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


## InstagramGetAudioTrack

> interface{} InstagramGetAudioTrack(ctx, audioId).Execute()

Get audio track

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
	audioId := "audioId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramGetAudioTrack(context.Background(), audioId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramGetAudioTrack``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramGetAudioTrack`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramGetAudioTrack`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**audioId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramGetAudioTrackRequest struct via the builder pattern


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


## InstagramGetComments

> interface{} InstagramGetComments(ctx, code).Amount(amount).Cursor(cursor).Execute()

Get comments

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
	code := "code_example" // string | 
	amount := int32(56) // int32 |  (optional) (default to 20)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramGetComments(context.Background(), code).Amount(amount).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramGetComments``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramGetComments`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramGetComments`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**code** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramGetCommentsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **amount** | **int32** |  | [default to 20]
 **cursor** | **string** |  | 

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


## InstagramGetFollowers

> interface{} InstagramGetFollowers(ctx, username).Amount(amount).Cursor(cursor).Order(order).Execute()

Get followers



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
	username := "username_example" // string | 
	amount := int32(56) // int32 |  (optional) (default to 50)
	cursor := "cursor_example" // string |  (optional)
	order := "order_example" // string | date_followed_latest | date_followed_earliest (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramGetFollowers(context.Background(), username).Amount(amount).Cursor(cursor).Order(order).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramGetFollowers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramGetFollowers`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramGetFollowers`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramGetFollowersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **amount** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 
 **order** | **string** | date_followed_latest | date_followed_earliest | 

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


## InstagramGetFollowing

> interface{} InstagramGetFollowing(ctx, username).Amount(amount).Cursor(cursor).Execute()

Get following

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
	username := "username_example" // string | 
	amount := int32(56) // int32 |  (optional) (default to 50)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramGetFollowing(context.Background(), username).Amount(amount).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramGetFollowing``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramGetFollowing`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramGetFollowing`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramGetFollowingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **amount** | **int32** |  | [default to 50]
 **cursor** | **string** |  | 

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


## InstagramGetHashtagInfo

> interface{} InstagramGetHashtagInfo(ctx, tag).Execute()

Get hashtag info

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
	tag := "tag_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramGetHashtagInfo(context.Background(), tag).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramGetHashtagInfo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramGetHashtagInfo`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramGetHashtagInfo`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tag** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramGetHashtagInfoRequest struct via the builder pattern


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


## InstagramGetHighlights

> interface{} InstagramGetHighlights(ctx, username).Execute()

Get highlights

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
	username := "username_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramGetHighlights(context.Background(), username).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramGetHighlights``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramGetHighlights`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramGetHighlights`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramGetHighlightsRequest struct via the builder pattern


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


## InstagramGetLikers

> interface{} InstagramGetLikers(ctx, code).Execute()

Get likers

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
	code := "code_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramGetLikers(context.Background(), code).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramGetLikers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramGetLikers`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramGetLikers`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**code** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramGetLikersRequest struct via the builder pattern


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


## InstagramGetLocation

> interface{} InstagramGetLocation(ctx, locationPk).Execute()

Get location

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
	locationPk := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramGetLocation(context.Background(), locationPk).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramGetLocation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramGetLocation`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramGetLocation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**locationPk** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramGetLocationRequest struct via the builder pattern


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


## InstagramGetPostReelDetail

> interface{} InstagramGetPostReelDetail(ctx, code).Execute()

Get post/reel detail



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
	code := "code_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramGetPostReelDetail(context.Background(), code).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramGetPostReelDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramGetPostReelDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramGetPostReelDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**code** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramGetPostReelDetailRequest struct via the builder pattern


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


## InstagramGetProfile

> interface{} InstagramGetProfile(ctx, username).Execute()

Get profile



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
	username := "username_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramGetProfile(context.Background(), username).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramGetProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramGetProfile`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramGetProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramGetProfileRequest struct via the builder pattern


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


## InstagramGetTaggedPosts

> interface{} InstagramGetTaggedPosts(ctx, username).Amount(amount).Cursor(cursor).Execute()

Get tagged posts

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
	username := "username_example" // string | 
	amount := int32(56) // int32 |  (optional) (default to 20)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramGetTaggedPosts(context.Background(), username).Amount(amount).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramGetTaggedPosts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramGetTaggedPosts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramGetTaggedPosts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramGetTaggedPostsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **amount** | **int32** |  | [default to 20]
 **cursor** | **string** |  | 

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


## InstagramGetUserPosts

> interface{} InstagramGetUserPosts(ctx, username).Amount(amount).Cursor(cursor).Execute()

Get user posts



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
	username := "username_example" // string | 
	amount := int32(56) // int32 |  (optional) (default to 20)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramGetUserPosts(context.Background(), username).Amount(amount).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramGetUserPosts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramGetUserPosts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramGetUserPosts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramGetUserPostsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **amount** | **int32** |  | [default to 20]
 **cursor** | **string** |  | 

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


## InstagramGetUserReels

> interface{} InstagramGetUserReels(ctx, username).Amount(amount).Cursor(cursor).Execute()

Get user reels

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
	username := "username_example" // string | 
	amount := int32(56) // int32 |  (optional) (default to 20)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramGetUserReels(context.Background(), username).Amount(amount).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramGetUserReels``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramGetUserReels`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramGetUserReels`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramGetUserReelsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **amount** | **int32** |  | [default to 20]
 **cursor** | **string** |  | 

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


## InstagramHealth

> interface{} InstagramHealth(ctx).Execute()

Health

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
	resp, r, err := apiClient.InstagramAPI.InstagramHealth(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramHealth``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramHealth`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramHealth`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramHealthRequest struct via the builder pattern


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


## InstagramHealthHead

> interface{} InstagramHealthHead(ctx).Execute()

Health

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
	resp, r, err := apiClient.InstagramAPI.InstagramHealthHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramHealthHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramHealthHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramHealthHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramHealthHeadRequest struct via the builder pattern


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


## InstagramRecentHashtagPosts

> interface{} InstagramRecentHashtagPosts(ctx, tag).Amount(amount).Cursor(cursor).Execute()

Recent hashtag posts

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
	tag := "tag_example" // string | 
	amount := int32(56) // int32 |  (optional) (default to 20)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramRecentHashtagPosts(context.Background(), tag).Amount(amount).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramRecentHashtagPosts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramRecentHashtagPosts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramRecentHashtagPosts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tag** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramRecentHashtagPostsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **amount** | **int32** |  | [default to 20]
 **cursor** | **string** |  | 

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


## InstagramRelatedProfiles

> interface{} InstagramRelatedProfiles(ctx, username).Execute()

Related profiles

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
	username := "username_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramRelatedProfiles(context.Background(), username).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramRelatedProfiles``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramRelatedProfiles`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramRelatedProfiles`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramRelatedProfilesRequest struct via the builder pattern


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


## InstagramSearchHashtags

> interface{} InstagramSearchHashtags(ctx).Query(query).Execute()

Search hashtags

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
	query := "query_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramSearchHashtags(context.Background()).Query(query).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramSearchHashtags``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramSearchHashtags`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramSearchHashtags`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiInstagramSearchHashtagsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 

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


## InstagramSearchUsers

> interface{} InstagramSearchUsers(ctx).Query(query).Execute()

Search users

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
	query := "query_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramSearchUsers(context.Background()).Query(query).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramSearchUsers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramSearchUsers`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramSearchUsers`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiInstagramSearchUsersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 

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


## InstagramTopHashtagPosts

> interface{} InstagramTopHashtagPosts(ctx, tag).Amount(amount).Cursor(cursor).Execute()

Top hashtag posts

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
	tag := "tag_example" // string | 
	amount := int32(56) // int32 |  (optional) (default to 20)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InstagramAPI.InstagramTopHashtagPosts(context.Background(), tag).Amount(amount).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InstagramAPI.InstagramTopHashtagPosts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InstagramTopHashtagPosts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `InstagramAPI.InstagramTopHashtagPosts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tag** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstagramTopHashtagPostsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **amount** | **int32** |  | [default to 20]
 **cursor** | **string** |  | 

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


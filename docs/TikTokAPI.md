# \TikTokAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**TiktokGeneralSearch**](TikTokAPI.md#TiktokGeneralSearch) | **Get** /v1/tiktok/search | General search
[**TiktokGetCommentReplies**](TikTokAPI.md#TiktokGetCommentReplies) | **Get** /v1/tiktok/comments/{comment_id}/replies | Get comment replies
[**TiktokGetComments**](TikTokAPI.md#TiktokGetComments) | **Get** /v1/tiktok/videos/{video_id}/comments | Get comments
[**TiktokGetFollowersDeprecated**](TikTokAPI.md#TiktokGetFollowersDeprecated) | **Get** /v1/tiktok/users/{username}/followers | Get followers (deprecated)
[**TiktokGetFollowingDeprecated**](TikTokAPI.md#TiktokGetFollowingDeprecated) | **Get** /v1/tiktok/users/{username}/following | Get following (deprecated)
[**TiktokGetHashtagDetail**](TikTokAPI.md#TiktokGetHashtagDetail) | **Get** /v1/tiktok/hashtags/{name} | Get hashtag detail
[**TiktokGetHashtagVideos**](TikTokAPI.md#TiktokGetHashtagVideos) | **Get** /v1/tiktok/hashtags/{name}/videos | Get hashtag videos
[**TiktokGetLikedVideosDeprecated**](TikTokAPI.md#TiktokGetLikedVideosDeprecated) | **Get** /v1/tiktok/users/{username}/liked | Get liked videos (deprecated)
[**TiktokGetMusicSoundDetail**](TikTokAPI.md#TiktokGetMusicSoundDetail) | **Get** /v1/tiktok/music/{music_id} | Get music/sound detail
[**TiktokGetMusicVideos**](TikTokAPI.md#TiktokGetMusicVideos) | **Get** /v1/tiktok/music/{music_id}/videos | Get music videos
[**TiktokGetOembedMetadata**](TikTokAPI.md#TiktokGetOembedMetadata) | **Get** /v1/tiktok/oembed | Get oEmbed metadata
[**TiktokGetRelatedVideos**](TikTokAPI.md#TiktokGetRelatedVideos) | **Get** /v1/tiktok/videos/{video_id}/related | Get related videos
[**TiktokGetReposts**](TikTokAPI.md#TiktokGetReposts) | **Get** /v1/tiktok/users/{username}/reposts | Get reposts
[**TiktokGetTranscript**](TikTokAPI.md#TiktokGetTranscript) | **Get** /v1/tiktok/videos/{video_id}/transcript | Get transcript
[**TiktokGetUserProfile**](TikTokAPI.md#TiktokGetUserProfile) | **Get** /v1/tiktok/users/{username} | Get user profile
[**TiktokGetUserVideos**](TikTokAPI.md#TiktokGetUserVideos) | **Get** /v1/tiktok/users/{username}/videos | Get user videos
[**TiktokGetVideoDetail**](TikTokAPI.md#TiktokGetVideoDetail) | **Get** /v1/tiktok/videos/{video_id} | Get video detail
[**TiktokHealthCheck**](TikTokAPI.md#TiktokHealthCheck) | **Get** /v1/tiktok/health | Health check
[**TiktokHealthCheckHead**](TikTokAPI.md#TiktokHealthCheckHead) | **Head** /v1/tiktok/health | Health check
[**TiktokListRegions**](TikTokAPI.md#TiktokListRegions) | **Get** /v1/tiktok/regions | List regions
[**TiktokSearchHashtags**](TikTokAPI.md#TiktokSearchHashtags) | **Get** /v1/tiktok/search/hashtags | Search hashtags
[**TiktokSearchTheTiktokAdLibrary**](TikTokAPI.md#TiktokSearchTheTiktokAdLibrary) | **Get** /v1/tiktok/ads/search | Search the TikTok Ad Library
[**TiktokSearchUsers**](TikTokAPI.md#TiktokSearchUsers) | **Get** /v1/tiktok/search/users | Search users
[**TiktokSearchVideos**](TikTokAPI.md#TiktokSearchVideos) | **Get** /v1/tiktok/search/videos | Search videos
[**TiktokTrendingHashtags**](TikTokAPI.md#TiktokTrendingHashtags) | **Get** /v1/tiktok/trending/hashtags | Trending hashtags
[**TiktokTrendingSongs**](TikTokAPI.md#TiktokTrendingSongs) | **Get** /v1/tiktok/trending/songs | Trending songs
[**TiktokTrendingVideos**](TikTokAPI.md#TiktokTrendingVideos) | **Get** /v1/tiktok/trending/videos | Trending videos



## TiktokGeneralSearch

> interface{} TiktokGeneralSearch(ctx).Query(query).Region(region).Count(count).Cursor(cursor).Execute()

General search



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
	query := "query_example" // string | Search keyword
	region := "region_example" // string |  (optional) (default to "US")
	count := int32(56) // int32 |  (optional) (default to 20)
	cursor := "cursor_example" // string | Composite pagination cursor (offset.search_id) from a prior page's pagination.cursor (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokGeneralSearch(context.Background()).Query(query).Region(region).Count(count).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokGeneralSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokGeneralSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokGeneralSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTiktokGeneralSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keyword | 
 **region** | **string** |  | [default to &quot;US&quot;]
 **count** | **int32** |  | [default to 20]
 **cursor** | **string** | Composite pagination cursor (offset.search_id) from a prior page&#39;s pagination.cursor | 

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


## TiktokGetCommentReplies

> interface{} TiktokGetCommentReplies(ctx, commentId).VideoId(videoId).Region(region).Count(count).Cursor(cursor).Execute()

Get comment replies



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
	commentId := "commentId_example" // string | 
	videoId := "videoId_example" // string | Parent video id
	region := "region_example" // string |  (optional) (default to "US")
	count := int32(56) // int32 |  (optional) (default to 20)
	cursor := "cursor_example" // string | Pagination cursor from a prior page's pagination.cursor (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokGetCommentReplies(context.Background(), commentId).VideoId(videoId).Region(region).Count(count).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokGetCommentReplies``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokGetCommentReplies`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokGetCommentReplies`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**commentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokGetCommentRepliesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **videoId** | **string** | Parent video id | 
 **region** | **string** |  | [default to &quot;US&quot;]
 **count** | **int32** |  | [default to 20]
 **cursor** | **string** | Pagination cursor from a prior page&#39;s pagination.cursor | 

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


## TiktokGetComments

> interface{} TiktokGetComments(ctx, videoId).Region(region).Count(count).Cursor(cursor).Execute()

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
	videoId := "videoId_example" // string | 
	region := "region_example" // string |  (optional) (default to "US")
	count := int32(56) // int32 |  (optional) (default to 20)
	cursor := "cursor_example" // string | Pagination cursor from a prior page's pagination.cursor (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokGetComments(context.Background(), videoId).Region(region).Count(count).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokGetComments``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokGetComments`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokGetComments`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**videoId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokGetCommentsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **region** | **string** |  | [default to &quot;US&quot;]
 **count** | **int32** |  | [default to 20]
 **cursor** | **string** | Pagination cursor from a prior page&#39;s pagination.cursor | 

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


## TiktokGetFollowersDeprecated

> interface{} TiktokGetFollowersDeprecated(ctx, username).Region(region).Count(count).Execute()

Get followers (deprecated)



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
	region := "region_example" // string |  (optional) (default to "US")
	count := int32(56) // int32 |  (optional) (default to 30)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokGetFollowersDeprecated(context.Background(), username).Region(region).Count(count).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokGetFollowersDeprecated``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokGetFollowersDeprecated`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokGetFollowersDeprecated`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokGetFollowersDeprecatedRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **region** | **string** |  | [default to &quot;US&quot;]
 **count** | **int32** |  | [default to 30]

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


## TiktokGetFollowingDeprecated

> interface{} TiktokGetFollowingDeprecated(ctx, username).Region(region).Count(count).Execute()

Get following (deprecated)



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
	region := "region_example" // string |  (optional) (default to "US")
	count := int32(56) // int32 |  (optional) (default to 30)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokGetFollowingDeprecated(context.Background(), username).Region(region).Count(count).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokGetFollowingDeprecated``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokGetFollowingDeprecated`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokGetFollowingDeprecated`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokGetFollowingDeprecatedRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **region** | **string** |  | [default to &quot;US&quot;]
 **count** | **int32** |  | [default to 30]

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


## TiktokGetHashtagDetail

> interface{} TiktokGetHashtagDetail(ctx, name).Region(region).Execute()

Get hashtag detail



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
	name := "name_example" // string | 
	region := "region_example" // string |  (optional) (default to "US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokGetHashtagDetail(context.Background(), name).Region(region).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokGetHashtagDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokGetHashtagDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokGetHashtagDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**name** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokGetHashtagDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **region** | **string** |  | [default to &quot;US&quot;]

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


## TiktokGetHashtagVideos

> interface{} TiktokGetHashtagVideos(ctx, name).Region(region).Count(count).Cursor(cursor).Execute()

Get hashtag videos



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
	name := "name_example" // string | 
	region := "region_example" // string |  (optional) (default to "US")
	count := int32(56) // int32 |  (optional) (default to 30)
	cursor := "cursor_example" // string | Pagination cursor from a prior page's pagination.cursor (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokGetHashtagVideos(context.Background(), name).Region(region).Count(count).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokGetHashtagVideos``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokGetHashtagVideos`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokGetHashtagVideos`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**name** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokGetHashtagVideosRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **region** | **string** |  | [default to &quot;US&quot;]
 **count** | **int32** |  | [default to 30]
 **cursor** | **string** | Pagination cursor from a prior page&#39;s pagination.cursor | 

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


## TiktokGetLikedVideosDeprecated

> interface{} TiktokGetLikedVideosDeprecated(ctx, username).Region(region).Count(count).Execute()

Get liked videos (deprecated)



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
	region := "region_example" // string |  (optional) (default to "US")
	count := int32(56) // int32 |  (optional) (default to 30)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokGetLikedVideosDeprecated(context.Background(), username).Region(region).Count(count).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokGetLikedVideosDeprecated``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokGetLikedVideosDeprecated`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokGetLikedVideosDeprecated`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokGetLikedVideosDeprecatedRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **region** | **string** |  | [default to &quot;US&quot;]
 **count** | **int32** |  | [default to 30]

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


## TiktokGetMusicSoundDetail

> interface{} TiktokGetMusicSoundDetail(ctx, musicId).Region(region).Execute()

Get music/sound detail



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
	musicId := "musicId_example" // string | 
	region := "region_example" // string |  (optional) (default to "US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokGetMusicSoundDetail(context.Background(), musicId).Region(region).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokGetMusicSoundDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokGetMusicSoundDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokGetMusicSoundDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**musicId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokGetMusicSoundDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **region** | **string** |  | [default to &quot;US&quot;]

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


## TiktokGetMusicVideos

> interface{} TiktokGetMusicVideos(ctx, musicId).Region(region).Count(count).Cursor(cursor).Execute()

Get music videos



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
	musicId := "musicId_example" // string | 
	region := "region_example" // string |  (optional) (default to "US")
	count := int32(56) // int32 |  (optional) (default to 30)
	cursor := "cursor_example" // string | Pagination cursor from a prior page's pagination.cursor (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokGetMusicVideos(context.Background(), musicId).Region(region).Count(count).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokGetMusicVideos``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokGetMusicVideos`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokGetMusicVideos`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**musicId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokGetMusicVideosRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **region** | **string** |  | [default to &quot;US&quot;]
 **count** | **int32** |  | [default to 30]
 **cursor** | **string** | Pagination cursor from a prior page&#39;s pagination.cursor | 

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


## TiktokGetOembedMetadata

> interface{} TiktokGetOembedMetadata(ctx).Url(url).Region(region).Execute()

Get oEmbed metadata



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
	url := "url_example" // string | Full TikTok video or profile URL
	region := "region_example" // string |  (optional) (default to "US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokGetOembedMetadata(context.Background()).Url(url).Region(region).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokGetOembedMetadata``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokGetOembedMetadata`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokGetOembedMetadata`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTiktokGetOembedMetadataRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **url** | **string** | Full TikTok video or profile URL | 
 **region** | **string** |  | [default to &quot;US&quot;]

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


## TiktokGetRelatedVideos

> interface{} TiktokGetRelatedVideos(ctx, videoId).Region(region).Count(count).Execute()

Get related videos



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
	videoId := "videoId_example" // string | 
	region := "region_example" // string |  (optional) (default to "US")
	count := int32(56) // int32 |  (optional) (default to 16)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokGetRelatedVideos(context.Background(), videoId).Region(region).Count(count).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokGetRelatedVideos``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokGetRelatedVideos`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokGetRelatedVideos`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**videoId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokGetRelatedVideosRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **region** | **string** |  | [default to &quot;US&quot;]
 **count** | **int32** |  | [default to 16]

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


## TiktokGetReposts

> interface{} TiktokGetReposts(ctx, username).Region(region).Count(count).Execute()

Get reposts



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
	region := "region_example" // string |  (optional) (default to "US")
	count := int32(56) // int32 |  (optional) (default to 30)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokGetReposts(context.Background(), username).Region(region).Count(count).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokGetReposts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokGetReposts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokGetReposts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokGetRepostsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **region** | **string** |  | [default to &quot;US&quot;]
 **count** | **int32** |  | [default to 30]

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


## TiktokGetTranscript

> interface{} TiktokGetTranscript(ctx, videoId).Region(region).Execute()

Get transcript



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
	videoId := "videoId_example" // string | 
	region := "region_example" // string |  (optional) (default to "US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokGetTranscript(context.Background(), videoId).Region(region).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokGetTranscript``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokGetTranscript`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokGetTranscript`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**videoId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokGetTranscriptRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **region** | **string** |  | [default to &quot;US&quot;]

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


## TiktokGetUserProfile

> interface{} TiktokGetUserProfile(ctx, username).Region(region).Execute()

Get user profile



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
	region := "region_example" // string | Content region (ISO 3166-1 alpha-2) (optional) (default to "US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokGetUserProfile(context.Background(), username).Region(region).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokGetUserProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokGetUserProfile`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokGetUserProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokGetUserProfileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **region** | **string** | Content region (ISO 3166-1 alpha-2) | [default to &quot;US&quot;]

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


## TiktokGetUserVideos

> interface{} TiktokGetUserVideos(ctx, username).Region(region).Count(count).Cursor(cursor).Execute()

Get user videos



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
	region := "region_example" // string |  (optional) (default to "US")
	count := int32(56) // int32 |  (optional) (default to 30)
	cursor := "cursor_example" // string | Pagination cursor from a prior page's `pagination.cursor` (signer path only). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokGetUserVideos(context.Background(), username).Region(region).Count(count).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokGetUserVideos``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokGetUserVideos`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokGetUserVideos`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokGetUserVideosRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **region** | **string** |  | [default to &quot;US&quot;]
 **count** | **int32** |  | [default to 30]
 **cursor** | **string** | Pagination cursor from a prior page&#39;s &#x60;pagination.cursor&#x60; (signer path only). | 

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


## TiktokGetVideoDetail

> interface{} TiktokGetVideoDetail(ctx, videoId).Region(region).Username(username).Execute()

Get video detail



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
	videoId := "videoId_example" // string | 
	region := "region_example" // string |  (optional) (default to "US")
	username := "username_example" // string | Author handle (skips oEmbed lookup) (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokGetVideoDetail(context.Background(), videoId).Region(region).Username(username).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokGetVideoDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokGetVideoDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokGetVideoDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**videoId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokGetVideoDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **region** | **string** |  | [default to &quot;US&quot;]
 **username** | **string** | Author handle (skips oEmbed lookup) | 

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


## TiktokHealthCheck

> interface{} TiktokHealthCheck(ctx).Execute()

Health check



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
	resp, r, err := apiClient.TikTokAPI.TiktokHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokHealthCheckRequest struct via the builder pattern


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


## TiktokHealthCheckHead

> interface{} TiktokHealthCheckHead(ctx).Execute()

Health check



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
	resp, r, err := apiClient.TikTokAPI.TiktokHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokHealthCheckHeadRequest struct via the builder pattern


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


## TiktokListRegions

> interface{} TiktokListRegions(ctx).Execute()

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
	resp, r, err := apiClient.TikTokAPI.TiktokListRegions(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokListRegions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokListRegions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokListRegions`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiTiktokListRegionsRequest struct via the builder pattern


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


## TiktokSearchHashtags

> interface{} TiktokSearchHashtags(ctx).Query(query).Region(region).Count(count).Cursor(cursor).Execute()

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
	query := "query_example" // string | Search keyword
	region := "region_example" // string |  (optional) (default to "US")
	count := int32(56) // int32 |  (optional) (default to 20)
	cursor := "cursor_example" // string | Composite pagination cursor (offset.search_id) from a prior page's pagination.cursor (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokSearchHashtags(context.Background()).Query(query).Region(region).Count(count).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokSearchHashtags``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokSearchHashtags`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokSearchHashtags`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTiktokSearchHashtagsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keyword | 
 **region** | **string** |  | [default to &quot;US&quot;]
 **count** | **int32** |  | [default to 20]
 **cursor** | **string** | Composite pagination cursor (offset.search_id) from a prior page&#39;s pagination.cursor | 

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


## TiktokSearchTheTiktokAdLibrary

> interface{} TiktokSearchTheTiktokAdLibrary(ctx).Query(query).AdvertiserId(advertiserId).Region(region).Days(days).Sort(sort).Offset(offset).SearchId(searchId).Count(count).Execute()

Search the TikTok Ad Library



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
	query := "query_example" // string | Keyword (ignored when advertiser_id is set) (optional) (default to "")
	advertiserId := "advertiserId_example" // string | Advertiser business id(s) for advertiser search (optional) (default to "")
	region := "region_example" // string | EU region code (the Ad Library is EU-only) (optional) (default to "DE")
	days := int32(56) // int32 |  (optional) (default to 30)
	sort := "sort_example" // string |  (optional) (default to "last_shown_date,desc")
	offset := int32(56) // int32 |  (optional) (default to 0)
	searchId := "searchId_example" // string |  (optional) (default to "")
	count := int32(56) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokSearchTheTiktokAdLibrary(context.Background()).Query(query).AdvertiserId(advertiserId).Region(region).Days(days).Sort(sort).Offset(offset).SearchId(searchId).Count(count).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokSearchTheTiktokAdLibrary``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokSearchTheTiktokAdLibrary`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokSearchTheTiktokAdLibrary`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTiktokSearchTheTiktokAdLibraryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Keyword (ignored when advertiser_id is set) | [default to &quot;&quot;]
 **advertiserId** | **string** | Advertiser business id(s) for advertiser search | [default to &quot;&quot;]
 **region** | **string** | EU region code (the Ad Library is EU-only) | [default to &quot;DE&quot;]
 **days** | **int32** |  | [default to 30]
 **sort** | **string** |  | [default to &quot;last_shown_date,desc&quot;]
 **offset** | **int32** |  | [default to 0]
 **searchId** | **string** |  | [default to &quot;&quot;]
 **count** | **int32** |  | [default to 20]

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


## TiktokSearchUsers

> interface{} TiktokSearchUsers(ctx).Query(query).Region(region).Count(count).Cursor(cursor).Execute()

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
	query := "query_example" // string | Search keyword
	region := "region_example" // string |  (optional) (default to "US")
	count := int32(56) // int32 |  (optional) (default to 20)
	cursor := "cursor_example" // string | Composite pagination cursor (offset.search_id) from a prior page's pagination.cursor (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokSearchUsers(context.Background()).Query(query).Region(region).Count(count).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokSearchUsers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokSearchUsers`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokSearchUsers`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTiktokSearchUsersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keyword | 
 **region** | **string** |  | [default to &quot;US&quot;]
 **count** | **int32** |  | [default to 20]
 **cursor** | **string** | Composite pagination cursor (offset.search_id) from a prior page&#39;s pagination.cursor | 

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


## TiktokSearchVideos

> interface{} TiktokSearchVideos(ctx).Query(query).Region(region).Count(count).Cursor(cursor).Execute()

Search videos



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
	query := "query_example" // string | Search keyword
	region := "region_example" // string |  (optional) (default to "US")
	count := int32(56) // int32 |  (optional) (default to 20)
	cursor := "cursor_example" // string | Composite pagination cursor (offset.search_id) from a prior page's pagination.cursor (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokSearchVideos(context.Background()).Query(query).Region(region).Count(count).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokSearchVideos``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokSearchVideos`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokSearchVideos`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTiktokSearchVideosRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keyword | 
 **region** | **string** |  | [default to &quot;US&quot;]
 **count** | **int32** |  | [default to 20]
 **cursor** | **string** | Composite pagination cursor (offset.search_id) from a prior page&#39;s pagination.cursor | 

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


## TiktokTrendingHashtags

> interface{} TiktokTrendingHashtags(ctx).Region(region).Period(period).Count(count).Execute()

Trending hashtags



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
	region := "region_example" // string |  (optional) (default to "US")
	period := int32(56) // int32 |  (optional) (default to 7)
	count := int32(56) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokTrendingHashtags(context.Background()).Region(region).Period(period).Count(count).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokTrendingHashtags``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokTrendingHashtags`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokTrendingHashtags`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTiktokTrendingHashtagsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **region** | **string** |  | [default to &quot;US&quot;]
 **period** | **int32** |  | [default to 7]
 **count** | **int32** |  | [default to 20]

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


## TiktokTrendingSongs

> interface{} TiktokTrendingSongs(ctx).Region(region).Period(period).Count(count).Execute()

Trending songs



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
	region := "region_example" // string |  (optional) (default to "US")
	period := int32(56) // int32 |  (optional) (default to 7)
	count := int32(56) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokTrendingSongs(context.Background()).Region(region).Period(period).Count(count).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokTrendingSongs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokTrendingSongs`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokTrendingSongs`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTiktokTrendingSongsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **region** | **string** |  | [default to &quot;US&quot;]
 **period** | **int32** |  | [default to 7]
 **count** | **int32** |  | [default to 20]

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


## TiktokTrendingVideos

> interface{} TiktokTrendingVideos(ctx).Region(region).Count(count).Execute()

Trending videos



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
	region := "region_example" // string |  (optional) (default to "US")
	count := int32(56) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TikTokAPI.TiktokTrendingVideos(context.Background()).Region(region).Count(count).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TikTokAPI.TiktokTrendingVideos``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TiktokTrendingVideos`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TikTokAPI.TiktokTrendingVideos`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTiktokTrendingVideosRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **region** | **string** |  | [default to &quot;US&quot;]
 **count** | **int32** |  | [default to 20]

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


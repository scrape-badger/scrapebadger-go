# \YouTubeAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**YoutubeBatchVideoDetail**](YouTubeAPI.md#YoutubeBatchVideoDetail) | **Post** /v1/youtube/videos/batch | Batch video detail
[**YoutubeChannelAbout**](YouTubeAPI.md#YoutubeChannelAbout) | **Get** /v1/youtube/channels/{channel_id}/about | Channel about
[**YoutubeChannelPlaylists**](YouTubeAPI.md#YoutubeChannelPlaylists) | **Get** /v1/youtube/channels/{channel_id}/playlists | Channel playlists
[**YoutubeChannelShorts**](YouTubeAPI.md#YoutubeChannelShorts) | **Get** /v1/youtube/channels/{channel_id}/shorts | Channel shorts
[**YoutubeChannelStreams**](YouTubeAPI.md#YoutubeChannelStreams) | **Get** /v1/youtube/channels/{channel_id}/streams | Channel streams
[**YoutubeChannelVideos**](YouTubeAPI.md#YoutubeChannelVideos) | **Get** /v1/youtube/channels/{channel_id}/videos | Channel videos
[**YoutubeCommentReplies**](YouTubeAPI.md#YoutubeCommentReplies) | **Get** /v1/youtube/videos/{video_id}/comments/{comment_id}/replies | Comment replies
[**YoutubeCommunityPostComments**](YouTubeAPI.md#YoutubeCommunityPostComments) | **Get** /v1/youtube/posts/{post_id}/comments | Community post comments
[**YoutubeCommunityPosts**](YouTubeAPI.md#YoutubeCommunityPosts) | **Get** /v1/youtube/channels/{channel_id}/community | Community posts
[**YoutubeContentRegions**](YouTubeAPI.md#YoutubeContentRegions) | **Get** /v1/youtube/regions | Content regions
[**YoutubeGetACommunityPost**](YouTubeAPI.md#YoutubeGetACommunityPost) | **Get** /v1/youtube/posts/{post_id} | Get a community post
[**YoutubeGetAMixRadioQueue**](YouTubeAPI.md#YoutubeGetAMixRadioQueue) | **Get** /v1/youtube/mixes/{playlist_id} | Get a mix / radio queue
[**YoutubeGetAShort**](YouTubeAPI.md#YoutubeGetAShort) | **Get** /v1/youtube/shorts/{video_id} | Get a Short
[**YoutubeGetChannelDetail**](YouTubeAPI.md#YoutubeGetChannelDetail) | **Get** /v1/youtube/channels/{channel_id} | Get channel detail
[**YoutubeGetPlaylistDetail**](YouTubeAPI.md#YoutubeGetPlaylistDetail) | **Get** /v1/youtube/playlists/{playlist_id} | Get playlist detail
[**YoutubeGetVideoDetail**](YouTubeAPI.md#YoutubeGetVideoDetail) | **Get** /v1/youtube/videos/{video_id} | Get video detail
[**YoutubeGuestHomeFeed**](YouTubeAPI.md#YoutubeGuestHomeFeed) | **Get** /v1/youtube/home | Guest home feed
[**YoutubeKeywordSuggestions**](YouTubeAPI.md#YoutubeKeywordSuggestions) | **Get** /v1/youtube/autocomplete | Keyword suggestions
[**YoutubeListCaptionTracks**](YouTubeAPI.md#YoutubeListCaptionTracks) | **Get** /v1/youtube/videos/{video_id}/captions | List caption tracks
[**YoutubeLiveChatMessages**](YouTubeAPI.md#YoutubeLiveChatMessages) | **Get** /v1/youtube/videos/{video_id}/live_chat | Live chat messages
[**YoutubeOembedMetadata**](YouTubeAPI.md#YoutubeOembedMetadata) | **Get** /v1/youtube/oembed | oEmbed metadata
[**YoutubePlaylistItemsPage**](YouTubeAPI.md#YoutubePlaylistItemsPage) | **Get** /v1/youtube/playlists/{playlist_id}/items | Playlist items page
[**YoutubeRelatedVideos**](YouTubeAPI.md#YoutubeRelatedVideos) | **Get** /v1/youtube/videos/{video_id}/related | Related videos
[**YoutubeResolveHandleUrlToId**](YouTubeAPI.md#YoutubeResolveHandleUrlToId) | **Get** /v1/youtube/channels/resolve | Resolve handle/URL to id
[**YoutubeSearchWithinAChannel**](YouTubeAPI.md#YoutubeSearchWithinAChannel) | **Get** /v1/youtube/channels/{channel_id}/search | Search within a channel
[**YoutubeSearchYoutube**](YouTubeAPI.md#YoutubeSearchYoutube) | **Get** /v1/youtube/search | Search YouTube
[**YoutubeSearchYoutubeMusic**](YouTubeAPI.md#YoutubeSearchYoutubeMusic) | **Get** /v1/youtube/music/search | Search YouTube Music
[**YoutubeShortsBySound**](YouTubeAPI.md#YoutubeShortsBySound) | **Get** /v1/youtube/shorts/by_sound/{sound_id} | Shorts by sound
[**YoutubeStreamFormats**](YouTubeAPI.md#YoutubeStreamFormats) | **Get** /v1/youtube/videos/{video_id}/streams | Stream formats
[**YoutubeSubscriberCountFast**](YouTubeAPI.md#YoutubeSubscriberCountFast) | **Get** /v1/youtube/channels/{channel_id}/subscriber_count | Subscriber count (fast)
[**YoutubeSupportedMarkets**](YouTubeAPI.md#YoutubeSupportedMarkets) | **Get** /v1/youtube/markets | Supported markets
[**YoutubeTrendingShorts**](YouTubeAPI.md#YoutubeTrendingShorts) | **Get** /v1/youtube/trending/shorts | Trending shorts
[**YoutubeTrendingVideos**](YouTubeAPI.md#YoutubeTrendingVideos) | **Get** /v1/youtube/trending | Trending videos
[**YoutubeUiLanguages**](YouTubeAPI.md#YoutubeUiLanguages) | **Get** /v1/youtube/languages | UI languages
[**YoutubeVideoCategories**](YouTubeAPI.md#YoutubeVideoCategories) | **Get** /v1/youtube/categories | Video categories
[**YoutubeVideoComments**](YouTubeAPI.md#YoutubeVideoComments) | **Get** /v1/youtube/videos/{video_id}/comments | Video comments
[**YoutubeVideoTranscript**](YouTubeAPI.md#YoutubeVideoTranscript) | **Get** /v1/youtube/videos/{video_id}/transcript | Video transcript
[**YoutubeVideosUnderAHashtag**](YouTubeAPI.md#YoutubeVideosUnderAHashtag) | **Get** /v1/youtube/hashtags/{tag} | Videos under a hashtag
[**YoutubeYoutubeScraperHealthCheck**](YouTubeAPI.md#YoutubeYoutubeScraperHealthCheck) | **Get** /v1/youtube/health | YouTube scraper health check
[**YoutubeYoutubeScraperHealthCheckHead**](YouTubeAPI.md#YoutubeYoutubeScraperHealthCheckHead) | **Head** /v1/youtube/health | YouTube scraper health check



## YoutubeBatchVideoDetail

> interface{} YoutubeBatchVideoDetail(ctx).RequestBody(requestBody).Execute()

Batch video detail

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
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeBatchVideoDetail(context.Background()).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeBatchVideoDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeBatchVideoDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeBatchVideoDetail`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeBatchVideoDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **requestBody** | **map[string]interface{}** |  | 

### Return type

**interface{}**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## YoutubeChannelAbout

> interface{} YoutubeChannelAbout(ctx, channelId).Execute()

Channel about

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
	channelId := "channelId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeChannelAbout(context.Background(), channelId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeChannelAbout``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeChannelAbout`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeChannelAbout`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**channelId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeChannelAboutRequest struct via the builder pattern


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


## YoutubeChannelPlaylists

> interface{} YoutubeChannelPlaylists(ctx, channelId).Execute()

Channel playlists

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
	channelId := "channelId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeChannelPlaylists(context.Background(), channelId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeChannelPlaylists``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeChannelPlaylists`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeChannelPlaylists`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**channelId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeChannelPlaylistsRequest struct via the builder pattern


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


## YoutubeChannelShorts

> interface{} YoutubeChannelShorts(ctx, channelId).Execute()

Channel shorts

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
	channelId := "channelId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeChannelShorts(context.Background(), channelId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeChannelShorts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeChannelShorts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeChannelShorts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**channelId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeChannelShortsRequest struct via the builder pattern


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


## YoutubeChannelStreams

> interface{} YoutubeChannelStreams(ctx, channelId).Execute()

Channel streams

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
	channelId := "channelId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeChannelStreams(context.Background(), channelId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeChannelStreams``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeChannelStreams`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeChannelStreams`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**channelId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeChannelStreamsRequest struct via the builder pattern


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


## YoutubeChannelVideos

> interface{} YoutubeChannelVideos(ctx, channelId).Execute()

Channel videos

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
	channelId := "channelId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeChannelVideos(context.Background(), channelId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeChannelVideos``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeChannelVideos`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeChannelVideos`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**channelId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeChannelVideosRequest struct via the builder pattern


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


## YoutubeCommentReplies

> interface{} YoutubeCommentReplies(ctx, videoId, commentId).Continuation(continuation).Execute()

Comment replies

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
	commentId := "commentId_example" // string | 
	continuation := "continuation_example" // string | Replies continuation token

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeCommentReplies(context.Background(), videoId, commentId).Continuation(continuation).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeCommentReplies``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeCommentReplies`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeCommentReplies`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**videoId** | **string** |  | 
**commentId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeCommentRepliesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **continuation** | **string** | Replies continuation token | 

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


## YoutubeCommunityPostComments

> interface{} YoutubeCommunityPostComments(ctx, postId).Execute()

Community post comments

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
	resp, r, err := apiClient.YouTubeAPI.YoutubeCommunityPostComments(context.Background(), postId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeCommunityPostComments``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeCommunityPostComments`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeCommunityPostComments`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**postId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeCommunityPostCommentsRequest struct via the builder pattern


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


## YoutubeCommunityPosts

> interface{} YoutubeCommunityPosts(ctx, channelId).Execute()

Community posts

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
	channelId := "channelId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeCommunityPosts(context.Background(), channelId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeCommunityPosts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeCommunityPosts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeCommunityPosts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**channelId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeCommunityPostsRequest struct via the builder pattern


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


## YoutubeContentRegions

> interface{} YoutubeContentRegions(ctx).Execute()

Content regions

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
	resp, r, err := apiClient.YouTubeAPI.YoutubeContentRegions(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeContentRegions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeContentRegions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeContentRegions`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeContentRegionsRequest struct via the builder pattern


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


## YoutubeGetACommunityPost

> interface{} YoutubeGetACommunityPost(ctx, postId).Execute()

Get a community post

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
	resp, r, err := apiClient.YouTubeAPI.YoutubeGetACommunityPost(context.Background(), postId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeGetACommunityPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeGetACommunityPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeGetACommunityPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**postId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeGetACommunityPostRequest struct via the builder pattern


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


## YoutubeGetAMixRadioQueue

> interface{} YoutubeGetAMixRadioQueue(ctx, playlistId).Execute()

Get a mix / radio queue

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
	playlistId := "playlistId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeGetAMixRadioQueue(context.Background(), playlistId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeGetAMixRadioQueue``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeGetAMixRadioQueue`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeGetAMixRadioQueue`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**playlistId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeGetAMixRadioQueueRequest struct via the builder pattern


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


## YoutubeGetAShort

> interface{} YoutubeGetAShort(ctx, videoId).Execute()

Get a Short

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeGetAShort(context.Background(), videoId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeGetAShort``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeGetAShort`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeGetAShort`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**videoId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeGetAShortRequest struct via the builder pattern


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


## YoutubeGetChannelDetail

> interface{} YoutubeGetChannelDetail(ctx, channelId).Gl(gl).Hl(hl).Execute()

Get channel detail



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
	channelId := "channelId_example" // string | 
	gl := "gl_example" // string |  (optional)
	hl := "hl_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeGetChannelDetail(context.Background(), channelId).Gl(gl).Hl(hl).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeGetChannelDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeGetChannelDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeGetChannelDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**channelId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeGetChannelDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **gl** | **string** |  | 
 **hl** | **string** |  | 

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


## YoutubeGetPlaylistDetail

> interface{} YoutubeGetPlaylistDetail(ctx, playlistId).Execute()

Get playlist detail

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
	playlistId := "playlistId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeGetPlaylistDetail(context.Background(), playlistId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeGetPlaylistDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeGetPlaylistDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeGetPlaylistDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**playlistId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeGetPlaylistDetailRequest struct via the builder pattern


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


## YoutubeGetVideoDetail

> interface{} YoutubeGetVideoDetail(ctx, videoId).Gl(gl).Hl(hl).Execute()

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
	gl := "gl_example" // string |  (optional)
	hl := "hl_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeGetVideoDetail(context.Background(), videoId).Gl(gl).Hl(hl).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeGetVideoDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeGetVideoDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeGetVideoDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**videoId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeGetVideoDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **gl** | **string** |  | 
 **hl** | **string** |  | 

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


## YoutubeGuestHomeFeed

> interface{} YoutubeGuestHomeFeed(ctx).Execute()

Guest home feed

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
	resp, r, err := apiClient.YouTubeAPI.YoutubeGuestHomeFeed(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeGuestHomeFeed``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeGuestHomeFeed`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeGuestHomeFeed`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeGuestHomeFeedRequest struct via the builder pattern


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


## YoutubeKeywordSuggestions

> interface{} YoutubeKeywordSuggestions(ctx).Query(query).Gl(gl).Hl(hl).Execute()

Keyword suggestions



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
	query := "query_example" // string | Partial query prefix
	gl := "gl_example" // string |  (optional)
	hl := "hl_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeKeywordSuggestions(context.Background()).Query(query).Gl(gl).Hl(hl).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeKeywordSuggestions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeKeywordSuggestions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeKeywordSuggestions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeKeywordSuggestionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Partial query prefix | 
 **gl** | **string** |  | 
 **hl** | **string** |  | 

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


## YoutubeListCaptionTracks

> interface{} YoutubeListCaptionTracks(ctx, videoId).Execute()

List caption tracks

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeListCaptionTracks(context.Background(), videoId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeListCaptionTracks``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeListCaptionTracks`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeListCaptionTracks`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**videoId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeListCaptionTracksRequest struct via the builder pattern


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


## YoutubeLiveChatMessages

> interface{} YoutubeLiveChatMessages(ctx, videoId).Continuation(continuation).Replay(replay).Execute()

Live chat messages

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
	continuation := "continuation_example" // string |  (optional)
	replay := true // bool |  (optional) (default to false)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeLiveChatMessages(context.Background(), videoId).Continuation(continuation).Replay(replay).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeLiveChatMessages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeLiveChatMessages`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeLiveChatMessages`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**videoId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeLiveChatMessagesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **continuation** | **string** |  | 
 **replay** | **bool** |  | [default to false]

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


## YoutubeOembedMetadata

> interface{} YoutubeOembedMetadata(ctx).Url(url).Execute()

oEmbed metadata

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
	url := "url_example" // string | A YouTube URL

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeOembedMetadata(context.Background()).Url(url).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeOembedMetadata``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeOembedMetadata`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeOembedMetadata`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeOembedMetadataRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **url** | **string** | A YouTube URL | 

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


## YoutubePlaylistItemsPage

> interface{} YoutubePlaylistItemsPage(ctx, playlistId).Execute()

Playlist items page

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
	playlistId := "playlistId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubePlaylistItemsPage(context.Background(), playlistId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubePlaylistItemsPage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubePlaylistItemsPage`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubePlaylistItemsPage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**playlistId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubePlaylistItemsPageRequest struct via the builder pattern


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


## YoutubeRelatedVideos

> interface{} YoutubeRelatedVideos(ctx, videoId).Execute()

Related videos

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeRelatedVideos(context.Background(), videoId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeRelatedVideos``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeRelatedVideos`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeRelatedVideos`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**videoId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeRelatedVideosRequest struct via the builder pattern


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


## YoutubeResolveHandleUrlToId

> interface{} YoutubeResolveHandleUrlToId(ctx).Handle(handle).Url(url).Execute()

Resolve handle/URL to id

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
	handle := "handle_example" // string |  (optional)
	url := "url_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeResolveHandleUrlToId(context.Background()).Handle(handle).Url(url).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeResolveHandleUrlToId``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeResolveHandleUrlToId`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeResolveHandleUrlToId`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeResolveHandleUrlToIdRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string** |  | 
 **url** | **string** |  | 

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


## YoutubeSearchWithinAChannel

> interface{} YoutubeSearchWithinAChannel(ctx, channelId).Query(query).Execute()

Search within a channel

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
	channelId := "channelId_example" // string | 
	query := "query_example" // string | Search keywords

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeSearchWithinAChannel(context.Background(), channelId).Query(query).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeSearchWithinAChannel``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeSearchWithinAChannel`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeSearchWithinAChannel`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**channelId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeSearchWithinAChannelRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **query** | **string** | Search keywords | 

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


## YoutubeSearchYoutube

> interface{} YoutubeSearchYoutube(ctx).Query(query).Type_(type_).SortBy(sortBy).UploadDate(uploadDate).Duration(duration).Features(features).Gl(gl).Hl(hl).Continuation(continuation).Execute()

Search YouTube



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
	type_ := "type__example" // string | video|channel|playlist|movie|all (optional)
	sortBy := "sortBy_example" // string | relevance|date|views|rating (optional)
	uploadDate := "uploadDate_example" // string | hour|today|week|month|year (optional)
	duration := "duration_example" // string | short|medium|long (optional)
	features := "features_example" // string | hd,4k,360,vr180,3d,hdr,cc,subtitles,live (optional)
	gl := "gl_example" // string | Content region (US, GB, DE…) (optional)
	hl := "hl_example" // string | UI language (optional)
	continuation := "continuation_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeSearchYoutube(context.Background()).Query(query).Type_(type_).SortBy(sortBy).UploadDate(uploadDate).Duration(duration).Features(features).Gl(gl).Hl(hl).Continuation(continuation).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeSearchYoutube``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeSearchYoutube`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeSearchYoutube`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeSearchYoutubeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords | 
 **type_** | **string** | video|channel|playlist|movie|all | 
 **sortBy** | **string** | relevance|date|views|rating | 
 **uploadDate** | **string** | hour|today|week|month|year | 
 **duration** | **string** | short|medium|long | 
 **features** | **string** | hd,4k,360,vr180,3d,hdr,cc,subtitles,live | 
 **gl** | **string** | Content region (US, GB, DE…) | 
 **hl** | **string** | UI language | 
 **continuation** | **string** |  | 

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


## YoutubeSearchYoutubeMusic

> interface{} YoutubeSearchYoutubeMusic(ctx).Query(query).Execute()

Search YouTube Music

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeSearchYoutubeMusic(context.Background()).Query(query).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeSearchYoutubeMusic``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeSearchYoutubeMusic`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeSearchYoutubeMusic`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeSearchYoutubeMusicRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Search keywords | 

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


## YoutubeShortsBySound

> interface{} YoutubeShortsBySound(ctx, soundId).Execute()

Shorts by sound

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
	soundId := "soundId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeShortsBySound(context.Background(), soundId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeShortsBySound``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeShortsBySound`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeShortsBySound`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**soundId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeShortsBySoundRequest struct via the builder pattern


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


## YoutubeStreamFormats

> interface{} YoutubeStreamFormats(ctx, videoId).Client(client).Execute()

Stream formats



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
	client := "client_example" // string | IOS|ANDROID|WEB (optional) (default to "IOS")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeStreamFormats(context.Background(), videoId).Client(client).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeStreamFormats``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeStreamFormats`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeStreamFormats`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**videoId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeStreamFormatsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **client** | **string** | IOS|ANDROID|WEB | [default to &quot;IOS&quot;]

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


## YoutubeSubscriberCountFast

> interface{} YoutubeSubscriberCountFast(ctx, channelId).Execute()

Subscriber count (fast)

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
	channelId := "channelId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeSubscriberCountFast(context.Background(), channelId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeSubscriberCountFast``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeSubscriberCountFast`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeSubscriberCountFast`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**channelId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeSubscriberCountFastRequest struct via the builder pattern


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


## YoutubeSupportedMarkets

> interface{} YoutubeSupportedMarkets(ctx).Execute()

Supported markets

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
	resp, r, err := apiClient.YouTubeAPI.YoutubeSupportedMarkets(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeSupportedMarkets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeSupportedMarkets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeSupportedMarkets`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeSupportedMarketsRequest struct via the builder pattern


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


## YoutubeTrendingShorts

> interface{} YoutubeTrendingShorts(ctx).Execute()

Trending shorts

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
	resp, r, err := apiClient.YouTubeAPI.YoutubeTrendingShorts(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeTrendingShorts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeTrendingShorts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeTrendingShorts`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeTrendingShortsRequest struct via the builder pattern


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


## YoutubeTrendingVideos

> interface{} YoutubeTrendingVideos(ctx).Gl(gl).Type_(type_).Execute()

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
	gl := "gl_example" // string |  (optional)
	type_ := "type__example" // string | now|music|gaming|movies (optional) (default to "now")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeTrendingVideos(context.Background()).Gl(gl).Type_(type_).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeTrendingVideos``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeTrendingVideos`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeTrendingVideos`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeTrendingVideosRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gl** | **string** |  | 
 **type_** | **string** | now|music|gaming|movies | [default to &quot;now&quot;]

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


## YoutubeUiLanguages

> interface{} YoutubeUiLanguages(ctx).Execute()

UI languages

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
	resp, r, err := apiClient.YouTubeAPI.YoutubeUiLanguages(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeUiLanguages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeUiLanguages`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeUiLanguages`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeUiLanguagesRequest struct via the builder pattern


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


## YoutubeVideoCategories

> interface{} YoutubeVideoCategories(ctx).Gl(gl).Execute()

Video categories

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
	gl := "gl_example" // string |  (optional) (default to "US")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeVideoCategories(context.Background()).Gl(gl).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeVideoCategories``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeVideoCategories`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeVideoCategories`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeVideoCategoriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gl** | **string** |  | [default to &quot;US&quot;]

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


## YoutubeVideoComments

> interface{} YoutubeVideoComments(ctx, videoId).SortBy(sortBy).Continuation(continuation).Execute()

Video comments

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
	sortBy := "sortBy_example" // string | top|newest (optional) (default to "top")
	continuation := "continuation_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeVideoComments(context.Background(), videoId).SortBy(sortBy).Continuation(continuation).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeVideoComments``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeVideoComments`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeVideoComments`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**videoId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeVideoCommentsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **sortBy** | **string** | top|newest | [default to &quot;top&quot;]
 **continuation** | **string** |  | 

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


## YoutubeVideoTranscript

> interface{} YoutubeVideoTranscript(ctx, videoId).Language(language).Execute()

Video transcript

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
	language := "language_example" // string | BCP-47 language code (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.YouTubeAPI.YoutubeVideoTranscript(context.Background(), videoId).Language(language).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeVideoTranscript``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeVideoTranscript`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeVideoTranscript`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**videoId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeVideoTranscriptRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **language** | **string** | BCP-47 language code | 

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


## YoutubeVideosUnderAHashtag

> interface{} YoutubeVideosUnderAHashtag(ctx, tag).Execute()

Videos under a hashtag

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
	resp, r, err := apiClient.YouTubeAPI.YoutubeVideosUnderAHashtag(context.Background(), tag).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeVideosUnderAHashtag``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeVideosUnderAHashtag`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeVideosUnderAHashtag`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tag** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeVideosUnderAHashtagRequest struct via the builder pattern


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


## YoutubeYoutubeScraperHealthCheck

> interface{} YoutubeYoutubeScraperHealthCheck(ctx).Execute()

YouTube scraper health check



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
	resp, r, err := apiClient.YouTubeAPI.YoutubeYoutubeScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeYoutubeScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeYoutubeScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeYoutubeScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeYoutubeScraperHealthCheckRequest struct via the builder pattern


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


## YoutubeYoutubeScraperHealthCheckHead

> interface{} YoutubeYoutubeScraperHealthCheckHead(ctx).Execute()

YouTube scraper health check



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
	resp, r, err := apiClient.YouTubeAPI.YoutubeYoutubeScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `YouTubeAPI.YoutubeYoutubeScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `YoutubeYoutubeScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `YouTubeAPI.YoutubeYoutubeScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiYoutubeYoutubeScraperHealthCheckHeadRequest struct via the builder pattern


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


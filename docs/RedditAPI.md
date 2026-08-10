# \RedditAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**RedditGetCrossPosts**](RedditAPI.md#RedditGetCrossPosts) | **Get** /v1/reddit/posts/{post_id}/duplicates | Get cross-posts
[**RedditGetPostComments**](RedditAPI.md#RedditGetPostComments) | **Get** /v1/reddit/posts/{post_id}/comments | Get post comments
[**RedditGetPostDetail**](RedditAPI.md#RedditGetPostDetail) | **Get** /v1/reddit/posts/{post_id} | Get post detail
[**RedditGetPostsByDomain**](RedditAPI.md#RedditGetPostsByDomain) | **Get** /v1/reddit/domains/{domain}/posts | Get posts by domain
[**RedditGetSubredditInfo**](RedditAPI.md#RedditGetSubredditInfo) | **Get** /v1/reddit/subreddits/{subreddit} | Get subreddit info
[**RedditGetSubredditPosts**](RedditAPI.md#RedditGetSubredditPosts) | **Get** /v1/reddit/subreddits/{subreddit}/posts | Get subreddit posts
[**RedditGetSubredditRules**](RedditAPI.md#RedditGetSubredditRules) | **Get** /v1/reddit/subreddits/{subreddit}/rules | Get subreddit rules
[**RedditGetTrendingPosts**](RedditAPI.md#RedditGetTrendingPosts) | **Get** /v1/reddit/posts/trending | Get trending posts
[**RedditGetUserProfile**](RedditAPI.md#RedditGetUserProfile) | **Get** /v1/reddit/users/{username} | Get user profile
[**RedditGetUserSComments**](RedditAPI.md#RedditGetUserSComments) | **Get** /v1/reddit/users/{username}/comments | Get user&#39;s comments
[**RedditGetUserSModeratedSubreddits**](RedditAPI.md#RedditGetUserSModeratedSubreddits) | **Get** /v1/reddit/users/{username}/moderated | Get user&#39;s moderated subreddits
[**RedditGetUserSPosts**](RedditAPI.md#RedditGetUserSPosts) | **Get** /v1/reddit/users/{username}/posts | Get user&#39;s posts
[**RedditGetUserSTrophies**](RedditAPI.md#RedditGetUserSTrophies) | **Get** /v1/reddit/users/{username}/trophies | Get user&#39;s trophies
[**RedditGetWikiPageContent**](RedditAPI.md#RedditGetWikiPageContent) | **Get** /v1/reddit/subreddits/{subreddit}/wiki/{page} | Get wiki page content
[**RedditListWikiPages**](RedditAPI.md#RedditListWikiPages) | **Get** /v1/reddit/subreddits/{subreddit}/wiki | List wiki pages
[**RedditNewSubreddits**](RedditAPI.md#RedditNewSubreddits) | **Get** /v1/reddit/subreddits/new | New subreddits
[**RedditPopularSubreddits**](RedditAPI.md#RedditPopularSubreddits) | **Get** /v1/reddit/subreddits/popular | Popular subreddits
[**RedditRedditScraperHealthCheck**](RedditAPI.md#RedditRedditScraperHealthCheck) | **Get** /v1/reddit/health | Reddit scraper health check
[**RedditRedditScraperHealthCheckHead**](RedditAPI.md#RedditRedditScraperHealthCheckHead) | **Head** /v1/reddit/health | Reddit scraper health check
[**RedditSearchRedditPosts**](RedditAPI.md#RedditSearchRedditPosts) | **Get** /v1/reddit/search/posts | Search Reddit posts
[**RedditSearchSubreddits**](RedditAPI.md#RedditSearchSubreddits) | **Get** /v1/reddit/search/subreddits | Search subreddits
[**RedditSearchUsers**](RedditAPI.md#RedditSearchUsers) | **Get** /v1/reddit/search/users | Search users



## RedditGetCrossPosts

> interface{} RedditGetCrossPosts(ctx, postId).Limit(limit).After(after).Execute()

Get cross-posts



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
	limit := int32(56) // int32 |  (optional) (default to 25)
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedditAPI.RedditGetCrossPosts(context.Background(), postId).Limit(limit).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditGetCrossPosts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditGetCrossPosts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditGetCrossPosts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**postId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRedditGetCrossPostsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int32** |  | [default to 25]
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


## RedditGetPostComments

> interface{} RedditGetPostComments(ctx, postId).Sort(sort).Limit(limit).Depth(depth).Execute()

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
	sort := "sort_example" // string | Sort: confidence, top, new, controversial, old, qa (optional) (default to "confidence")
	limit := int32(56) // int32 |  (optional) (default to 25)
	depth := int32(56) // int32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedditAPI.RedditGetPostComments(context.Background(), postId).Sort(sort).Limit(limit).Depth(depth).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditGetPostComments``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditGetPostComments`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditGetPostComments`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**postId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRedditGetPostCommentsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **sort** | **string** | Sort: confidence, top, new, controversial, old, qa | [default to &quot;confidence&quot;]
 **limit** | **int32** |  | [default to 25]
 **depth** | **int32** |  | 

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


## RedditGetPostDetail

> interface{} RedditGetPostDetail(ctx, postId).Execute()

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
	resp, r, err := apiClient.RedditAPI.RedditGetPostDetail(context.Background(), postId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditGetPostDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditGetPostDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditGetPostDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**postId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRedditGetPostDetailRequest struct via the builder pattern


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


## RedditGetPostsByDomain

> interface{} RedditGetPostsByDomain(ctx, domain).Sort(sort).T(t).Limit(limit).After(after).Execute()

Get posts by domain



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
	domain := "domain_example" // string | 
	sort := "sort_example" // string |  (optional) (default to "hot")
	t := "t_example" // string |  (optional) (default to "all")
	limit := int32(56) // int32 |  (optional) (default to 25)
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedditAPI.RedditGetPostsByDomain(context.Background(), domain).Sort(sort).T(t).Limit(limit).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditGetPostsByDomain``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditGetPostsByDomain`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditGetPostsByDomain`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**domain** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRedditGetPostsByDomainRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **sort** | **string** |  | [default to &quot;hot&quot;]
 **t** | **string** |  | [default to &quot;all&quot;]
 **limit** | **int32** |  | [default to 25]
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


## RedditGetSubredditInfo

> interface{} RedditGetSubredditInfo(ctx, subreddit).Execute()

Get subreddit info



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
	subreddit := "subreddit_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedditAPI.RedditGetSubredditInfo(context.Background(), subreddit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditGetSubredditInfo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditGetSubredditInfo`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditGetSubredditInfo`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**subreddit** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRedditGetSubredditInfoRequest struct via the builder pattern


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


## RedditGetSubredditPosts

> interface{} RedditGetSubredditPosts(ctx, subreddit).Sort(sort).T(t).Limit(limit).After(after).Execute()

Get subreddit posts



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
	subreddit := "subreddit_example" // string | 
	sort := "sort_example" // string | Sort: hot, new, top, rising, controversial (optional) (default to "hot")
	t := "t_example" // string | Time filter (optional) (default to "all")
	limit := int32(56) // int32 |  (optional) (default to 25)
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedditAPI.RedditGetSubredditPosts(context.Background(), subreddit).Sort(sort).T(t).Limit(limit).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditGetSubredditPosts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditGetSubredditPosts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditGetSubredditPosts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**subreddit** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRedditGetSubredditPostsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **sort** | **string** | Sort: hot, new, top, rising, controversial | [default to &quot;hot&quot;]
 **t** | **string** | Time filter | [default to &quot;all&quot;]
 **limit** | **int32** |  | [default to 25]
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


## RedditGetSubredditRules

> interface{} RedditGetSubredditRules(ctx, subreddit).Execute()

Get subreddit rules



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
	subreddit := "subreddit_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedditAPI.RedditGetSubredditRules(context.Background(), subreddit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditGetSubredditRules``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditGetSubredditRules`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditGetSubredditRules`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**subreddit** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRedditGetSubredditRulesRequest struct via the builder pattern


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


## RedditGetTrendingPosts

> interface{} RedditGetTrendingPosts(ctx).Sort(sort).T(t).Limit(limit).After(after).Execute()

Get trending posts



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
	sort := "sort_example" // string | Sort: hot, new, top, rising, controversial, best (optional) (default to "hot")
	t := "t_example" // string | Time filter (optional) (default to "day")
	limit := int32(56) // int32 |  (optional) (default to 25)
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedditAPI.RedditGetTrendingPosts(context.Background()).Sort(sort).T(t).Limit(limit).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditGetTrendingPosts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditGetTrendingPosts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditGetTrendingPosts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRedditGetTrendingPostsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sort** | **string** | Sort: hot, new, top, rising, controversial, best | [default to &quot;hot&quot;]
 **t** | **string** | Time filter | [default to &quot;day&quot;]
 **limit** | **int32** |  | [default to 25]
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


## RedditGetUserProfile

> interface{} RedditGetUserProfile(ctx, username).Execute()

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedditAPI.RedditGetUserProfile(context.Background(), username).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditGetUserProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditGetUserProfile`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditGetUserProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRedditGetUserProfileRequest struct via the builder pattern


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


## RedditGetUserSComments

> interface{} RedditGetUserSComments(ctx, username).Sort(sort).T(t).Limit(limit).After(after).Execute()

Get user's comments



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
	sort := "sort_example" // string |  (optional) (default to "new")
	t := "t_example" // string |  (optional) (default to "all")
	limit := int32(56) // int32 |  (optional) (default to 25)
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedditAPI.RedditGetUserSComments(context.Background(), username).Sort(sort).T(t).Limit(limit).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditGetUserSComments``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditGetUserSComments`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditGetUserSComments`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRedditGetUserSCommentsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **sort** | **string** |  | [default to &quot;new&quot;]
 **t** | **string** |  | [default to &quot;all&quot;]
 **limit** | **int32** |  | [default to 25]
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


## RedditGetUserSModeratedSubreddits

> interface{} RedditGetUserSModeratedSubreddits(ctx, username).Execute()

Get user's moderated subreddits



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
	resp, r, err := apiClient.RedditAPI.RedditGetUserSModeratedSubreddits(context.Background(), username).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditGetUserSModeratedSubreddits``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditGetUserSModeratedSubreddits`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditGetUserSModeratedSubreddits`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRedditGetUserSModeratedSubredditsRequest struct via the builder pattern


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


## RedditGetUserSPosts

> interface{} RedditGetUserSPosts(ctx, username).Sort(sort).T(t).Limit(limit).After(after).Execute()

Get user's posts



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
	sort := "sort_example" // string |  (optional) (default to "new")
	t := "t_example" // string |  (optional) (default to "all")
	limit := int32(56) // int32 |  (optional) (default to 25)
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedditAPI.RedditGetUserSPosts(context.Background(), username).Sort(sort).T(t).Limit(limit).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditGetUserSPosts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditGetUserSPosts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditGetUserSPosts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRedditGetUserSPostsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **sort** | **string** |  | [default to &quot;new&quot;]
 **t** | **string** |  | [default to &quot;all&quot;]
 **limit** | **int32** |  | [default to 25]
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


## RedditGetUserSTrophies

> interface{} RedditGetUserSTrophies(ctx, username).Execute()

Get user's trophies



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
	resp, r, err := apiClient.RedditAPI.RedditGetUserSTrophies(context.Background(), username).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditGetUserSTrophies``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditGetUserSTrophies`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditGetUserSTrophies`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRedditGetUserSTrophiesRequest struct via the builder pattern


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


## RedditGetWikiPageContent

> interface{} RedditGetWikiPageContent(ctx, subreddit, page).Execute()

Get wiki page content



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
	subreddit := "subreddit_example" // string | 
	page := "page_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedditAPI.RedditGetWikiPageContent(context.Background(), subreddit, page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditGetWikiPageContent``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditGetWikiPageContent`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditGetWikiPageContent`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**subreddit** | **string** |  | 
**page** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRedditGetWikiPageContentRequest struct via the builder pattern


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


## RedditListWikiPages

> interface{} RedditListWikiPages(ctx, subreddit).Execute()

List wiki pages



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
	subreddit := "subreddit_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedditAPI.RedditListWikiPages(context.Background(), subreddit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditListWikiPages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditListWikiPages`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditListWikiPages`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**subreddit** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRedditListWikiPagesRequest struct via the builder pattern


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


## RedditNewSubreddits

> interface{} RedditNewSubreddits(ctx).Limit(limit).After(after).Execute()

New subreddits



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
	limit := int32(56) // int32 |  (optional) (default to 25)
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedditAPI.RedditNewSubreddits(context.Background()).Limit(limit).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditNewSubreddits``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditNewSubreddits`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditNewSubreddits`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRedditNewSubredditsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 25]
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


## RedditPopularSubreddits

> interface{} RedditPopularSubreddits(ctx).Limit(limit).After(after).Execute()

Popular subreddits



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
	limit := int32(56) // int32 |  (optional) (default to 25)
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedditAPI.RedditPopularSubreddits(context.Background()).Limit(limit).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditPopularSubreddits``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditPopularSubreddits`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditPopularSubreddits`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRedditPopularSubredditsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 25]
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


## RedditRedditScraperHealthCheck

> interface{} RedditRedditScraperHealthCheck(ctx).Execute()

Reddit scraper health check

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
	resp, r, err := apiClient.RedditAPI.RedditRedditScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditRedditScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditRedditScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditRedditScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiRedditRedditScraperHealthCheckRequest struct via the builder pattern


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


## RedditRedditScraperHealthCheckHead

> interface{} RedditRedditScraperHealthCheckHead(ctx).Execute()

Reddit scraper health check

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
	resp, r, err := apiClient.RedditAPI.RedditRedditScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditRedditScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditRedditScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditRedditScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiRedditRedditScraperHealthCheckHeadRequest struct via the builder pattern


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


## RedditSearchRedditPosts

> interface{} RedditSearchRedditPosts(ctx).Q(q).Subreddit(subreddit).Sort(sort).T(t).Limit(limit).After(after).Execute()

Search Reddit posts



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
	subreddit := "subreddit_example" // string | Restrict to subreddit (optional)
	sort := "sort_example" // string | Sort: relevance, hot, top, new, comments (optional) (default to "relevance")
	t := "t_example" // string | Time: hour, day, week, month, year, all (optional) (default to "all")
	limit := int32(56) // int32 |  (optional) (default to 25)
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedditAPI.RedditSearchRedditPosts(context.Background()).Q(q).Subreddit(subreddit).Sort(sort).T(t).Limit(limit).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditSearchRedditPosts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditSearchRedditPosts`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditSearchRedditPosts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRedditSearchRedditPostsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search query | 
 **subreddit** | **string** | Restrict to subreddit | 
 **sort** | **string** | Sort: relevance, hot, top, new, comments | [default to &quot;relevance&quot;]
 **t** | **string** | Time: hour, day, week, month, year, all | [default to &quot;all&quot;]
 **limit** | **int32** |  | [default to 25]
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


## RedditSearchSubreddits

> interface{} RedditSearchSubreddits(ctx).Q(q).Limit(limit).After(after).Execute()

Search subreddits



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
	limit := int32(56) // int32 |  (optional) (default to 25)
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedditAPI.RedditSearchSubreddits(context.Background()).Q(q).Limit(limit).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditSearchSubreddits``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditSearchSubreddits`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditSearchSubreddits`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRedditSearchSubredditsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search query | 
 **limit** | **int32** |  | [default to 25]
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


## RedditSearchUsers

> interface{} RedditSearchUsers(ctx).Q(q).Limit(limit).After(after).Execute()

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
	q := "q_example" // string | Search query
	limit := int32(56) // int32 |  (optional) (default to 25)
	after := "after_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RedditAPI.RedditSearchUsers(context.Background()).Q(q).Limit(limit).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RedditAPI.RedditSearchUsers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RedditSearchUsers`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `RedditAPI.RedditSearchUsers`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRedditSearchUsersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** | Search query | 
 **limit** | **int32** |  | [default to 25]
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


# \TwitterAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**TwitterAdvancedTweetSearch**](TwitterAPI.md#TwitterAdvancedTweetSearch) | **Get** /v1/twitter/tweets/advanced_search | Advanced tweet search
[**TwitterBatchGetUsersByIds**](TwitterAPI.md#TwitterBatchGetUsersByIds) | **Get** /v1/twitter/users/batch_by_ids | Batch get users by IDs
[**TwitterBatchGetUsersByUsernames**](TwitterAPI.md#TwitterBatchGetUsersByUsernames) | **Get** /v1/twitter/users/batch_by_usernames | Batch get users by usernames
[**TwitterConfigureWebhookOnAMonitor**](TwitterAPI.md#TwitterConfigureWebhookOnAMonitor) | **Post** /v1/twitter/stream/webhooks | Configure webhook on a monitor
[**TwitterCreateFilterRule**](TwitterAPI.md#TwitterCreateFilterRule) | **Post** /v1/twitter/stream/filter-rules | Create filter rule
[**TwitterCreateStreamMonitor**](TwitterAPI.md#TwitterCreateStreamMonitor) | **Post** /v1/twitter/stream/monitors | Create stream monitor
[**TwitterDeleteFilterRule**](TwitterAPI.md#TwitterDeleteFilterRule) | **Delete** /v1/twitter/stream/filter-rules/{rule_id} | Delete filter rule
[**TwitterDeleteStreamMonitor**](TwitterAPI.md#TwitterDeleteStreamMonitor) | **Delete** /v1/twitter/stream/monitors/{monitor_id} | Delete stream monitor
[**TwitterGetArticleById**](TwitterAPI.md#TwitterGetArticleById) | **Get** /v1/twitter/tweets/article/{article_id} | Get article by ID
[**TwitterGetBroadcastDetails**](TwitterAPI.md#TwitterGetBroadcastDetails) | **Get** /v1/twitter/spaces/broadcast/{broadcast_id} | Get broadcast details
[**TwitterGetCommunityDetails**](TwitterAPI.md#TwitterGetCommunityDetails) | **Get** /v1/twitter/communities/{community_id} | Get community details
[**TwitterGetCommunityNotes**](TwitterAPI.md#TwitterGetCommunityNotes) | **Get** /v1/twitter/tweets/tweet/{tweet_id}/community_notes | Get community notes
[**TwitterGetCommunityTweets**](TwitterAPI.md#TwitterGetCommunityTweets) | **Get** /v1/twitter/communities/{community_id}/tweets | Get community tweets
[**TwitterGetFilterRule**](TwitterAPI.md#TwitterGetFilterRule) | **Get** /v1/twitter/stream/filter-rules/{rule_id} | Get filter rule
[**TwitterGetFilterRulePerPollRates**](TwitterAPI.md#TwitterGetFilterRulePerPollRates) | **Get** /v1/twitter/stream/filter-rules-pricing | Get filter rule per-poll rates
[**TwitterGetListDetails**](TwitterAPI.md#TwitterGetListDetails) | **Get** /v1/twitter/lists/{list_id}/detail | Get list details
[**TwitterGetListTweets**](TwitterAPI.md#TwitterGetListTweets) | **Get** /v1/twitter/lists/{list_id}/tweets | Get list tweets
[**TwitterGetPlaceDetails**](TwitterAPI.md#TwitterGetPlaceDetails) | **Get** /v1/twitter/geo/places/{place_id} | Get place details
[**TwitterGetSimilarTweets**](TwitterAPI.md#TwitterGetSimilarTweets) | **Get** /v1/twitter/tweets/tweet/{tweet_id}/similar | Get similar tweets
[**TwitterGetSpaceDetails**](TwitterAPI.md#TwitterGetSpaceDetails) | **Get** /v1/twitter/spaces/{space_id} | Get Space details
[**TwitterGetStreamMonitor**](TwitterAPI.md#TwitterGetStreamMonitor) | **Get** /v1/twitter/stream/monitors/{monitor_id} | Get stream monitor
[**TwitterGetTrendingTopics**](TwitterAPI.md#TwitterGetTrendingTopics) | **Get** /v1/twitter/trends/ | Get trending topics
[**TwitterGetTrendsByLocation**](TwitterAPI.md#TwitterGetTrendsByLocation) | **Get** /v1/twitter/trends/place/{woeid} | Get trends by location
[**TwitterGetTweetDetails**](TwitterAPI.md#TwitterGetTweetDetails) | **Get** /v1/twitter/tweets/tweet/{tweet_id} | Get tweet details
[**TwitterGetTweetEditHistory**](TwitterAPI.md#TwitterGetTweetEditHistory) | **Get** /v1/twitter/tweets/tweet/{tweet_id}/edit_history | Get tweet edit history
[**TwitterGetTweetFavoriters**](TwitterAPI.md#TwitterGetTweetFavoriters) | **Get** /v1/twitter/tweets/tweet/{tweet_id}/favoriters | Get tweet favoriters
[**TwitterGetTweetQuotes**](TwitterAPI.md#TwitterGetTweetQuotes) | **Get** /v1/twitter/tweets/tweet/{tweet_id}/quotes | Get tweet quotes
[**TwitterGetTweetReplies**](TwitterAPI.md#TwitterGetTweetReplies) | **Get** /v1/twitter/tweets/tweet/{tweet_id}/replies | Get tweet replies
[**TwitterGetTweetRetweeters**](TwitterAPI.md#TwitterGetTweetRetweeters) | **Get** /v1/twitter/tweets/tweet/{tweet_id}/retweeters | Get tweet retweeters
[**TwitterGetTweetsByIds**](TwitterAPI.md#TwitterGetTweetsByIds) | **Get** /v1/twitter/tweets/ | Get tweets by IDs
[**TwitterGetUserArticles**](TwitterAPI.md#TwitterGetUserArticles) | **Get** /v1/twitter/users/{user_id}/articles | Get user articles
[**TwitterGetUserById**](TwitterAPI.md#TwitterGetUserById) | **Get** /v1/twitter/users/{user_id}/by_id | Get user by ID
[**TwitterGetUserByUsername**](TwitterAPI.md#TwitterGetUserByUsername) | **Get** /v1/twitter/users/{username}/by_username | Get user by username
[**TwitterGetUserFollowers**](TwitterAPI.md#TwitterGetUserFollowers) | **Get** /v1/twitter/users/{username}/followers | Get user followers
[**TwitterGetUserFollowing**](TwitterAPI.md#TwitterGetUserFollowing) | **Get** /v1/twitter/users/{username}/followings | Get user following
[**TwitterGetUserMentions**](TwitterAPI.md#TwitterGetUserMentions) | **Get** /v1/twitter/users/{username}/mentions | Get user mentions
[**TwitterGetUserSubscriptions**](TwitterAPI.md#TwitterGetUserSubscriptions) | **Get** /v1/twitter/users/{user_id}/subscriptions | Get user subscriptions
[**TwitterGetUserTweets**](TwitterAPI.md#TwitterGetUserTweets) | **Get** /v1/twitter/users/{username}/latest_tweets | Get user tweets
[**TwitterListBillingLogs**](TwitterAPI.md#TwitterListBillingLogs) | **Get** /v1/twitter/stream/billing-logs | List billing logs
[**TwitterListDeliveryLogsForAFilterRule**](TwitterAPI.md#TwitterListDeliveryLogsForAFilterRule) | **Get** /v1/twitter/stream/filter-rules/{rule_id}/logs | List delivery logs for a filter rule
[**TwitterListFilterRules**](TwitterAPI.md#TwitterListFilterRules) | **Get** /v1/twitter/stream/filter-rules | List filter rules
[**TwitterListStreamMonitors**](TwitterAPI.md#TwitterListStreamMonitors) | **Get** /v1/twitter/stream/monitors | List stream monitors
[**TwitterListTweetDeliveryLogs**](TwitterAPI.md#TwitterListTweetDeliveryLogs) | **Get** /v1/twitter/stream/logs | List tweet delivery logs
[**TwitterListWebhooks**](TwitterAPI.md#TwitterListWebhooks) | **Get** /v1/twitter/stream/webhooks | List webhooks
[**TwitterRemoveWebhookFromMonitor**](TwitterAPI.md#TwitterRemoveWebhookFromMonitor) | **Delete** /v1/twitter/stream/webhooks/{webhook_id} | Remove webhook from monitor
[**TwitterSearchCommunities**](TwitterAPI.md#TwitterSearchCommunities) | **Get** /v1/twitter/communities/search | Search communities
[**TwitterSearchListTweets**](TwitterAPI.md#TwitterSearchListTweets) | **Get** /v1/twitter/lists/{list_id}/search_tweets | Search list tweets
[**TwitterSearchPlaces**](TwitterAPI.md#TwitterSearchPlaces) | **Get** /v1/twitter/geo/search | Search places
[**TwitterSearchUsers**](TwitterAPI.md#TwitterSearchUsers) | **Get** /v1/twitter/users/search_users | Search users
[**TwitterTestWebhookDelivery**](TwitterAPI.md#TwitterTestWebhookDelivery) | **Post** /v1/twitter/stream/webhooks/test | Test webhook delivery
[**TwitterTwitterScraperHealthCheck**](TwitterAPI.md#TwitterTwitterScraperHealthCheck) | **Get** /v1/twitter/health | Twitter scraper health check
[**TwitterTwitterScraperHealthCheckHead**](TwitterAPI.md#TwitterTwitterScraperHealthCheckHead) | **Head** /v1/twitter/health | Twitter scraper health check
[**TwitterUpdateFilterRule**](TwitterAPI.md#TwitterUpdateFilterRule) | **Patch** /v1/twitter/stream/filter-rules/{rule_id} | Update filter rule
[**TwitterUpdateStreamMonitor**](TwitterAPI.md#TwitterUpdateStreamMonitor) | **Patch** /v1/twitter/stream/monitors/{monitor_id} | Update stream monitor
[**TwitterValidateSearchQuery**](TwitterAPI.md#TwitterValidateSearchQuery) | **Post** /v1/twitter/stream/filter-rules/validate | Validate search query



## TwitterAdvancedTweetSearch

> interface{} TwitterAdvancedTweetSearch(ctx).Query(query).QueryType(queryType).Count(count).Cursor(cursor).Execute()

Advanced tweet search



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
	queryType := "queryType_example" // string |  (optional)
	count := int32(56) // int32 |  (optional)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterAdvancedTweetSearch(context.Background()).Query(query).QueryType(queryType).Count(count).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterAdvancedTweetSearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterAdvancedTweetSearch`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterAdvancedTweetSearch`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterAdvancedTweetSearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 
 **queryType** | **string** |  | 
 **count** | **int32** |  | 
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


## TwitterBatchGetUsersByIds

> interface{} TwitterBatchGetUsersByIds(ctx).UserIds(userIds).Execute()

Batch get users by IDs



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
	userIds := "userIds_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterBatchGetUsersByIds(context.Background()).UserIds(userIds).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterBatchGetUsersByIds``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterBatchGetUsersByIds`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterBatchGetUsersByIds`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterBatchGetUsersByIdsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userIds** | **string** |  | 

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


## TwitterBatchGetUsersByUsernames

> interface{} TwitterBatchGetUsersByUsernames(ctx).Usernames(usernames).Execute()

Batch get users by usernames



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
	usernames := "usernames_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterBatchGetUsersByUsernames(context.Background()).Usernames(usernames).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterBatchGetUsersByUsernames``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterBatchGetUsersByUsernames`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterBatchGetUsersByUsernames`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterBatchGetUsersByUsernamesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **usernames** | **string** |  | 

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


## TwitterConfigureWebhookOnAMonitor

> WebhookResponse TwitterConfigureWebhookOnAMonitor(ctx).WebhookCreate(webhookCreate).Execute()

Configure webhook on a monitor



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
	webhookCreate := *openapiclient.NewWebhookCreate("MonitorId_example", "Url_example") // WebhookCreate | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterConfigureWebhookOnAMonitor(context.Background()).WebhookCreate(webhookCreate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterConfigureWebhookOnAMonitor``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterConfigureWebhookOnAMonitor`: WebhookResponse
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterConfigureWebhookOnAMonitor`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterConfigureWebhookOnAMonitorRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **webhookCreate** | [**WebhookCreate**](WebhookCreate.md) |  | 

### Return type

[**WebhookResponse**](WebhookResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterCreateFilterRule

> FilterRuleResponse TwitterCreateFilterRule(ctx).FilterRuleCreate(filterRuleCreate).Execute()

Create filter rule



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
	filterRuleCreate := *openapiclient.NewFilterRuleCreate("Tag_example", "Query_example", float32(123)) // FilterRuleCreate | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterCreateFilterRule(context.Background()).FilterRuleCreate(filterRuleCreate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterCreateFilterRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterCreateFilterRule`: FilterRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterCreateFilterRule`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterCreateFilterRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filterRuleCreate** | [**FilterRuleCreate**](FilterRuleCreate.md) |  | 

### Return type

[**FilterRuleResponse**](FilterRuleResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterCreateStreamMonitor

> StreamMonitorResponse TwitterCreateStreamMonitor(ctx).StreamMonitorCreate(streamMonitorCreate).Execute()

Create stream monitor



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
	streamMonitorCreate := *openapiclient.NewStreamMonitorCreate("Name_example", []string{"Usernames_example"}) // StreamMonitorCreate | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterCreateStreamMonitor(context.Background()).StreamMonitorCreate(streamMonitorCreate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterCreateStreamMonitor``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterCreateStreamMonitor`: StreamMonitorResponse
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterCreateStreamMonitor`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterCreateStreamMonitorRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **streamMonitorCreate** | [**StreamMonitorCreate**](StreamMonitorCreate.md) |  | 

### Return type

[**StreamMonitorResponse**](StreamMonitorResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterDeleteFilterRule

> TwitterDeleteFilterRule(ctx, ruleId).Execute()

Delete filter rule



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
	ruleId := "ruleId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.TwitterAPI.TwitterDeleteFilterRule(context.Background(), ruleId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterDeleteFilterRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**ruleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterDeleteFilterRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterDeleteStreamMonitor

> TwitterDeleteStreamMonitor(ctx, monitorId).Execute()

Delete stream monitor



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
	monitorId := "monitorId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.TwitterAPI.TwitterDeleteStreamMonitor(context.Background(), monitorId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterDeleteStreamMonitor``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**monitorId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterDeleteStreamMonitorRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterGetArticleById

> interface{} TwitterGetArticleById(ctx, articleId).Execute()

Get article by ID



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
	articleId := "articleId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetArticleById(context.Background(), articleId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetArticleById``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetArticleById`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetArticleById`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**articleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetArticleByIdRequest struct via the builder pattern


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


## TwitterGetBroadcastDetails

> interface{} TwitterGetBroadcastDetails(ctx, broadcastId).Execute()

Get broadcast details



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
	broadcastId := "broadcastId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetBroadcastDetails(context.Background(), broadcastId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetBroadcastDetails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetBroadcastDetails`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetBroadcastDetails`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**broadcastId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetBroadcastDetailsRequest struct via the builder pattern


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


## TwitterGetCommunityDetails

> interface{} TwitterGetCommunityDetails(ctx, communityId).Execute()

Get community details



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
	communityId := "communityId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetCommunityDetails(context.Background(), communityId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetCommunityDetails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetCommunityDetails`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetCommunityDetails`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**communityId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetCommunityDetailsRequest struct via the builder pattern


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


## TwitterGetCommunityNotes

> interface{} TwitterGetCommunityNotes(ctx, tweetId).Execute()

Get community notes



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
	tweetId := "tweetId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetCommunityNotes(context.Background(), tweetId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetCommunityNotes``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetCommunityNotes`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetCommunityNotes`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tweetId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetCommunityNotesRequest struct via the builder pattern


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


## TwitterGetCommunityTweets

> interface{} TwitterGetCommunityTweets(ctx, communityId).TweetType(tweetType).Cursor(cursor).Execute()

Get community tweets



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
	communityId := "communityId_example" // string | 
	tweetType := "tweetType_example" // string |  (optional)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetCommunityTweets(context.Background(), communityId).TweetType(tweetType).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetCommunityTweets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetCommunityTweets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetCommunityTweets`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**communityId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetCommunityTweetsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **tweetType** | **string** |  | 
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


## TwitterGetFilterRule

> FilterRuleResponse TwitterGetFilterRule(ctx, ruleId).Execute()

Get filter rule



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
	ruleId := "ruleId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetFilterRule(context.Background(), ruleId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetFilterRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetFilterRule`: FilterRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetFilterRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**ruleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetFilterRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**FilterRuleResponse**](FilterRuleResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterGetFilterRulePerPollRates

> PortalApiRoutersV1TwitterFilterRulesFilterRulePricingResponse TwitterGetFilterRulePerPollRates(ctx).Execute()

Get filter rule per-poll rates



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
	resp, r, err := apiClient.TwitterAPI.TwitterGetFilterRulePerPollRates(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetFilterRulePerPollRates``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetFilterRulePerPollRates`: PortalApiRoutersV1TwitterFilterRulesFilterRulePricingResponse
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetFilterRulePerPollRates`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetFilterRulePerPollRatesRequest struct via the builder pattern


### Return type

[**PortalApiRoutersV1TwitterFilterRulesFilterRulePricingResponse**](PortalApiRoutersV1TwitterFilterRulesFilterRulePricingResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterGetListDetails

> interface{} TwitterGetListDetails(ctx, listId).Execute()

Get list details



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
	listId := "listId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetListDetails(context.Background(), listId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetListDetails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetListDetails`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetListDetails`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetListDetailsRequest struct via the builder pattern


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


## TwitterGetListTweets

> interface{} TwitterGetListTweets(ctx, listId).Cursor(cursor).Execute()

Get list tweets



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
	listId := "listId_example" // string | 
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetListTweets(context.Background(), listId).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetListTweets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetListTweets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetListTweets`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetListTweetsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

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


## TwitterGetPlaceDetails

> interface{} TwitterGetPlaceDetails(ctx, placeId).Execute()

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
	placeId := "placeId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetPlaceDetails(context.Background(), placeId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetPlaceDetails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetPlaceDetails`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetPlaceDetails`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**placeId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetPlaceDetailsRequest struct via the builder pattern


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


## TwitterGetSimilarTweets

> interface{} TwitterGetSimilarTweets(ctx, tweetId).Execute()

Get similar tweets



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
	tweetId := "tweetId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetSimilarTweets(context.Background(), tweetId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetSimilarTweets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetSimilarTweets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetSimilarTweets`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tweetId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetSimilarTweetsRequest struct via the builder pattern


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


## TwitterGetSpaceDetails

> interface{} TwitterGetSpaceDetails(ctx, spaceId).Execute()

Get Space details



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
	spaceId := "spaceId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetSpaceDetails(context.Background(), spaceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetSpaceDetails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetSpaceDetails`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetSpaceDetails`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**spaceId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetSpaceDetailsRequest struct via the builder pattern


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


## TwitterGetStreamMonitor

> StreamMonitorResponse TwitterGetStreamMonitor(ctx, monitorId).Execute()

Get stream monitor



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
	monitorId := "monitorId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetStreamMonitor(context.Background(), monitorId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetStreamMonitor``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetStreamMonitor`: StreamMonitorResponse
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetStreamMonitor`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**monitorId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetStreamMonitorRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**StreamMonitorResponse**](StreamMonitorResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterGetTrendingTopics

> interface{} TwitterGetTrendingTopics(ctx).Category(category).Count(count).Execute()

Get trending topics



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
	category := "category_example" // string |  (optional)
	count := int32(56) // int32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetTrendingTopics(context.Background()).Category(category).Count(count).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetTrendingTopics``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetTrendingTopics`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetTrendingTopics`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetTrendingTopicsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **category** | **string** |  | 
 **count** | **int32** |  | 

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


## TwitterGetTrendsByLocation

> interface{} TwitterGetTrendsByLocation(ctx, woeid).Execute()

Get trends by location



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
	woeid := "woeid_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetTrendsByLocation(context.Background(), woeid).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetTrendsByLocation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetTrendsByLocation`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetTrendsByLocation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**woeid** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetTrendsByLocationRequest struct via the builder pattern


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


## TwitterGetTweetDetails

> interface{} TwitterGetTweetDetails(ctx, tweetId).Cursor(cursor).Execute()

Get tweet details



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
	tweetId := "tweetId_example" // string | 
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetTweetDetails(context.Background(), tweetId).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetTweetDetails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetTweetDetails`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetTweetDetails`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tweetId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetTweetDetailsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

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


## TwitterGetTweetEditHistory

> interface{} TwitterGetTweetEditHistory(ctx, tweetId).Execute()

Get tweet edit history



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
	tweetId := "tweetId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetTweetEditHistory(context.Background(), tweetId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetTweetEditHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetTweetEditHistory`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetTweetEditHistory`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tweetId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetTweetEditHistoryRequest struct via the builder pattern


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


## TwitterGetTweetFavoriters

> interface{} TwitterGetTweetFavoriters(ctx, tweetId).Cursor(cursor).Execute()

Get tweet favoriters



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
	tweetId := "tweetId_example" // string | 
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetTweetFavoriters(context.Background(), tweetId).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetTweetFavoriters``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetTweetFavoriters`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetTweetFavoriters`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tweetId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetTweetFavoritersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

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


## TwitterGetTweetQuotes

> interface{} TwitterGetTweetQuotes(ctx, tweetId).Cursor(cursor).Execute()

Get tweet quotes



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
	tweetId := "tweetId_example" // string | 
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetTweetQuotes(context.Background(), tweetId).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetTweetQuotes``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetTweetQuotes`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetTweetQuotes`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tweetId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetTweetQuotesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

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


## TwitterGetTweetReplies

> interface{} TwitterGetTweetReplies(ctx, tweetId).Cursor(cursor).Execute()

Get tweet replies



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
	tweetId := "tweetId_example" // string | 
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetTweetReplies(context.Background(), tweetId).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetTweetReplies``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetTweetReplies`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetTweetReplies`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tweetId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetTweetRepliesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

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


## TwitterGetTweetRetweeters

> interface{} TwitterGetTweetRetweeters(ctx, tweetId).Cursor(cursor).Execute()

Get tweet retweeters



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
	tweetId := "tweetId_example" // string | 
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetTweetRetweeters(context.Background(), tweetId).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetTweetRetweeters``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetTweetRetweeters`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetTweetRetweeters`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**tweetId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetTweetRetweetersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

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


## TwitterGetTweetsByIds

> interface{} TwitterGetTweetsByIds(ctx).Tweets(tweets).Execute()

Get tweets by IDs



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
	tweets := "tweets_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetTweetsByIds(context.Background()).Tweets(tweets).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetTweetsByIds``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetTweetsByIds`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetTweetsByIds`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetTweetsByIdsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tweets** | **string** |  | 

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


## TwitterGetUserArticles

> interface{} TwitterGetUserArticles(ctx, userId).Cursor(cursor).Execute()

Get user articles



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
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetUserArticles(context.Background(), userId).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetUserArticles``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetUserArticles`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetUserArticles`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetUserArticlesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

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


## TwitterGetUserById

> interface{} TwitterGetUserById(ctx, userId).Execute()

Get user by ID



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
	resp, r, err := apiClient.TwitterAPI.TwitterGetUserById(context.Background(), userId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetUserById``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetUserById`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetUserById`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetUserByIdRequest struct via the builder pattern


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


## TwitterGetUserByUsername

> interface{} TwitterGetUserByUsername(ctx, username).Execute()

Get user by username



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
	resp, r, err := apiClient.TwitterAPI.TwitterGetUserByUsername(context.Background(), username).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetUserByUsername``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetUserByUsername`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetUserByUsername`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetUserByUsernameRequest struct via the builder pattern


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


## TwitterGetUserFollowers

> interface{} TwitterGetUserFollowers(ctx, username).Cursor(cursor).Execute()

Get user followers



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
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetUserFollowers(context.Background(), username).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetUserFollowers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetUserFollowers`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetUserFollowers`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetUserFollowersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

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


## TwitterGetUserFollowing

> interface{} TwitterGetUserFollowing(ctx, username).Cursor(cursor).Execute()

Get user following



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
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetUserFollowing(context.Background(), username).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetUserFollowing``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetUserFollowing`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetUserFollowing`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetUserFollowingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

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


## TwitterGetUserMentions

> interface{} TwitterGetUserMentions(ctx, username).Count(count).Cursor(cursor).Execute()

Get user mentions



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
	count := int32(56) // int32 |  (optional)
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetUserMentions(context.Background(), username).Count(count).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetUserMentions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetUserMentions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetUserMentions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetUserMentionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **count** | **int32** |  | 
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


## TwitterGetUserSubscriptions

> interface{} TwitterGetUserSubscriptions(ctx, userId).Cursor(cursor).Execute()

Get user subscriptions



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
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetUserSubscriptions(context.Background(), userId).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetUserSubscriptions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetUserSubscriptions`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetUserSubscriptions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetUserSubscriptionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

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


## TwitterGetUserTweets

> interface{} TwitterGetUserTweets(ctx, username).Cursor(cursor).Execute()

Get user tweets



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
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterGetUserTweets(context.Background(), username).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterGetUserTweets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterGetUserTweets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterGetUserTweets`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterGetUserTweetsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

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


## TwitterListBillingLogs

> BillingLogListResponse TwitterListBillingLogs(ctx).MonitorId(monitorId).Page(page).PageSize(pageSize).Execute()

List billing logs



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
	monitorId := "monitorId_example" // string |  (optional)
	page := int32(56) // int32 |  (optional) (default to 1)
	pageSize := int32(56) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterListBillingLogs(context.Background()).MonitorId(monitorId).Page(page).PageSize(pageSize).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterListBillingLogs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterListBillingLogs`: BillingLogListResponse
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterListBillingLogs`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterListBillingLogsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **monitorId** | **string** |  | 
 **page** | **int32** |  | [default to 1]
 **pageSize** | **int32** |  | [default to 20]

### Return type

[**BillingLogListResponse**](BillingLogListResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterListDeliveryLogsForAFilterRule

> FilterRuleDeliveryLogListResponse TwitterListDeliveryLogsForAFilterRule(ctx, ruleId).DeliveryStatus(deliveryStatus).AuthorUsername(authorUsername).Page(page).PageSize(pageSize).Sort(sort).Execute()

List delivery logs for a filter rule



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
	ruleId := "ruleId_example" // string | 
	deliveryStatus := "deliveryStatus_example" // string |  (optional)
	authorUsername := "authorUsername_example" // string |  (optional)
	page := int32(56) // int32 |  (optional) (default to 1)
	pageSize := int32(56) // int32 |  (optional) (default to 20)
	sort := "sort_example" // string |  (optional) (default to "desc")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterListDeliveryLogsForAFilterRule(context.Background(), ruleId).DeliveryStatus(deliveryStatus).AuthorUsername(authorUsername).Page(page).PageSize(pageSize).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterListDeliveryLogsForAFilterRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterListDeliveryLogsForAFilterRule`: FilterRuleDeliveryLogListResponse
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterListDeliveryLogsForAFilterRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**ruleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterListDeliveryLogsForAFilterRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **deliveryStatus** | **string** |  | 
 **authorUsername** | **string** |  | 
 **page** | **int32** |  | [default to 1]
 **pageSize** | **int32** |  | [default to 20]
 **sort** | **string** |  | [default to &quot;desc&quot;]

### Return type

[**FilterRuleDeliveryLogListResponse**](FilterRuleDeliveryLogListResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterListFilterRules

> FilterRuleListResponse TwitterListFilterRules(ctx).Status(status).Page(page).PageSize(pageSize).Execute()

List filter rules



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
	status := "status_example" // string |  (optional)
	page := int32(56) // int32 |  (optional) (default to 1)
	pageSize := int32(56) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterListFilterRules(context.Background()).Status(status).Page(page).PageSize(pageSize).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterListFilterRules``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterListFilterRules`: FilterRuleListResponse
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterListFilterRules`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterListFilterRulesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | **string** |  | 
 **page** | **int32** |  | [default to 1]
 **pageSize** | **int32** |  | [default to 20]

### Return type

[**FilterRuleListResponse**](FilterRuleListResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterListStreamMonitors

> StreamMonitorListResponse TwitterListStreamMonitors(ctx).Status(status).Page(page).PageSize(pageSize).Execute()

List stream monitors



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
	status := "status_example" // string |  (optional)
	page := int32(56) // int32 |  (optional) (default to 1)
	pageSize := int32(56) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterListStreamMonitors(context.Background()).Status(status).Page(page).PageSize(pageSize).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterListStreamMonitors``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterListStreamMonitors`: StreamMonitorListResponse
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterListStreamMonitors`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterListStreamMonitorsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | **string** |  | 
 **page** | **int32** |  | [default to 1]
 **pageSize** | **int32** |  | [default to 20]

### Return type

[**StreamMonitorListResponse**](StreamMonitorListResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterListTweetDeliveryLogs

> TweetDeliveryLogListResponse TwitterListTweetDeliveryLogs(ctx).MonitorId(monitorId).AuthorUsername(authorUsername).DeliveryStatus(deliveryStatus).Page(page).PageSize(pageSize).Sort(sort).Execute()

List tweet delivery logs



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
	monitorId := "monitorId_example" // string |  (optional)
	authorUsername := "authorUsername_example" // string |  (optional)
	deliveryStatus := "deliveryStatus_example" // string |  (optional)
	page := int32(56) // int32 |  (optional) (default to 1)
	pageSize := int32(56) // int32 |  (optional) (default to 20)
	sort := "sort_example" // string |  (optional) (default to "desc")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterListTweetDeliveryLogs(context.Background()).MonitorId(monitorId).AuthorUsername(authorUsername).DeliveryStatus(deliveryStatus).Page(page).PageSize(pageSize).Sort(sort).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterListTweetDeliveryLogs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterListTweetDeliveryLogs`: TweetDeliveryLogListResponse
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterListTweetDeliveryLogs`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterListTweetDeliveryLogsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **monitorId** | **string** |  | 
 **authorUsername** | **string** |  | 
 **deliveryStatus** | **string** |  | 
 **page** | **int32** |  | [default to 1]
 **pageSize** | **int32** |  | [default to 20]
 **sort** | **string** |  | [default to &quot;desc&quot;]

### Return type

[**TweetDeliveryLogListResponse**](TweetDeliveryLogListResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterListWebhooks

> WebhookListResponse TwitterListWebhooks(ctx).MonitorId(monitorId).Execute()

List webhooks



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
	monitorId := "monitorId_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterListWebhooks(context.Background()).MonitorId(monitorId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterListWebhooks``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterListWebhooks`: WebhookListResponse
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterListWebhooks`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterListWebhooksRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **monitorId** | **string** |  | 

### Return type

[**WebhookListResponse**](WebhookListResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterRemoveWebhookFromMonitor

> TwitterRemoveWebhookFromMonitor(ctx, webhookId).Execute()

Remove webhook from monitor



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
	webhookId := "webhookId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.TwitterAPI.TwitterRemoveWebhookFromMonitor(context.Background(), webhookId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterRemoveWebhookFromMonitor``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**webhookId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterRemoveWebhookFromMonitorRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterSearchCommunities

> interface{} TwitterSearchCommunities(ctx).Query(query).Cursor(cursor).Execute()

Search communities



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
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterSearchCommunities(context.Background()).Query(query).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterSearchCommunities``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterSearchCommunities`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterSearchCommunities`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterSearchCommunitiesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 
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


## TwitterSearchListTweets

> interface{} TwitterSearchListTweets(ctx, listId).Query(query).Cursor(cursor).Execute()

Search list tweets



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
	listId := "listId_example" // string | 
	query := "query_example" // string | 
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterSearchListTweets(context.Background(), listId).Query(query).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterSearchListTweets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterSearchListTweets`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterSearchListTweets`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterSearchListTweetsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **query** | **string** |  | 
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


## TwitterSearchPlaces

> interface{} TwitterSearchPlaces(ctx).Query(query).Lat(lat).Long(long).Execute()

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
	query := "query_example" // string |  (optional)
	lat := float32(8.14) // float32 |  (optional)
	long := float32(8.14) // float32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterSearchPlaces(context.Background()).Query(query).Lat(lat).Long(long).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterSearchPlaces``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterSearchPlaces`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterSearchPlaces`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterSearchPlacesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 
 **lat** | **float32** |  | 
 **long** | **float32** |  | 

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


## TwitterSearchUsers

> interface{} TwitterSearchUsers(ctx).Query(query).Cursor(cursor).Execute()

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
	cursor := "cursor_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterSearchUsers(context.Background()).Query(query).Cursor(cursor).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterSearchUsers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterSearchUsers`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterSearchUsers`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterSearchUsersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** |  | 
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


## TwitterTestWebhookDelivery

> WebhookTestResponse TwitterTestWebhookDelivery(ctx).WebhookTestRequest(webhookTestRequest).Execute()

Test webhook delivery



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
	webhookTestRequest := *openapiclient.NewWebhookTestRequest("MonitorId_example") // WebhookTestRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterTestWebhookDelivery(context.Background()).WebhookTestRequest(webhookTestRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterTestWebhookDelivery``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterTestWebhookDelivery`: WebhookTestResponse
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterTestWebhookDelivery`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterTestWebhookDeliveryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **webhookTestRequest** | [**WebhookTestRequest**](WebhookTestRequest.md) |  | 

### Return type

[**WebhookTestResponse**](WebhookTestResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterTwitterScraperHealthCheck

> interface{} TwitterTwitterScraperHealthCheck(ctx).Execute()

Twitter scraper health check



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
	resp, r, err := apiClient.TwitterAPI.TwitterTwitterScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterTwitterScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterTwitterScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterTwitterScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterTwitterScraperHealthCheckRequest struct via the builder pattern


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


## TwitterTwitterScraperHealthCheckHead

> interface{} TwitterTwitterScraperHealthCheckHead(ctx).Execute()

Twitter scraper health check



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
	resp, r, err := apiClient.TwitterAPI.TwitterTwitterScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterTwitterScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterTwitterScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterTwitterScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterTwitterScraperHealthCheckHeadRequest struct via the builder pattern


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


## TwitterUpdateFilterRule

> FilterRuleResponse TwitterUpdateFilterRule(ctx, ruleId).FilterRuleUpdate(filterRuleUpdate).Execute()

Update filter rule



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
	ruleId := "ruleId_example" // string | 
	filterRuleUpdate := *openapiclient.NewFilterRuleUpdate() // FilterRuleUpdate | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterUpdateFilterRule(context.Background(), ruleId).FilterRuleUpdate(filterRuleUpdate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterUpdateFilterRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterUpdateFilterRule`: FilterRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterUpdateFilterRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**ruleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterUpdateFilterRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filterRuleUpdate** | [**FilterRuleUpdate**](FilterRuleUpdate.md) |  | 

### Return type

[**FilterRuleResponse**](FilterRuleResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterUpdateStreamMonitor

> StreamMonitorResponse TwitterUpdateStreamMonitor(ctx, monitorId).StreamMonitorUpdate(streamMonitorUpdate).Execute()

Update stream monitor



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
	monitorId := "monitorId_example" // string | 
	streamMonitorUpdate := *openapiclient.NewStreamMonitorUpdate() // StreamMonitorUpdate | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterUpdateStreamMonitor(context.Background(), monitorId).StreamMonitorUpdate(streamMonitorUpdate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterUpdateStreamMonitor``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterUpdateStreamMonitor`: StreamMonitorResponse
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterUpdateStreamMonitor`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**monitorId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTwitterUpdateStreamMonitorRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **streamMonitorUpdate** | [**StreamMonitorUpdate**](StreamMonitorUpdate.md) |  | 

### Return type

[**StreamMonitorResponse**](StreamMonitorResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TwitterValidateSearchQuery

> FilterRuleValidateResponse TwitterValidateSearchQuery(ctx).FilterRuleValidateRequest(filterRuleValidateRequest).Execute()

Validate search query



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
	filterRuleValidateRequest := *openapiclient.NewFilterRuleValidateRequest("Query_example") // FilterRuleValidateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TwitterAPI.TwitterValidateSearchQuery(context.Background()).FilterRuleValidateRequest(filterRuleValidateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TwitterAPI.TwitterValidateSearchQuery``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TwitterValidateSearchQuery`: FilterRuleValidateResponse
	fmt.Fprintf(os.Stdout, "Response from `TwitterAPI.TwitterValidateSearchQuery`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTwitterValidateSearchQueryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filterRuleValidateRequest** | [**FilterRuleValidateRequest**](FilterRuleValidateRequest.md) |  | 

### Return type

[**FilterRuleValidateResponse**](FilterRuleValidateResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


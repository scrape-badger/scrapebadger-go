# \GitHubAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GithubGetProfile**](GitHubAPI.md#GithubGetProfile) | **Get** /v1/github/profiles/{username} | Get profile
[**GithubGetRepository**](GitHubAPI.md#GithubGetRepository) | **Get** /v1/github/repositories/{owner}/{repo} | Get repository



## GithubGetProfile

> GitHubProfileResponse GithubGetProfile(ctx, username).Tab(tab).Year(year).Page(page).NextPageToken(nextPageToken).Execute()

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
	tab := "tab_example" // string | Profile section; stars is available for users only (optional) (default to "overview")
	year := int32(56) // int32 | Overview only: 1970 through the current UTC year; activity is December or current month (optional)
	page := int32(56) // int32 | Repositories only: page number, 30 rows per page (optional)
	nextPageToken := "nextPageToken_example" // string | Stars only: previous pagination.next_page_token (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GitHubAPI.GithubGetProfile(context.Background(), username).Tab(tab).Year(year).Page(page).NextPageToken(nextPageToken).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GitHubAPI.GithubGetProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GithubGetProfile`: GitHubProfileResponse
	fmt.Fprintf(os.Stdout, "Response from `GitHubAPI.GithubGetProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**username** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGithubGetProfileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **tab** | **string** | Profile section; stars is available for users only | [default to &quot;overview&quot;]
 **year** | **int32** | Overview only: 1970 through the current UTC year; activity is December or current month | 
 **page** | **int32** | Repositories only: page number, 30 rows per page | 
 **nextPageToken** | **string** | Stars only: previous pagination.next_page_token | 

### Return type

[**GitHubProfileResponse**](GitHubProfileResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GithubGetRepository

> GitHubRepositoryResponse GithubGetRepository(ctx, owner, repo).Execute()

Get repository



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/scrape-badger/scrapebadger-go"
)

func main() {
	owner := "owner_example" // string | 
	repo := "repo_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.GitHubAPI.GithubGetRepository(context.Background(), owner, repo).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `GitHubAPI.GithubGetRepository``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GithubGetRepository`: GitHubRepositoryResponse
	fmt.Fprintf(os.Stdout, "Response from `GitHubAPI.GithubGetRepository`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**owner** | **string** |  | 
**repo** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGithubGetRepositoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**GitHubRepositoryResponse**](GitHubRepositoryResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


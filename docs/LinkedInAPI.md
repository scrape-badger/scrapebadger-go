# \LinkedInAPI

All URIs are relative to *https://scrapebadger.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**LinkedinGetACompanySJobPostings**](LinkedInAPI.md#LinkedinGetACompanySJobPostings) | **Get** /v1/linkedin/companies/{company_id}/jobs | Get a company&#39;s job postings
[**LinkedinGetACourse**](LinkedInAPI.md#LinkedinGetACourse) | **Get** /v1/linkedin/learning/{course_slug} | Get a course
[**LinkedinGetAPublicArticle**](LinkedInAPI.md#LinkedinGetAPublicArticle) | **Get** /v1/linkedin/articles/{article_slug} | Get a public article
[**LinkedinGetAPublicPost**](LinkedInAPI.md#LinkedinGetAPublicPost) | **Get** /v1/linkedin/posts/{post_slug} | Get a public post
[**LinkedinGetCompany**](LinkedInAPI.md#LinkedinGetCompany) | **Get** /v1/linkedin/companies/{universal_name} | Get company
[**LinkedinGetJobDetail**](LinkedInAPI.md#LinkedinGetJobDetail) | **Get** /v1/linkedin/jobs/{job_id} | Get job detail
[**LinkedinGetPublicProfile**](LinkedInAPI.md#LinkedinGetPublicProfile) | **Get** /v1/linkedin/profiles/{public_id} | Get public profile
[**LinkedinGetSchool**](LinkedInAPI.md#LinkedinGetSchool) | **Get** /v1/linkedin/schools/{universal_name} | Get school
[**LinkedinLinkedinScraperHealthCheck**](LinkedInAPI.md#LinkedinLinkedinScraperHealthCheck) | **Get** /v1/linkedin/health | LinkedIn scraper health check
[**LinkedinLinkedinScraperHealthCheckHead**](LinkedInAPI.md#LinkedinLinkedinScraperHealthCheckHead) | **Head** /v1/linkedin/health | LinkedIn scraper health check
[**LinkedinSearchLinkedinJobs**](LinkedInAPI.md#LinkedinSearchLinkedinJobs) | **Get** /v1/linkedin/jobs/search | Search LinkedIn jobs
[**LinkedinSuggestLocationGeoIds**](LinkedInAPI.md#LinkedinSuggestLocationGeoIds) | **Get** /v1/linkedin/geo/suggest | Suggest location geo ids



## LinkedinGetACompanySJobPostings

> interface{} LinkedinGetACompanySJobPostings(ctx, companyId).Start(start).Country(country).Execute()

Get a company's job postings



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/scrape-badger/scrapebadger-go"
)

func main() {
	companyId := "companyId_example" // string | 
	start := int32(56) // int32 | Pagination offset (0, 25, 50, ...) (optional) (default to 0)
	country := "country_example" // string | Residential proxy country (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LinkedInAPI.LinkedinGetACompanySJobPostings(context.Background(), companyId).Start(start).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LinkedInAPI.LinkedinGetACompanySJobPostings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LinkedinGetACompanySJobPostings`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LinkedInAPI.LinkedinGetACompanySJobPostings`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**companyId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiLinkedinGetACompanySJobPostingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **start** | **int32** | Pagination offset (0, 25, 50, ...) | [default to 0]
 **country** | **string** | Residential proxy country | [default to &quot;us&quot;]

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


## LinkedinGetACourse

> interface{} LinkedinGetACourse(ctx, courseSlug).Country(country).Execute()

Get a course



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/scrape-badger/scrapebadger-go"
)

func main() {
	courseSlug := "courseSlug_example" // string | 
	country := "country_example" // string | Residential proxy country (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LinkedInAPI.LinkedinGetACourse(context.Background(), courseSlug).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LinkedInAPI.LinkedinGetACourse``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LinkedinGetACourse`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LinkedInAPI.LinkedinGetACourse`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseSlug** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiLinkedinGetACourseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | Residential proxy country | [default to &quot;us&quot;]

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


## LinkedinGetAPublicArticle

> interface{} LinkedinGetAPublicArticle(ctx, articleSlug).Country(country).Execute()

Get a public article



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/scrape-badger/scrapebadger-go"
)

func main() {
	articleSlug := "articleSlug_example" // string | 
	country := "country_example" // string | Residential proxy country (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LinkedInAPI.LinkedinGetAPublicArticle(context.Background(), articleSlug).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LinkedInAPI.LinkedinGetAPublicArticle``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LinkedinGetAPublicArticle`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LinkedInAPI.LinkedinGetAPublicArticle`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**articleSlug** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiLinkedinGetAPublicArticleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | Residential proxy country | [default to &quot;us&quot;]

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


## LinkedinGetAPublicPost

> interface{} LinkedinGetAPublicPost(ctx, postSlug).Country(country).Execute()

Get a public post



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/scrape-badger/scrapebadger-go"
)

func main() {
	postSlug := "postSlug_example" // string | 
	country := "country_example" // string | Residential proxy country (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LinkedInAPI.LinkedinGetAPublicPost(context.Background(), postSlug).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LinkedInAPI.LinkedinGetAPublicPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LinkedinGetAPublicPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LinkedInAPI.LinkedinGetAPublicPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**postSlug** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiLinkedinGetAPublicPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | Residential proxy country | [default to &quot;us&quot;]

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


## LinkedinGetCompany

> interface{} LinkedinGetCompany(ctx, universalName).Country(country).Execute()

Get company



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/scrape-badger/scrapebadger-go"
)

func main() {
	universalName := "universalName_example" // string | 
	country := "country_example" // string | Residential proxy country (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LinkedInAPI.LinkedinGetCompany(context.Background(), universalName).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LinkedInAPI.LinkedinGetCompany``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LinkedinGetCompany`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LinkedInAPI.LinkedinGetCompany`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**universalName** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiLinkedinGetCompanyRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | Residential proxy country | [default to &quot;us&quot;]

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


## LinkedinGetJobDetail

> interface{} LinkedinGetJobDetail(ctx, jobId).Country(country).Execute()

Get job detail



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/scrape-badger/scrapebadger-go"
)

func main() {
	jobId := "jobId_example" // string | 
	country := "country_example" // string | Residential proxy country (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LinkedInAPI.LinkedinGetJobDetail(context.Background(), jobId).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LinkedInAPI.LinkedinGetJobDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LinkedinGetJobDetail`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LinkedInAPI.LinkedinGetJobDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**jobId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiLinkedinGetJobDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | Residential proxy country | [default to &quot;us&quot;]

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


## LinkedinGetPublicProfile

> interface{} LinkedinGetPublicProfile(ctx, publicId).Country(country).Execute()

Get public profile



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/scrape-badger/scrapebadger-go"
)

func main() {
	publicId := "publicId_example" // string | 
	country := "country_example" // string | Residential proxy country (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LinkedInAPI.LinkedinGetPublicProfile(context.Background(), publicId).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LinkedInAPI.LinkedinGetPublicProfile``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LinkedinGetPublicProfile`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LinkedInAPI.LinkedinGetPublicProfile`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**publicId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiLinkedinGetPublicProfileRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | Residential proxy country | [default to &quot;us&quot;]

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


## LinkedinGetSchool

> interface{} LinkedinGetSchool(ctx, universalName).Country(country).Execute()

Get school



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/scrape-badger/scrapebadger-go"
)

func main() {
	universalName := "universalName_example" // string | 
	country := "country_example" // string | Residential proxy country (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LinkedInAPI.LinkedinGetSchool(context.Background(), universalName).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LinkedInAPI.LinkedinGetSchool``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LinkedinGetSchool`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LinkedInAPI.LinkedinGetSchool`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**universalName** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiLinkedinGetSchoolRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **country** | **string** | Residential proxy country | [default to &quot;us&quot;]

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


## LinkedinLinkedinScraperHealthCheck

> interface{} LinkedinLinkedinScraperHealthCheck(ctx).Execute()

LinkedIn scraper health check



### Example

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
	resp, r, err := apiClient.LinkedInAPI.LinkedinLinkedinScraperHealthCheck(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LinkedInAPI.LinkedinLinkedinScraperHealthCheck``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LinkedinLinkedinScraperHealthCheck`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LinkedInAPI.LinkedinLinkedinScraperHealthCheck`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiLinkedinLinkedinScraperHealthCheckRequest struct via the builder pattern


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


## LinkedinLinkedinScraperHealthCheckHead

> interface{} LinkedinLinkedinScraperHealthCheckHead(ctx).Execute()

LinkedIn scraper health check



### Example

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
	resp, r, err := apiClient.LinkedInAPI.LinkedinLinkedinScraperHealthCheckHead(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LinkedInAPI.LinkedinLinkedinScraperHealthCheckHead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LinkedinLinkedinScraperHealthCheckHead`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LinkedInAPI.LinkedinLinkedinScraperHealthCheckHead`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiLinkedinLinkedinScraperHealthCheckHeadRequest struct via the builder pattern


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


## LinkedinSearchLinkedinJobs

> interface{} LinkedinSearchLinkedinJobs(ctx).Keywords(keywords).Location(location).GeoId(geoId).CompanyId(companyId).DatePosted(datePosted).Experience(experience).JobType(jobType).Workplace(workplace).Sort(sort).Start(start).Country(country).Execute()

Search LinkedIn jobs



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/scrape-badger/scrapebadger-go"
)

func main() {
	keywords := "keywords_example" // string | Job title / keywords (optional)
	location := "location_example" // string | Location text, e.g. 'New York' (optional)
	geoId := "geoId_example" // string | LinkedIn numeric geo id (overrides location) (optional)
	companyId := "companyId_example" // string | Restrict to a company (numeric id) (optional)
	datePosted := "datePosted_example" // string | past_24h | past_week | past_month | any (optional)
	experience := "experience_example" // string | internship|entry|associate|mid_senior|director|executive (comma-separated) (optional)
	jobType := "jobType_example" // string | full_time|part_time|contract|temporary|internship|volunteer|other (optional)
	workplace := "workplace_example" // string | onsite|remote|hybrid (comma-separated) (optional)
	sort := "sort_example" // string | relevant | recent (optional)
	start := int32(56) // int32 | Pagination offset (0, 25, 50, ...) (optional) (default to 0)
	country := "country_example" // string | Residential proxy country (optional) (default to "us")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LinkedInAPI.LinkedinSearchLinkedinJobs(context.Background()).Keywords(keywords).Location(location).GeoId(geoId).CompanyId(companyId).DatePosted(datePosted).Experience(experience).JobType(jobType).Workplace(workplace).Sort(sort).Start(start).Country(country).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LinkedInAPI.LinkedinSearchLinkedinJobs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LinkedinSearchLinkedinJobs`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LinkedInAPI.LinkedinSearchLinkedinJobs`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiLinkedinSearchLinkedinJobsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **keywords** | **string** | Job title / keywords | 
 **location** | **string** | Location text, e.g. &#39;New York&#39; | 
 **geoId** | **string** | LinkedIn numeric geo id (overrides location) | 
 **companyId** | **string** | Restrict to a company (numeric id) | 
 **datePosted** | **string** | past_24h | past_week | past_month | any | 
 **experience** | **string** | internship|entry|associate|mid_senior|director|executive (comma-separated) | 
 **jobType** | **string** | full_time|part_time|contract|temporary|internship|volunteer|other | 
 **workplace** | **string** | onsite|remote|hybrid (comma-separated) | 
 **sort** | **string** | relevant | recent | 
 **start** | **int32** | Pagination offset (0, 25, 50, ...) | [default to 0]
 **country** | **string** | Residential proxy country | [default to &quot;us&quot;]

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


## LinkedinSuggestLocationGeoIds

> interface{} LinkedinSuggestLocationGeoIds(ctx).Query(query).Type_(type_).Execute()

Suggest location geo ids



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/scrape-badger/scrapebadger-go"
)

func main() {
	query := "query_example" // string | Location text, e.g. 'London'
	type_ := "type__example" // string | geo | company (optional) (default to "geo")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LinkedInAPI.LinkedinSuggestLocationGeoIds(context.Background()).Query(query).Type_(type_).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LinkedInAPI.LinkedinSuggestLocationGeoIds``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `LinkedinSuggestLocationGeoIds`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `LinkedInAPI.LinkedinSuggestLocationGeoIds`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiLinkedinSuggestLocationGeoIdsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **string** | Location text, e.g. &#39;London&#39; | 
 **type_** | **string** | geo | company | [default to &quot;geo&quot;]

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


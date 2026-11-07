# BraveResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Position** | **int32** |  | 
**Title** | **string** |  | 
**Url** | **string** |  | 
**Snippet** | Pointer to [**Snippet**](Snippet.md) |  | [optional] 
**Description** | Pointer to [**Description**](Description.md) |  | [optional] 
**DisplayUrl** | Pointer to [**DisplayUrl**](DisplayUrl.md) |  | [optional] 
**SiteName** | Pointer to [**SiteName**](SiteName.md) |  | [optional] 
**Language** | Pointer to [**Language**](Language.md) |  | [optional] 
**Type** | Pointer to [**Type**](Type.md) |  | [optional] 
**Subtype** | Pointer to [**Subtype**](Subtype.md) |  | [optional] 
**IsLive** | Pointer to [**IsLive**](IsLive.md) |  | [optional] 
**Profile** | Pointer to [**Profile**](Profile.md) |  | [optional] 
**MetaUrl** | Pointer to [**MetaUrl**](MetaUrl.md) |  | [optional] 
**Thumbnail** | Pointer to [**Thumbnail**](Thumbnail.md) |  | [optional] 
**Age** | Pointer to [**Age**](Age.md) |  | [optional] 
**PageAge** | Pointer to [**PageAge**](PageAge.md) |  | [optional] 
**PublishedAt** | Pointer to [**PublishedAt**](PublishedAt.md) |  | [optional] 
**PublishedUtc** | Pointer to [**PublishedUtc**](PublishedUtc.md) |  | [optional] 
**PageFetched** | Pointer to [**PageFetched**](PageFetched.md) |  | [optional] 
**PageFetchedAt** | Pointer to [**PageFetchedAt**](PageFetchedAt.md) |  | [optional] 
**PageFetchedUtc** | Pointer to [**PageFetchedUtc**](PageFetchedUtc.md) |  | [optional] 
**Sitelinks** | Pointer to **[]map[string]interface{}** |  | [optional] 
**Article** | Pointer to [**Article**](Article.md) |  | [optional] 
**Book** | Pointer to [**Book**](Book.md) |  | [optional] 
**Organization** | Pointer to [**Organization**](Organization.md) |  | [optional] 
**Location** | Pointer to [**Location**](Location.md) |  | [optional] 
**Product** | Pointer to [**Product1**](Product1.md) |  | [optional] 
**ProductCluster** | Pointer to [**ProductCluster**](ProductCluster.md) |  | [optional] 
**Rating** | Pointer to [**Rating**](Rating.md) |  | [optional] 
**Recipe** | Pointer to [**Recipe**](Recipe.md) |  | [optional] 
**Review** | Pointer to [**Review**](Review.md) |  | [optional] 
**Software** | Pointer to [**Software**](Software.md) |  | [optional] 
**Faq** | Pointer to [**Faq**](Faq.md) |  | [optional] 
**Qa** | Pointer to [**Qa**](Qa.md) |  | [optional] 
**DeepResults** | Pointer to [**DeepResults**](DeepResults.md) |  | [optional] 
**Cluster** | Pointer to [**Cluster**](Cluster.md) |  | [optional] 
**Video** | Pointer to [**Video**](Video.md) |  | [optional] 
**Properties** | Pointer to [**Properties**](Properties.md) |  | [optional] 
**Data** | Pointer to [**Data**](Data.md) |  | [optional] 
**FamilyFriendly** | Pointer to [**FamilyFriendly**](FamilyFriendly.md) |  | [optional] 
**Confidence** | Pointer to [**Confidence**](Confidence.md) |  | [optional] 
**Source** | Pointer to [**Source**](Source.md) |  | [optional] 

## Methods

### NewBraveResult

`func NewBraveResult(position int32, title string, url string, ) *BraveResult`

NewBraveResult instantiates a new BraveResult object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBraveResultWithDefaults

`func NewBraveResultWithDefaults() *BraveResult`

NewBraveResultWithDefaults instantiates a new BraveResult object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPosition

`func (o *BraveResult) GetPosition() int32`

GetPosition returns the Position field if non-nil, zero value otherwise.

### GetPositionOk

`func (o *BraveResult) GetPositionOk() (*int32, bool)`

GetPositionOk returns a tuple with the Position field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPosition

`func (o *BraveResult) SetPosition(v int32)`

SetPosition sets Position field to given value.


### GetTitle

`func (o *BraveResult) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *BraveResult) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *BraveResult) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetUrl

`func (o *BraveResult) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *BraveResult) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *BraveResult) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetSnippet

`func (o *BraveResult) GetSnippet() Snippet`

GetSnippet returns the Snippet field if non-nil, zero value otherwise.

### GetSnippetOk

`func (o *BraveResult) GetSnippetOk() (*Snippet, bool)`

GetSnippetOk returns a tuple with the Snippet field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSnippet

`func (o *BraveResult) SetSnippet(v Snippet)`

SetSnippet sets Snippet field to given value.

### HasSnippet

`func (o *BraveResult) HasSnippet() bool`

HasSnippet returns a boolean if a field has been set.

### GetDescription

`func (o *BraveResult) GetDescription() Description`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *BraveResult) GetDescriptionOk() (*Description, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *BraveResult) SetDescription(v Description)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *BraveResult) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetDisplayUrl

`func (o *BraveResult) GetDisplayUrl() DisplayUrl`

GetDisplayUrl returns the DisplayUrl field if non-nil, zero value otherwise.

### GetDisplayUrlOk

`func (o *BraveResult) GetDisplayUrlOk() (*DisplayUrl, bool)`

GetDisplayUrlOk returns a tuple with the DisplayUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayUrl

`func (o *BraveResult) SetDisplayUrl(v DisplayUrl)`

SetDisplayUrl sets DisplayUrl field to given value.

### HasDisplayUrl

`func (o *BraveResult) HasDisplayUrl() bool`

HasDisplayUrl returns a boolean if a field has been set.

### GetSiteName

`func (o *BraveResult) GetSiteName() SiteName`

GetSiteName returns the SiteName field if non-nil, zero value otherwise.

### GetSiteNameOk

`func (o *BraveResult) GetSiteNameOk() (*SiteName, bool)`

GetSiteNameOk returns a tuple with the SiteName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSiteName

`func (o *BraveResult) SetSiteName(v SiteName)`

SetSiteName sets SiteName field to given value.

### HasSiteName

`func (o *BraveResult) HasSiteName() bool`

HasSiteName returns a boolean if a field has been set.

### GetLanguage

`func (o *BraveResult) GetLanguage() Language`

GetLanguage returns the Language field if non-nil, zero value otherwise.

### GetLanguageOk

`func (o *BraveResult) GetLanguageOk() (*Language, bool)`

GetLanguageOk returns a tuple with the Language field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLanguage

`func (o *BraveResult) SetLanguage(v Language)`

SetLanguage sets Language field to given value.

### HasLanguage

`func (o *BraveResult) HasLanguage() bool`

HasLanguage returns a boolean if a field has been set.

### GetType

`func (o *BraveResult) GetType() Type`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *BraveResult) GetTypeOk() (*Type, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *BraveResult) SetType(v Type)`

SetType sets Type field to given value.

### HasType

`func (o *BraveResult) HasType() bool`

HasType returns a boolean if a field has been set.

### GetSubtype

`func (o *BraveResult) GetSubtype() Subtype`

GetSubtype returns the Subtype field if non-nil, zero value otherwise.

### GetSubtypeOk

`func (o *BraveResult) GetSubtypeOk() (*Subtype, bool)`

GetSubtypeOk returns a tuple with the Subtype field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubtype

`func (o *BraveResult) SetSubtype(v Subtype)`

SetSubtype sets Subtype field to given value.

### HasSubtype

`func (o *BraveResult) HasSubtype() bool`

HasSubtype returns a boolean if a field has been set.

### GetIsLive

`func (o *BraveResult) GetIsLive() IsLive`

GetIsLive returns the IsLive field if non-nil, zero value otherwise.

### GetIsLiveOk

`func (o *BraveResult) GetIsLiveOk() (*IsLive, bool)`

GetIsLiveOk returns a tuple with the IsLive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsLive

`func (o *BraveResult) SetIsLive(v IsLive)`

SetIsLive sets IsLive field to given value.

### HasIsLive

`func (o *BraveResult) HasIsLive() bool`

HasIsLive returns a boolean if a field has been set.

### GetProfile

`func (o *BraveResult) GetProfile() Profile`

GetProfile returns the Profile field if non-nil, zero value otherwise.

### GetProfileOk

`func (o *BraveResult) GetProfileOk() (*Profile, bool)`

GetProfileOk returns a tuple with the Profile field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProfile

`func (o *BraveResult) SetProfile(v Profile)`

SetProfile sets Profile field to given value.

### HasProfile

`func (o *BraveResult) HasProfile() bool`

HasProfile returns a boolean if a field has been set.

### GetMetaUrl

`func (o *BraveResult) GetMetaUrl() MetaUrl`

GetMetaUrl returns the MetaUrl field if non-nil, zero value otherwise.

### GetMetaUrlOk

`func (o *BraveResult) GetMetaUrlOk() (*MetaUrl, bool)`

GetMetaUrlOk returns a tuple with the MetaUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetaUrl

`func (o *BraveResult) SetMetaUrl(v MetaUrl)`

SetMetaUrl sets MetaUrl field to given value.

### HasMetaUrl

`func (o *BraveResult) HasMetaUrl() bool`

HasMetaUrl returns a boolean if a field has been set.

### GetThumbnail

`func (o *BraveResult) GetThumbnail() Thumbnail`

GetThumbnail returns the Thumbnail field if non-nil, zero value otherwise.

### GetThumbnailOk

`func (o *BraveResult) GetThumbnailOk() (*Thumbnail, bool)`

GetThumbnailOk returns a tuple with the Thumbnail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThumbnail

`func (o *BraveResult) SetThumbnail(v Thumbnail)`

SetThumbnail sets Thumbnail field to given value.

### HasThumbnail

`func (o *BraveResult) HasThumbnail() bool`

HasThumbnail returns a boolean if a field has been set.

### GetAge

`func (o *BraveResult) GetAge() Age`

GetAge returns the Age field if non-nil, zero value otherwise.

### GetAgeOk

`func (o *BraveResult) GetAgeOk() (*Age, bool)`

GetAgeOk returns a tuple with the Age field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAge

`func (o *BraveResult) SetAge(v Age)`

SetAge sets Age field to given value.

### HasAge

`func (o *BraveResult) HasAge() bool`

HasAge returns a boolean if a field has been set.

### GetPageAge

`func (o *BraveResult) GetPageAge() PageAge`

GetPageAge returns the PageAge field if non-nil, zero value otherwise.

### GetPageAgeOk

`func (o *BraveResult) GetPageAgeOk() (*PageAge, bool)`

GetPageAgeOk returns a tuple with the PageAge field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageAge

`func (o *BraveResult) SetPageAge(v PageAge)`

SetPageAge sets PageAge field to given value.

### HasPageAge

`func (o *BraveResult) HasPageAge() bool`

HasPageAge returns a boolean if a field has been set.

### GetPublishedAt

`func (o *BraveResult) GetPublishedAt() PublishedAt`

GetPublishedAt returns the PublishedAt field if non-nil, zero value otherwise.

### GetPublishedAtOk

`func (o *BraveResult) GetPublishedAtOk() (*PublishedAt, bool)`

GetPublishedAtOk returns a tuple with the PublishedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPublishedAt

`func (o *BraveResult) SetPublishedAt(v PublishedAt)`

SetPublishedAt sets PublishedAt field to given value.

### HasPublishedAt

`func (o *BraveResult) HasPublishedAt() bool`

HasPublishedAt returns a boolean if a field has been set.

### GetPublishedUtc

`func (o *BraveResult) GetPublishedUtc() PublishedUtc`

GetPublishedUtc returns the PublishedUtc field if non-nil, zero value otherwise.

### GetPublishedUtcOk

`func (o *BraveResult) GetPublishedUtcOk() (*PublishedUtc, bool)`

GetPublishedUtcOk returns a tuple with the PublishedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPublishedUtc

`func (o *BraveResult) SetPublishedUtc(v PublishedUtc)`

SetPublishedUtc sets PublishedUtc field to given value.

### HasPublishedUtc

`func (o *BraveResult) HasPublishedUtc() bool`

HasPublishedUtc returns a boolean if a field has been set.

### GetPageFetched

`func (o *BraveResult) GetPageFetched() PageFetched`

GetPageFetched returns the PageFetched field if non-nil, zero value otherwise.

### GetPageFetchedOk

`func (o *BraveResult) GetPageFetchedOk() (*PageFetched, bool)`

GetPageFetchedOk returns a tuple with the PageFetched field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageFetched

`func (o *BraveResult) SetPageFetched(v PageFetched)`

SetPageFetched sets PageFetched field to given value.

### HasPageFetched

`func (o *BraveResult) HasPageFetched() bool`

HasPageFetched returns a boolean if a field has been set.

### GetPageFetchedAt

`func (o *BraveResult) GetPageFetchedAt() PageFetchedAt`

GetPageFetchedAt returns the PageFetchedAt field if non-nil, zero value otherwise.

### GetPageFetchedAtOk

`func (o *BraveResult) GetPageFetchedAtOk() (*PageFetchedAt, bool)`

GetPageFetchedAtOk returns a tuple with the PageFetchedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageFetchedAt

`func (o *BraveResult) SetPageFetchedAt(v PageFetchedAt)`

SetPageFetchedAt sets PageFetchedAt field to given value.

### HasPageFetchedAt

`func (o *BraveResult) HasPageFetchedAt() bool`

HasPageFetchedAt returns a boolean if a field has been set.

### GetPageFetchedUtc

`func (o *BraveResult) GetPageFetchedUtc() PageFetchedUtc`

GetPageFetchedUtc returns the PageFetchedUtc field if non-nil, zero value otherwise.

### GetPageFetchedUtcOk

`func (o *BraveResult) GetPageFetchedUtcOk() (*PageFetchedUtc, bool)`

GetPageFetchedUtcOk returns a tuple with the PageFetchedUtc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageFetchedUtc

`func (o *BraveResult) SetPageFetchedUtc(v PageFetchedUtc)`

SetPageFetchedUtc sets PageFetchedUtc field to given value.

### HasPageFetchedUtc

`func (o *BraveResult) HasPageFetchedUtc() bool`

HasPageFetchedUtc returns a boolean if a field has been set.

### GetSitelinks

`func (o *BraveResult) GetSitelinks() []*map[string]interface{}`

GetSitelinks returns the Sitelinks field if non-nil, zero value otherwise.

### GetSitelinksOk

`func (o *BraveResult) GetSitelinksOk() (*[]*map[string]interface{}, bool)`

GetSitelinksOk returns a tuple with the Sitelinks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSitelinks

`func (o *BraveResult) SetSitelinks(v []*map[string]interface{})`

SetSitelinks sets Sitelinks field to given value.

### HasSitelinks

`func (o *BraveResult) HasSitelinks() bool`

HasSitelinks returns a boolean if a field has been set.

### GetArticle

`func (o *BraveResult) GetArticle() Article`

GetArticle returns the Article field if non-nil, zero value otherwise.

### GetArticleOk

`func (o *BraveResult) GetArticleOk() (*Article, bool)`

GetArticleOk returns a tuple with the Article field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArticle

`func (o *BraveResult) SetArticle(v Article)`

SetArticle sets Article field to given value.

### HasArticle

`func (o *BraveResult) HasArticle() bool`

HasArticle returns a boolean if a field has been set.

### GetBook

`func (o *BraveResult) GetBook() Book`

GetBook returns the Book field if non-nil, zero value otherwise.

### GetBookOk

`func (o *BraveResult) GetBookOk() (*Book, bool)`

GetBookOk returns a tuple with the Book field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBook

`func (o *BraveResult) SetBook(v Book)`

SetBook sets Book field to given value.

### HasBook

`func (o *BraveResult) HasBook() bool`

HasBook returns a boolean if a field has been set.

### GetOrganization

`func (o *BraveResult) GetOrganization() Organization`

GetOrganization returns the Organization field if non-nil, zero value otherwise.

### GetOrganizationOk

`func (o *BraveResult) GetOrganizationOk() (*Organization, bool)`

GetOrganizationOk returns a tuple with the Organization field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganization

`func (o *BraveResult) SetOrganization(v Organization)`

SetOrganization sets Organization field to given value.

### HasOrganization

`func (o *BraveResult) HasOrganization() bool`

HasOrganization returns a boolean if a field has been set.

### GetLocation

`func (o *BraveResult) GetLocation() Location`

GetLocation returns the Location field if non-nil, zero value otherwise.

### GetLocationOk

`func (o *BraveResult) GetLocationOk() (*Location, bool)`

GetLocationOk returns a tuple with the Location field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocation

`func (o *BraveResult) SetLocation(v Location)`

SetLocation sets Location field to given value.

### HasLocation

`func (o *BraveResult) HasLocation() bool`

HasLocation returns a boolean if a field has been set.

### GetProduct

`func (o *BraveResult) GetProduct() Product1`

GetProduct returns the Product field if non-nil, zero value otherwise.

### GetProductOk

`func (o *BraveResult) GetProductOk() (*Product1, bool)`

GetProductOk returns a tuple with the Product field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProduct

`func (o *BraveResult) SetProduct(v Product1)`

SetProduct sets Product field to given value.

### HasProduct

`func (o *BraveResult) HasProduct() bool`

HasProduct returns a boolean if a field has been set.

### GetProductCluster

`func (o *BraveResult) GetProductCluster() ProductCluster`

GetProductCluster returns the ProductCluster field if non-nil, zero value otherwise.

### GetProductClusterOk

`func (o *BraveResult) GetProductClusterOk() (*ProductCluster, bool)`

GetProductClusterOk returns a tuple with the ProductCluster field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductCluster

`func (o *BraveResult) SetProductCluster(v ProductCluster)`

SetProductCluster sets ProductCluster field to given value.

### HasProductCluster

`func (o *BraveResult) HasProductCluster() bool`

HasProductCluster returns a boolean if a field has been set.

### GetRating

`func (o *BraveResult) GetRating() Rating`

GetRating returns the Rating field if non-nil, zero value otherwise.

### GetRatingOk

`func (o *BraveResult) GetRatingOk() (*Rating, bool)`

GetRatingOk returns a tuple with the Rating field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRating

`func (o *BraveResult) SetRating(v Rating)`

SetRating sets Rating field to given value.

### HasRating

`func (o *BraveResult) HasRating() bool`

HasRating returns a boolean if a field has been set.

### GetRecipe

`func (o *BraveResult) GetRecipe() Recipe`

GetRecipe returns the Recipe field if non-nil, zero value otherwise.

### GetRecipeOk

`func (o *BraveResult) GetRecipeOk() (*Recipe, bool)`

GetRecipeOk returns a tuple with the Recipe field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecipe

`func (o *BraveResult) SetRecipe(v Recipe)`

SetRecipe sets Recipe field to given value.

### HasRecipe

`func (o *BraveResult) HasRecipe() bool`

HasRecipe returns a boolean if a field has been set.

### GetReview

`func (o *BraveResult) GetReview() Review`

GetReview returns the Review field if non-nil, zero value otherwise.

### GetReviewOk

`func (o *BraveResult) GetReviewOk() (*Review, bool)`

GetReviewOk returns a tuple with the Review field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReview

`func (o *BraveResult) SetReview(v Review)`

SetReview sets Review field to given value.

### HasReview

`func (o *BraveResult) HasReview() bool`

HasReview returns a boolean if a field has been set.

### GetSoftware

`func (o *BraveResult) GetSoftware() Software`

GetSoftware returns the Software field if non-nil, zero value otherwise.

### GetSoftwareOk

`func (o *BraveResult) GetSoftwareOk() (*Software, bool)`

GetSoftwareOk returns a tuple with the Software field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSoftware

`func (o *BraveResult) SetSoftware(v Software)`

SetSoftware sets Software field to given value.

### HasSoftware

`func (o *BraveResult) HasSoftware() bool`

HasSoftware returns a boolean if a field has been set.

### GetFaq

`func (o *BraveResult) GetFaq() Faq`

GetFaq returns the Faq field if non-nil, zero value otherwise.

### GetFaqOk

`func (o *BraveResult) GetFaqOk() (*Faq, bool)`

GetFaqOk returns a tuple with the Faq field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFaq

`func (o *BraveResult) SetFaq(v Faq)`

SetFaq sets Faq field to given value.

### HasFaq

`func (o *BraveResult) HasFaq() bool`

HasFaq returns a boolean if a field has been set.

### GetQa

`func (o *BraveResult) GetQa() Qa`

GetQa returns the Qa field if non-nil, zero value otherwise.

### GetQaOk

`func (o *BraveResult) GetQaOk() (*Qa, bool)`

GetQaOk returns a tuple with the Qa field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQa

`func (o *BraveResult) SetQa(v Qa)`

SetQa sets Qa field to given value.

### HasQa

`func (o *BraveResult) HasQa() bool`

HasQa returns a boolean if a field has been set.

### GetDeepResults

`func (o *BraveResult) GetDeepResults() DeepResults`

GetDeepResults returns the DeepResults field if non-nil, zero value otherwise.

### GetDeepResultsOk

`func (o *BraveResult) GetDeepResultsOk() (*DeepResults, bool)`

GetDeepResultsOk returns a tuple with the DeepResults field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeepResults

`func (o *BraveResult) SetDeepResults(v DeepResults)`

SetDeepResults sets DeepResults field to given value.

### HasDeepResults

`func (o *BraveResult) HasDeepResults() bool`

HasDeepResults returns a boolean if a field has been set.

### GetCluster

`func (o *BraveResult) GetCluster() Cluster`

GetCluster returns the Cluster field if non-nil, zero value otherwise.

### GetClusterOk

`func (o *BraveResult) GetClusterOk() (*Cluster, bool)`

GetClusterOk returns a tuple with the Cluster field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCluster

`func (o *BraveResult) SetCluster(v Cluster)`

SetCluster sets Cluster field to given value.

### HasCluster

`func (o *BraveResult) HasCluster() bool`

HasCluster returns a boolean if a field has been set.

### GetVideo

`func (o *BraveResult) GetVideo() Video`

GetVideo returns the Video field if non-nil, zero value otherwise.

### GetVideoOk

`func (o *BraveResult) GetVideoOk() (*Video, bool)`

GetVideoOk returns a tuple with the Video field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVideo

`func (o *BraveResult) SetVideo(v Video)`

SetVideo sets Video field to given value.

### HasVideo

`func (o *BraveResult) HasVideo() bool`

HasVideo returns a boolean if a field has been set.

### GetProperties

`func (o *BraveResult) GetProperties() Properties`

GetProperties returns the Properties field if non-nil, zero value otherwise.

### GetPropertiesOk

`func (o *BraveResult) GetPropertiesOk() (*Properties, bool)`

GetPropertiesOk returns a tuple with the Properties field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProperties

`func (o *BraveResult) SetProperties(v Properties)`

SetProperties sets Properties field to given value.

### HasProperties

`func (o *BraveResult) HasProperties() bool`

HasProperties returns a boolean if a field has been set.

### GetData

`func (o *BraveResult) GetData() Data`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *BraveResult) GetDataOk() (*Data, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *BraveResult) SetData(v Data)`

SetData sets Data field to given value.

### HasData

`func (o *BraveResult) HasData() bool`

HasData returns a boolean if a field has been set.

### GetFamilyFriendly

`func (o *BraveResult) GetFamilyFriendly() FamilyFriendly`

GetFamilyFriendly returns the FamilyFriendly field if non-nil, zero value otherwise.

### GetFamilyFriendlyOk

`func (o *BraveResult) GetFamilyFriendlyOk() (*FamilyFriendly, bool)`

GetFamilyFriendlyOk returns a tuple with the FamilyFriendly field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFamilyFriendly

`func (o *BraveResult) SetFamilyFriendly(v FamilyFriendly)`

SetFamilyFriendly sets FamilyFriendly field to given value.

### HasFamilyFriendly

`func (o *BraveResult) HasFamilyFriendly() bool`

HasFamilyFriendly returns a boolean if a field has been set.

### GetConfidence

`func (o *BraveResult) GetConfidence() Confidence`

GetConfidence returns the Confidence field if non-nil, zero value otherwise.

### GetConfidenceOk

`func (o *BraveResult) GetConfidenceOk() (*Confidence, bool)`

GetConfidenceOk returns a tuple with the Confidence field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfidence

`func (o *BraveResult) SetConfidence(v Confidence)`

SetConfidence sets Confidence field to given value.

### HasConfidence

`func (o *BraveResult) HasConfidence() bool`

HasConfidence returns a boolean if a field has been set.

### GetSource

`func (o *BraveResult) GetSource() Source`

GetSource returns the Source field if non-nil, zero value otherwise.

### GetSourceOk

`func (o *BraveResult) GetSourceOk() (*Source, bool)`

GetSourceOk returns a tuple with the Source field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSource

`func (o *BraveResult) SetSource(v Source)`

SetSource sets Source field to given value.

### HasSource

`func (o *BraveResult) HasSource() bool`

HasSource returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



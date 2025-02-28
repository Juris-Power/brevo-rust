# \ExternalFeedsApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_external_feed**](ExternalFeedsApi.md#create_external_feed) | **POST** /feeds | Create an external feed
[**delete_external_feed**](ExternalFeedsApi.md#delete_external_feed) | **DELETE** /feeds/{uuid} | Delete an external feed
[**get_all_external_feeds**](ExternalFeedsApi.md#get_all_external_feeds) | **GET** /feeds | Fetch all external feeds
[**get_external_feed_by_uuid**](ExternalFeedsApi.md#get_external_feed_by_uuid) | **GET** /feeds/{uuid} | Get an external feed by UUID
[**update_external_feed**](ExternalFeedsApi.md#update_external_feed) | **PUT** /feeds/{uuid} | Update an external feed



## create_external_feed

> models::CreateExternalFeed201Response create_external_feed(create_external_feed)
Create an external feed

This endpoint will create an external feed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_external_feed** | [**CreateExternalFeed**](CreateExternalFeed.md) | Values to create a feed | [required] |

### Return type

[**models::CreateExternalFeed201Response**](createExternalFeed_201_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_external_feed

> delete_external_feed(uuid)
Delete an external feed

This endpoint will delete an external feed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **String** | UUID of the feed to delete | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_all_external_feeds

> models::GetAllExternalFeeds get_all_external_feeds(search, start_date, end_date, sort, auth_type, limit, offset)
Fetch all external feeds

This endpoint can fetch all created external feeds.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**search** | Option<**String**> | Can be used to filter records by search keyword on feed name |  |
**start_date** | Option<**String**> | Mandatory if `endDate` is used. Starting date (YYYY-MM-DD) from which you want to fetch the list. Can be maximum 30 days older than current date. |  |
**end_date** | Option<**String**> | Mandatory if `startDate` is used. Ending date (YYYY-MM-DD) till which you want to fetch the list. Maximum time period that can be selected is one month. |  |
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed. |  |[default to desc]
**auth_type** | Option<**String**> | Filter the records by `authType` of the feed. |  |
**limit** | Option<**i64**> | Number of documents returned per page. |  |[default to 50]
**offset** | Option<**i64**> | Index of the first document on the page. |  |[default to 0]

### Return type

[**models::GetAllExternalFeeds**](getAllExternalFeeds.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_external_feed_by_uuid

> models::GetExternalFeedByUuid get_external_feed_by_uuid(uuid)
Get an external feed by UUID

This endpoint will update an external feed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **String** | UUID of the feed to fetch | [required] |

### Return type

[**models::GetExternalFeedByUuid**](getExternalFeedByUUID.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_external_feed

> update_external_feed(uuid, update_external_feed)
Update an external feed

This endpoint will update an external feed.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **String** | UUID of the feed to update | [required] |
**update_external_feed** | [**UpdateExternalFeed**](UpdateExternalFeed.md) | Values to update a feed | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


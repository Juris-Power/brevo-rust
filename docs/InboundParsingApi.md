# \InboundParsingApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_inbound_email_attachment**](InboundParsingApi.md#get_inbound_email_attachment) | **GET** /inbound/attachments/{downloadToken} | Retrieve inbound attachment with download token.
[**get_inbound_email_events**](InboundParsingApi.md#get_inbound_email_events) | **GET** /inbound/events | Get the list of all the events for the received emails.
[**get_inbound_email_events_by_uuid**](InboundParsingApi.md#get_inbound_email_events_by_uuid) | **GET** /inbound/events/{uuid} | Fetch all events history for one particular received email.



## get_inbound_email_attachment

> std::path::PathBuf get_inbound_email_attachment(download_token)
Retrieve inbound attachment with download token.

This endpoint will retrieve inbound attachment with download token.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**download_token** | **String** | Token to fetch a particular attachment | [required] |

### Return type

[**std::path::PathBuf**](std::path::PathBuf.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_inbound_email_events

> models::GetInboundEmailEvents get_inbound_email_events(sender, start_date, end_date, limit, offset, sort)
Get the list of all the events for the received emails.

This endpoint will show the list of all the events for the received emails.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**sender** | Option<**String**> | Email address of the sender. |  |
**start_date** | Option<**String**> | Mandatory if endDate is used. Starting date (YYYY-MM-DD or YYYY-MM-DDTHH:mm:ss.SSSZ) from which you want to fetch the list. Maximum time period that can be selected is one month. |  |
**end_date** | Option<**String**> | Mandatory if startDate is used. Ending date (YYYY-MM-DD or YYYY-MM-DDTHH:mm:ss.SSSZ) till which you want to fetch the list. Maximum time period that can be selected is one month. |  |
**limit** | Option<**i64**> | Number of documents returned per page |  |[default to 100]
**offset** | Option<**i64**> | Index of the first document on the page |  |[default to 0]
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation |  |[default to desc]

### Return type

[**models::GetInboundEmailEvents**](getInboundEmailEvents.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_inbound_email_events_by_uuid

> models::GetInboundEmailEventsByUuid get_inbound_email_events_by_uuid(uuid)
Fetch all events history for one particular received email.

This endpoint will show the list of all events history for one particular received email.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **String** | UUID to fetch events specific to recieved email | [required] |

### Return type

[**models::GetInboundEmailEventsByUuid**](getInboundEmailEventsByUuid.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


# \TransactionalWhatsAppApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_whatsapp_event_report**](TransactionalWhatsAppApi.md#get_whatsapp_event_report) | **GET** /whatsapp/statistics/events | Get all your WhatsApp activity (unaggregated events)
[**send_whatsapp_message**](TransactionalWhatsAppApi.md#send_whatsapp_message) | **POST** /whatsapp/sendMessage | Send a WhatsApp message



## get_whatsapp_event_report

> models::GetWhatsappEventReport get_whatsapp_event_report(limit, offset, start_date, end_date, days, contact_number, event, sort)
Get all your WhatsApp activity (unaggregated events)

This endpoint will show the unaggregated statistics for WhatsApp activity (30 days by default if `startDate` and `endDate` or `days` is not passed. The date range can not exceed 90 days)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**limit** | Option<**i64**> | Number limitation for the result returned |  |[default to 2500]
**offset** | Option<**i64**> | Beginning point in the list to retrieve from |  |[default to 0]
**start_date** | Option<**String**> | **Mandatory if endDate is used.** Starting date of the report (YYYY-MM-DD). Must be lower than equal to endDate  |  |
**end_date** | Option<**String**> | **Mandatory if startDate is used.** Ending date of the report (YYYY-MM-DD). Must be greater than equal to startDate  |  |
**days** | Option<**i64**> | Number of days in the past including today (positive integer). _Not compatible with 'startDate' and 'endDate'_  |  |
**contact_number** | Option<**String**> | Filter results for specific contact (WhatsApp Number with country code. Example, 85264318721) |  |
**event** | Option<**String**> | Filter the report for a specific event type |  |
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed |  |[default to desc]

### Return type

[**models::GetWhatsappEventReport**](getWhatsappEventReport.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## send_whatsapp_message

> models::SendWhatsappMessage201Response send_whatsapp_message(send_whatsapp_message_request)
Send a WhatsApp message

This endpoint is used to send a WhatsApp message. <br/>(**The first message you send using the API must contain a Template ID. You must create a template on WhatsApp on the Brevo platform to fetch the Template ID.**)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**send_whatsapp_message_request** | [**SendWhatsappMessageRequest**](SendWhatsappMessageRequest.md) | Values to send WhatsApp message | [required] |

### Return type

[**models::SendWhatsappMessage201Response**](sendWhatsappMessage_201_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


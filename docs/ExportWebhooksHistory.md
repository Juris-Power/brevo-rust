# ExportWebhooksHistory

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**days** | Option<**i32**> | Number of days in the past including today (positive integer). _Not compatible with 'startDate' and 'endDate'_ | [optional]
**start_date** | Option<**String**> | Mandatory if endDate is used. Starting date of the history (YYYY-MM-DD). Must be lower than equal to endDate | [optional]
**end_date** | Option<**String**> | Mandatory if startDate is used. Ending date of the report (YYYY-MM-DD). Must be greater than equal to startDate | [optional]
**sort** | Option<**String**> | Sorting order of records (asc or desc) | [optional]
**r#type** | **String** | Filter the history based on webhook type | 
**event** | **String** | Filter the history for a specific event type | 
**notify_url** | **String** | Webhook URL to receive CSV file link | 
**webhook_id** | Option<**i32**> | Filter the history for a specific webhook id | [optional]
**email** | Option<**String**> | Filter the history for a specific email | [optional]
**message_id** | Option<**i32**> | Filter the history for a specific message id. Applicable only for transactional webhooks. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



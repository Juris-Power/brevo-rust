# GetInboundEmailEventsByUuid

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**received_at** | Option<**String**> | Date when email was received on SMTP relay | [optional]
**delivered_at** | Option<**String**> | Date when email was delivered successfully to client’s webhook | [optional]
**recipient** | Option<**String**> | Recipient’s email address | [optional]
**sender** | Option<**String**> | Sender’s email address | [optional]
**message_id** | Option<**String**> | Value of the Message-ID header. This will be present only after the processing is done. | [optional]
**subject** | Option<**String**> | Value of the Subject header. This will be present only after the processing is done.  | [optional]
**attachments** | Option<[**Vec<models::GetInboundEmailEventsByUuidAttachmentsInner>**](getInboundEmailEventsByUuid_attachments_inner.md)> | List of attachments of the email. This will be present only after the processing is done. | [optional]
**logs** | Option<[**Vec<models::GetInboundEmailEventsByUuidLogsInner>**](getInboundEmailEventsByUuid_logs_inner.md)> | List of events/logs that describe the lifecycle of the email on SIB platform | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



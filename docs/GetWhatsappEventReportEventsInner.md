# GetWhatsappEventReportEventsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contact_number** | **String** | WhatsApp Number with country code. Example, 85264318721 | 
**date** | **String** | UTC date-time on which the event has been generated | 
**message_id** | **String** | Message ID which generated the event | 
**event** | **String** | Event which occurred | 
**reason** | Option<**String**> | Reason for the event (will be there in case of `error` and `soft-bounce` events) | [optional]
**body** | Option<**String**> | Text of the reply (will be there only in case of `reply` event with text) | [optional]
**media_url** | Option<**String**> | Url of the media reply (will be there only in case of `reply` event with media) | [optional]
**sender_number** | **String** | WhatsApp Number with country code. Example, 85264318721 | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ConversationsMessage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> | Message ID. It can be used for further manipulations with the message. | [optional]
**r#type** | Option<**String**> | `\"agent\"` for agents’ messages, `\"visitor\"` for visitors’ messages. | [optional]
**text** | Option<**String**> | Message text or name of the attached file | [optional]
**visitor_id** | Option<**String**> | visitor’s ID | [optional]
**agent_id** | Option<**String**> | ID of the agent on whose behalf the message was sent (only in messages sent by an agent). | [optional]
**agent_name** | Option<**String**> | Agent’s name as displayed to the visitor. Only in the messages sent by an agent. | [optional]
**created_at** | Option<**i64**> | Timestamp in milliseconds. | [optional]
**is_pushed** | Option<**bool**> | `true` for pushed messages | [optional]
**received_from** | Option<**String**> | In two-way integrations, messages sent via REST API can be marked with receivedFrom property and then filtered out when received in a webhook to avoid infinite loop. | [optional]
**file** | Option<[**models::ConversationsMessageFile**](ConversationsMessage_file.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



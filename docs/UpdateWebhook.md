# UpdateWebhook

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | Option<**String**> | URL of the webhook | [optional]
**description** | Option<**String**> | Description of the webhook | [optional]
**events** | Option<**Vec<String>**> | - Events triggering the webhook. Possible values for **Transactional** type webhook: #### `sent` OR `request`, `delivered`, `hardBounce`, `softBounce`, `blocked`, `spam`, `invalid`, `deferred`, `click`, `opened`, `uniqueOpened` and `unsubscribed` - Possible values for **Marketing** type webhook: #### `spam`, `opened`, `click`, `hardBounce`, `softBounce`, `unsubscribed`, `listAddition` & `delivered` - Possible values for **Inbound** type webhook: #### `inboundEmailProcessed`  | [optional]
**domain** | Option<**String**> | Inbound domain of webhook, used in case of event type `inbound` | [optional]
**batched** | Option<**bool**> | Batching configuration of the webhook, we send batched webhooks if its true | [optional]
**auth** | Option<[**serde_json::Value**](.md)> | Authentication header to be send with the webhook requests | [optional]
**headers** | Option<[**Vec<serde_json::Value>**](serde_json::Value.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



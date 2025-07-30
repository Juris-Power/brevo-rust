# CreateWebhook

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **String** | URL of the webhook | 
**description** | Option<**String**> | Description of the webhook | [optional]
**events** | **Vec<String>** | - Events triggering the webhook. Possible values for **Transactional** type webhook: #### `sent` OR `request`, `delivered`, `hardBounce`, `softBounce`, `blocked`, `spam`, `invalid`, `deferred`, `click`, `opened`, `uniqueOpened` and `unsubscribed` - Possible values for **Marketing** type webhook: #### `spam`, `opened`, `click`, `hardBounce`, `softBounce`, `unsubscribed`, `listAddition` & `delivered` - Possible values for **Inbound** type webhook: #### `inboundEmailProcessed` - Possible values for type **Transactional** and channel **SMS** #### `accepted`,`delivered`,`softBounce`,`hardBounce`,`unsubscribe`,`reply`, `subscribe`,`sent`,`blacklisted`,`skip` - Possible values for type **Marketing**  channel **SMS** #### `sent`,`delivered`,`softBounce`,`hardBounce`,`unsubscribe`,`reply`, `subscribe`,`skip`  | 
**r#type** | Option<**String**> | Type of the webhook | [optional][default to Transactional]
**channel** | Option<**String**> | channel of webhook | [optional][default to Email]
**domain** | Option<**String**> | Inbound domain of webhook, required in case of event type `inbound` | [optional]
**batched** | Option<**bool**> | Batching configuration of the webhook, we send batched webhooks if its true | [optional]
**auth** | Option<[**models::CreateWebhookAuth**](createWebhook_auth.md)> |  | [optional]
**headers** | Option<[**Vec<models::CreateWebhookHeadersInner>**](createWebhook_headers_inner.md)> | The headers sent with the request to the webhook. Header format: \"headers\": [{ \"key\": \"cf-secret\",\"value\": \"test-header-value\"}]  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



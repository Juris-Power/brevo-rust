# GetWebhook

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **String** | URL of the webhook | 
**id** | **i64** | ID of the webhook | 
**description** | **String** | Description of the webhook | 
**events** | **Vec<String>** |  | 
**r#type** | **String** | Type of webhook (marketing or transactional) | 
**channel** | Option<**String**> | channel of webhook | [optional][default to Email]
**created_at** | **String** | Creation UTC date-time of the webhook (YYYY-MM-DDTHH:mm:ss.SSSZ) | 
**modified_at** | **String** | Last modification UTC date-time of the webhook (YYYY-MM-DDTHH:mm:ss.SSSZ) | 
**batched** | Option<**bool**> | Batching configuration of the webhook, we send batched webhooks if its true | [optional]
**auth** | Option<[**serde_json::Value**](.md)> | Authentication header to be send with the webhook requests | [optional]
**headers** | Option<[**Vec<serde_json::Value>**](serde_json::Value.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



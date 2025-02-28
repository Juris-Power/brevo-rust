# \WebhooksApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_webhook**](WebhooksApi.md#create_webhook) | **POST** /webhooks | Create a webhook
[**delete_webhook**](WebhooksApi.md#delete_webhook) | **DELETE** /webhooks/{webhookId} | Delete a webhook
[**export_webhooks_history**](WebhooksApi.md#export_webhooks_history) | **POST** /webhooks/export | Export all webhook events
[**get_webhook**](WebhooksApi.md#get_webhook) | **GET** /webhooks/{webhookId} | Get a webhook details
[**get_webhooks**](WebhooksApi.md#get_webhooks) | **GET** /webhooks | Get all webhooks
[**update_webhook**](WebhooksApi.md#update_webhook) | **PUT** /webhooks/{webhookId} | Update a webhook



## create_webhook

> models::CreateModel create_webhook(create_webhook)
Create a webhook

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_webhook** | [**CreateWebhook**](CreateWebhook.md) | Values to create a webhook | [required] |

### Return type

[**models::CreateModel**](createModel.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_webhook

> delete_webhook(webhook_id)
Delete a webhook

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**webhook_id** | **i64** | Id of the webhook | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## export_webhooks_history

> models::CreatedProcessId export_webhooks_history(export_webhooks_history_request)
Export all webhook events

This endpoint will submit a request to get the history of webhooks in the CSV file. The link to download the CSV file will be sent to the webhook that was provided in the notifyURL.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**export_webhooks_history_request** | [**ExportWebhooksHistoryRequest**](ExportWebhooksHistoryRequest.md) | Values to submit for webhooks history | [required] |

### Return type

[**models::CreatedProcessId**](createdProcessId.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_webhook

> models::GetWebhook get_webhook(webhook_id)
Get a webhook details

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**webhook_id** | **i64** | Id of the webhook | [required] |

### Return type

[**models::GetWebhook**](getWebhook.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_webhooks

> models::GetWebhooks get_webhooks(r#type, sort)
Get all webhooks

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**r#type** | Option<**String**> | Filter on webhook type |  |[default to transactional]
**sort** | Option<**String**> | Sort the results in the ascending/descending order of webhook creation |  |[default to desc]

### Return type

[**models::GetWebhooks**](getWebhooks.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_webhook

> update_webhook(webhook_id, update_webhook)
Update a webhook

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**webhook_id** | **i64** | Id of the webhook | [required] |
**update_webhook** | [**UpdateWebhook**](UpdateWebhook.md) | Values to update a webhook | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


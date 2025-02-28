# \ConversationsApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**conversations_agent_online_ping_post**](ConversationsApi.md#conversations_agent_online_ping_post) | **POST** /conversations/agentOnlinePing | Sets agent’s status to online for 2-3 minutes
[**conversations_messages_id_delete**](ConversationsApi.md#conversations_messages_id_delete) | **DELETE** /conversations/messages/{id} | Delete a message sent by an agent
[**conversations_messages_id_get**](ConversationsApi.md#conversations_messages_id_get) | **GET** /conversations/messages/{id} | Get a message
[**conversations_messages_id_put**](ConversationsApi.md#conversations_messages_id_put) | **PUT** /conversations/messages/{id} | Update a message sent by an agent
[**conversations_messages_post**](ConversationsApi.md#conversations_messages_post) | **POST** /conversations/messages | Send a message as an agent
[**conversations_pushed_messages_id_delete**](ConversationsApi.md#conversations_pushed_messages_id_delete) | **DELETE** /conversations/pushedMessages/{id} | Delete an automated message
[**conversations_pushed_messages_id_get**](ConversationsApi.md#conversations_pushed_messages_id_get) | **GET** /conversations/pushedMessages/{id} | Get an automated message
[**conversations_pushed_messages_id_put**](ConversationsApi.md#conversations_pushed_messages_id_put) | **PUT** /conversations/pushedMessages/{id} | Update an automated message
[**conversations_pushed_messages_post**](ConversationsApi.md#conversations_pushed_messages_post) | **POST** /conversations/pushedMessages | Send an automated message to a visitor



## conversations_agent_online_ping_post

> conversations_agent_online_ping_post(conversations_agent_online_ping_post_request)
Sets agent’s status to online for 2-3 minutes

We recommend pinging this endpoint every minute for as long as the agent has to be considered online.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**conversations_agent_online_ping_post_request** | [**ConversationsAgentOnlinePingPostRequest**](ConversationsAgentOnlinePingPostRequest.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## conversations_messages_id_delete

> conversations_messages_id_delete(id)
Delete a message sent by an agent

Only agents’ messages can be deleted.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | ID of the message | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## conversations_messages_id_get

> models::ConversationsMessage conversations_messages_id_get(id)
Get a message

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | ID of the message | [required] |

### Return type

[**models::ConversationsMessage**](ConversationsMessage.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## conversations_messages_id_put

> models::ConversationsMessage conversations_messages_id_put(id, conversations_messages_id_put_request)
Update a message sent by an agent

Only agents’ messages can be edited.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | ID of the message | [required] |
**conversations_messages_id_put_request** | [**ConversationsMessagesIdPutRequest**](ConversationsMessagesIdPutRequest.md) |  | [required] |

### Return type

[**models::ConversationsMessage**](ConversationsMessage.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## conversations_messages_post

> models::ConversationsMessage conversations_messages_post(conversations_messages_post_request)
Send a message as an agent

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**conversations_messages_post_request** | [**ConversationsMessagesPostRequest**](ConversationsMessagesPostRequest.md) |  | [required] |

### Return type

[**models::ConversationsMessage**](ConversationsMessage.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## conversations_pushed_messages_id_delete

> conversations_pushed_messages_id_delete(id)
Delete an automated message

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | ID of the message | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## conversations_pushed_messages_id_get

> models::ConversationsMessage conversations_pushed_messages_id_get(id)
Get an automated message

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | ID of the message sent previously | [required] |

### Return type

[**models::ConversationsMessage**](ConversationsMessage.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## conversations_pushed_messages_id_put

> models::ConversationsMessage conversations_pushed_messages_id_put(id, conversations_messages_id_put_request)
Update an automated message

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | ID of the message | [required] |
**conversations_messages_id_put_request** | [**ConversationsMessagesIdPutRequest**](ConversationsMessagesIdPutRequest.md) |  | [required] |

### Return type

[**models::ConversationsMessage**](ConversationsMessage.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## conversations_pushed_messages_post

> models::ConversationsMessage conversations_pushed_messages_post(conversations_pushed_messages_post_request)
Send an automated message to a visitor

Example of automated messages: order status, announce new features in your web app, etc.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**conversations_pushed_messages_post_request** | [**ConversationsPushedMessagesPostRequest**](ConversationsPushedMessagesPostRequest.md) |  | [required] |

### Return type

[**models::ConversationsMessage**](ConversationsMessage.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


# \BalanceApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**begin_transaction**](BalanceApi.md#begin_transaction) | **POST** /loyalty/balance/programs/{pid}/transactions | Create new transaction
[**cancel_transaction**](BalanceApi.md#cancel_transaction) | **POST** /loyalty/balance/programs/{pid}/transactions/{tid}/cancel | Cancel transaction
[**complete_transaction**](BalanceApi.md#complete_transaction) | **POST** /loyalty/balance/programs/{pid}/transactions/{tid}/complete | Complete transaction
[**create_balance_limit**](BalanceApi.md#create_balance_limit) | **POST** /loyalty/balance/programs/{pid}/balance-definitions/{bdid}/limits | Create balance limits
[**create_balance_order**](BalanceApi.md#create_balance_order) | **POST** /loyalty/balance/programs/{pid}/create-order | Create balance order
[**delete_balance_definition**](BalanceApi.md#delete_balance_definition) | **DELETE** /loyalty/balance/programs/{pid}/balance-definitions/{bdid} | Delete balance definition
[**delete_balance_limit**](BalanceApi.md#delete_balance_limit) | **DELETE** /loyalty/balance/programs/{pid}/balance-definitions/{bdid}/limits/{blid} | Delete balance limit
[**get_balance_definition**](BalanceApi.md#get_balance_definition) | **GET** /loyalty/balance/programs/{pid}/balance-definitions/{bdid} | Get balance definition
[**get_balance_definition_list**](BalanceApi.md#get_balance_definition_list) | **GET** /loyalty/balance/programs/{pid}/balance-definitions | Get balance definition list
[**get_balance_limit**](BalanceApi.md#get_balance_limit) | **GET** /loyalty/balance/programs/{pid}/balance-definitions/{bdid}/limits/{blid} | Get balance limits
[**get_contact_balances**](BalanceApi.md#get_contact_balances) | **GET** /loyalty/balance/programs/{pid}/contact-balances | Get balance list
[**get_subscription_balances**](BalanceApi.md#get_subscription_balances) | **GET** /loyalty/balance/programs/{pid}/subscriptions/{cid}/balances | Get subscription balances
[**loyalty_balance_programs_pid_active_balance_get**](BalanceApi.md#loyalty_balance_programs_pid_active_balance_get) | **GET** /loyalty/balance/programs/{pid}/active-balance | Get Active Balances API
[**loyalty_balance_programs_pid_balance_definitions_post**](BalanceApi.md#loyalty_balance_programs_pid_balance_definitions_post) | **POST** /loyalty/balance/programs/{pid}/balance-definitions | Create balance definition
[**loyalty_balance_programs_pid_subscriptions_cid_balances_post**](BalanceApi.md#loyalty_balance_programs_pid_subscriptions_cid_balances_post) | **POST** /loyalty/balance/programs/{pid}/subscriptions/{cid}/balances | Create subscription balances
[**loyalty_balance_programs_pid_transaction_history_get**](BalanceApi.md#loyalty_balance_programs_pid_transaction_history_get) | **GET** /loyalty/balance/programs/{pid}/transaction-history | Get Transaction History API
[**update_balance_definition**](BalanceApi.md#update_balance_definition) | **PUT** /loyalty/balance/programs/{pid}/balance-definitions/{bdid} | Update balance definition
[**update_balance_limit**](BalanceApi.md#update_balance_limit) | **PUT** /loyalty/balance/programs/{pid}/balance-definitions/{bdid}/limits/{blid} | Updates balance limit



## begin_transaction

> models::Transaction begin_transaction(pid, create_transaction_payload)
Create new transaction

Creates new transaction and returns information

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |
**create_transaction_payload** | [**CreateTransactionPayload**](CreateTransactionPayload.md) | Transaction Payload | [required] |

### Return type

[**models::Transaction**](transaction.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## cancel_transaction

> models::Transaction cancel_transaction(pid, tid)
Cancel transaction

Cancels transaction

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |
**tid** | **uuid::Uuid** | Transaction Id | [required] |

### Return type

[**models::Transaction**](transaction.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## complete_transaction

> models::Transaction complete_transaction(pid, tid)
Complete transaction

Completes transaction

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |
**tid** | **uuid::Uuid** | Transaction Id | [required] |

### Return type

[**models::Transaction**](transaction.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_balance_limit

> models::BalanceLimit create_balance_limit(pid, bdid, create_balance_limit_payload)
Create balance limits

Creates balance limit and sends the created UUID along with the data

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |
**bdid** | **uuid::Uuid** | Balance Definition Id | [required] |
**create_balance_limit_payload** | [**CreateBalanceLimitPayload**](CreateBalanceLimitPayload.md) | Balance Definition Payload | [required] |

### Return type

[**models::BalanceLimit**](balanceLimit.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_balance_order

> models::BalanceOrder create_balance_order(pid, create_order_payload)
Create balance order

Returns created order

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |
**create_order_payload** | [**CreateOrderPayload**](CreateOrderPayload.md) | Order Payload | [required] |

### Return type

[**models::BalanceOrder**](balanceOrder.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_balance_definition

> delete_balance_definition(pid, bdid)
Delete balance definition

Delete Balance definition

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |
**bdid** | **uuid::Uuid** | Balance Definition Id | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_balance_limit

> delete_balance_limit(pid, bdid, blid)
Delete balance limit

Delete balance limit

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |
**bdid** | **uuid::Uuid** | Balance Definition Id | [required] |
**blid** | **uuid::Uuid** | Balance Limit Id | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_balance_definition

> models::BalanceDefinition get_balance_definition(pid, bdid, version)
Get balance definition

Returns balance definition

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |
**bdid** | **uuid::Uuid** | Balance Definition Id | [required] |
**version** | Option<**String**> | Version |  |[default to draft]

### Return type

[**models::BalanceDefinition**](balanceDefinition.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_balance_definition_list

> models::BalanceDefinitionPage get_balance_definition_list(pid, limit, offset, sort_field, sort, version)
Get balance definition list

Returns balance definition page

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |
**limit** | Option<**i32**> | Limit the number of records returned |  |[default to 200]
**offset** | Option<**i32**> | Offset to paginate records |  |[default to 0]
**sort_field** | Option<**String**> | Field to sort by |  |[default to updated_at]
**sort** | Option<**String**> | Sort direction |  |[default to desc]
**version** | Option<**String**> | Version |  |[default to draft]

### Return type

[**models::BalanceDefinitionPage**](balanceDefinitionPage.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_balance_limit

> models::BalanceLimit get_balance_limit(pid, bdid, blid, version)
Get balance limits

Fetches balance limits and send the created UUID along with the data

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |
**bdid** | **uuid::Uuid** | Balance Definition Id | [required] |
**blid** | **uuid::Uuid** | Balance Limit Id | [required] |
**version** | Option<**String**> | Version |  |[default to draft]

### Return type

[**models::BalanceLimit**](balanceLimit.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_balances

> models::ContactBalancesResp get_contact_balances(pid)
Get balance list

Returns balance list

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |

### Return type

[**models::ContactBalancesResp**](contactBalancesResp.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_subscription_balances

> models::ModelSubscriptionBalanceResp get_subscription_balances(cid, pid)
Get subscription balances

Returns subscription balances

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**cid** | **String** | Contact Id | [required] |
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |

### Return type

[**models::ModelSubscriptionBalanceResp**](modelSubscriptionBalanceResp.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## loyalty_balance_programs_pid_active_balance_get

> models::BalanceLimit loyalty_balance_programs_pid_active_balance_get(pid, contact_id, balance_definition_id, limit, offset, sort_field, sort)
Get Active Balances API

Returns Active Balances

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |
**contact_id** | **i32** | Contact ID | [required] |
**balance_definition_id** | **uuid::Uuid** | Balance Definition ID | [required] |
**limit** | Option<**i32**> | Limit |  |
**offset** | Option<**i32**> | Offset |  |
**sort_field** | Option<**String**> | Sort Field |  |
**sort** | Option<**String**> | Sort Order |  |

### Return type

[**models::BalanceLimit**](balanceLimit.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## loyalty_balance_programs_pid_balance_definitions_post

> models::BalanceDefinition loyalty_balance_programs_pid_balance_definitions_post(pid, create_balance_definition_payload)
Create balance definition

Creates balance definition and returns information

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |
**create_balance_definition_payload** | [**CreateBalanceDefinitionPayload**](CreateBalanceDefinitionPayload.md) | Create Balance Definition Payload | [required] |

### Return type

[**models::BalanceDefinition**](balanceDefinition.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## loyalty_balance_programs_pid_subscriptions_cid_balances_post

> models::Balance loyalty_balance_programs_pid_subscriptions_cid_balances_post(pid, cid, create_balance_payload)
Create subscription balances

Creates a balance for a contact

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |
**cid** | **uuid::Uuid** | Contact Id | [required] |
**create_balance_payload** | [**CreateBalancePayload**](CreateBalancePayload.md) | Create Balnce Payload | [required] |

### Return type

[**models::Balance**](balance.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## loyalty_balance_programs_pid_transaction_history_get

> models::TransactionHistoryResp loyalty_balance_programs_pid_transaction_history_get(pid, contact_id, balance_definition_id, limit, offset, sort_field, sort, filters)
Get Transaction History API

Returns transaction history

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |
**contact_id** | **i32** | Contact ID | [required] |[default to 0]
**balance_definition_id** | **uuid::Uuid** | Balance Definition ID | [required] |
**limit** | Option<**i32**> | Limit the number of records returned |  |[default to 20]
**offset** | Option<**i32**> | Skip a number of records |  |[default to 0]
**sort_field** | Option<**String**> | Field to sort by |  |[default to created_at]
**sort** | Option<**String**> | Sort order, either asc or desc |  |[default to desc]
**filters** | Option<[**Vec<String>**](String.md)> | Filters to apply |  |

### Return type

[**models::TransactionHistoryResp**](transactionHistoryResp.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_balance_definition

> models::BalanceDefinition update_balance_definition(pid, bdid, update_balance_definition_payload)
Update balance definition

Updates Balance definition

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |
**bdid** | **uuid::Uuid** | Balance Definition Id | [required] |
**update_balance_definition_payload** | [**UpdateBalanceDefinitionPayload**](UpdateBalanceDefinitionPayload.md) | Create Balance Definition Payload | [required] |

### Return type

[**models::BalanceDefinition**](balanceDefinition.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_balance_limit

> models::BalanceLimit update_balance_limit(pid, bdid, blid, update_balance_limit_payload)
Updates balance limit

Updates balance limit

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program Id | [required] |
**bdid** | **uuid::Uuid** | Balance Definition Id | [required] |
**blid** | **uuid::Uuid** | Balance Limit Id | [required] |
**update_balance_limit_payload** | [**UpdateBalanceLimitPayload**](UpdateBalanceLimitPayload.md) | Balance Limits Payload | [required] |

### Return type

[**models::BalanceLimit**](balanceLimit.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


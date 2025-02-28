# \ProgramApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_new_lp**](ProgramApi.md#create_new_lp) | **POST** /loyalty/config/programs | Create loyalty program
[**delete_contact_members**](ProgramApi.md#delete_contact_members) | **DELETE** /loyalty/config/programs/{pid}/subscription-members | Delete subscription member
[**delete_loyalty_program**](ProgramApi.md#delete_loyalty_program) | **DELETE** /loyalty/config/programs/{pid} | Delete Loyalty Program
[**get_loyalty_program_info**](ProgramApi.md#get_loyalty_program_info) | **GET** /loyalty/config/programs/{pid} | Get loyalty program Info
[**get_lp_list**](ProgramApi.md#get_lp_list) | **GET** /loyalty/config/programs | Get loyalty program list
[**get_parameter_subscription_info**](ProgramApi.md#get_parameter_subscription_info) | **GET** /loyalty/config/programs/{pid}/account-info | Get Subscription Data
[**partially_update_loyalty_program**](ProgramApi.md#partially_update_loyalty_program) | **PATCH** /loyalty/config/programs/{pid} | Partially update loyalty program
[**publish_loyalty_program**](ProgramApi.md#publish_loyalty_program) | **POST** /loyalty/config/programs/{pid}/publish | Publish loyalty program
[**subscribe_member_to_a_subscription**](ProgramApi.md#subscribe_member_to_a_subscription) | **POST** /loyalty/config/programs/{pid}/subscription-members | Create subscription member
[**subscribe_to_loyalty_program**](ProgramApi.md#subscribe_to_loyalty_program) | **POST** /loyalty/config/programs/{pid}/subscriptions | Create subscription
[**update_loyalty_program**](ProgramApi.md#update_loyalty_program) | **PUT** /loyalty/config/programs/{pid} | Update loyalty program



## create_new_lp

> models::LoyaltyProgram create_new_lp(create_loyalty_program_payload)
Create loyalty program

Creates loyalty program

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_loyalty_program_payload** | [**CreateLoyaltyProgramPayload**](CreateLoyaltyProgramPayload.md) | Payload for creating a new loyalty program. | [required] |

### Return type

[**models::LoyaltyProgram**](loyaltyProgram.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_contact_members

> delete_contact_members(pid, member_contact_ids)
Delete subscription member

Deletes member from a subscription

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID. A unique identifier for the loyalty program. | [required] |
**member_contact_ids** | **String** | Comma-separated list of member contact IDs to delete from the subscription. | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_loyalty_program

> delete_loyalty_program(pid)
Delete Loyalty Program

Deletes Loyalty Program

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID. A unique identifier for the loyalty program. | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_loyalty_program_info

> models::LoyaltyProgram get_loyalty_program_info(pid)
Get loyalty program Info

Returns loyalty program

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID. A unique identifier for the loyalty program. | [required] |

### Return type

[**models::LoyaltyProgram**](loyaltyProgram.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_lp_list

> models::LoyaltyProgramPage get_lp_list(limit, offset, sort_field, sort)
Get loyalty program list

Returns list of loyalty programs

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**limit** | Option<**i32**> | Number of documents per page |  |
**offset** | Option<**i32**> | Index of the first document in the page |  |
**sort_field** | Option<**String**> | Sort documents by field |  |
**sort** | Option<**String**> | Sort documents by field |  |

### Return type

[**models::LoyaltyProgramPage**](loyaltyProgramPage.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_parameter_subscription_info

> models::SubscriptionHandlerInfo get_parameter_subscription_info(pid, contact_id, params, loyalty_subscription_id)
Get Subscription Data

Get Information of balances, tiers, rewards and subscription members for a subscription

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID. A unique identifier for the loyalty program. | [required] |
**contact_id** | Option<**String**> | The contact ID to filter by. |  |
**params** | Option<**String**> | A list of filter parameters for querying the subscription info. |  |
**loyalty_subscription_id** | Option<**String**> | The loyalty subscription ID to filter by. |  |

### Return type

[**models::SubscriptionHandlerInfo**](subscriptionHandlerInfo.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## partially_update_loyalty_program

> models::LoyaltyProgram partially_update_loyalty_program(pid, patch_loyalty_program_payload)
Partially update loyalty program

Partially updates loyalty program

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID. A unique identifier for the loyalty program. | [required] |
**patch_loyalty_program_payload** | [**PatchLoyaltyProgramPayload**](PatchLoyaltyProgramPayload.md) | Loyalty Program Payload | [required] |

### Return type

[**models::LoyaltyProgram**](loyaltyProgram.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## publish_loyalty_program

> publish_loyalty_program(pid)
Publish loyalty program

Publishes loyalty program

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID. A unique identifier for the loyalty program. | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## subscribe_member_to_a_subscription

> models::SubscriptionMember subscribe_member_to_a_subscription(pid, add_subscription_member_payload)
Create subscription member

Add member to a subscription

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID. A unique identifier for the loyalty program. | [required] |
**add_subscription_member_payload** | [**AddSubscriptionMemberPayload**](AddSubscriptionMemberPayload.md) | Payload for adding a subscription member. | [required] |

### Return type

[**models::SubscriptionMember**](subscriptionMember.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## subscribe_to_loyalty_program

> models::Subscription subscribe_to_loyalty_program(pid, create_subscription_payload)
Create subscription

Subscribes to a loyalty program

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID. A unique identifier for the loyalty program. | [required] |
**create_subscription_payload** | [**CreateSubscriptionPayload**](CreateSubscriptionPayload.md) | Create Subscription Payload | [required] |

### Return type

[**models::Subscription**](subscription.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_loyalty_program

> models::LoyaltyProgram update_loyalty_program(pid, update_loyalty_program_payload)
Update loyalty program

Updates loyalty program

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID. A unique identifier for the loyalty program. | [required] |
**update_loyalty_program_payload** | [**UpdateLoyaltyProgramPayload**](UpdateLoyaltyProgramPayload.md) | Update Loyalty Program Payload | [required] |

### Return type

[**models::LoyaltyProgram**](loyaltyProgram.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


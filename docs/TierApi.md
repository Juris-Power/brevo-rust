# \TierApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_subscription_to_tier**](TierApi.md#add_subscription_to_tier) | **POST** /loyalty/tier/programs/{pid}/contacts/{cid}/tiers/{tid} | Assign a tier
[**create_tier_for_tier_group**](TierApi.md#create_tier_for_tier_group) | **POST** /loyalty/tier/programs/{pid}/tier-groups/{gid}/tiers | Create a tier
[**create_tier_group**](TierApi.md#create_tier_group) | **POST** /loyalty/tier/programs/{pid}/tier-groups | Create a tier group
[**delete_tier**](TierApi.md#delete_tier) | **DELETE** /loyalty/tier/programs/{pid}/tiers/{tid} | Delete tier
[**delete_tier_group**](TierApi.md#delete_tier_group) | **DELETE** /loyalty/tier/programs/{pid}/tier-groups/{gid} | Delete tier group
[**get_list_of_tier_groups**](TierApi.md#get_list_of_tier_groups) | **GET** /loyalty/tier/programs/{pid}/tier-groups | List tier groups
[**get_loyalty_program_tier**](TierApi.md#get_loyalty_program_tier) | **GET** /loyalty/tier/programs/{pid}/tiers | List tiers
[**get_tier_group**](TierApi.md#get_tier_group) | **GET** /loyalty/tier/programs/{pid}/tier-groups/{gid} | Get tier group
[**update_tier**](TierApi.md#update_tier) | **PUT** /loyalty/tier/programs/{pid}/tiers/{tid} | Update tier
[**update_tier_group**](TierApi.md#update_tier_group) | **PUT** /loyalty/tier/programs/{pid}/tier-groups/{gid} | Update tier group



## add_subscription_to_tier

> models::TierForContact add_subscription_to_tier(pid, cid, tid)
Assign a tier

Manually assigns a tier to a specific membership.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**cid** | **uuid::Uuid** | Contact ID | [required] |
**tid** | **uuid::Uuid** | Tier ID | [required] |

### Return type

[**models::TierForContact**](tierForContact.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_tier_for_tier_group

> models::Tier create_tier_for_tier_group(pid, gid, tier_request)
Create a tier

Creates a new tier in a loyalty program tier group. *(The changes will take effect with the next publication of the loyalty program)*

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**gid** | **uuid::Uuid** | Tier group ID | [required] |
**tier_request** | [**TierRequest**](TierRequest.md) |  | [required] |

### Return type

[**models::Tier**](tier.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_tier_group

> models::TierGroup create_tier_group(pid, create_tier_group_request)
Create a tier group

Creates a new tier group in a loyalty program. *(The changes will take effect with the next publication of the loyalty program)*

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**create_tier_group_request** | [**CreateTierGroupRequest**](CreateTierGroupRequest.md) | Tier group creation payload | [required] |

### Return type

[**models::TierGroup**](tierGroup.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tier

> String delete_tier(pid, tid)
Delete tier

Deletes a tier from a loyalty program tier group. *(The changes will take effect with the next publication of the loyalty program)*

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**tid** | **uuid::Uuid** | Tier ID | [required] |

### Return type

**String**

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_tier_group

> String delete_tier_group(pid, gid)
Delete tier group

Deletes a tier group from a loyalty program. *(The changes will take effect with the next publication of the loyalty program)*

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**gid** | **uuid::Uuid** | Tier group ID | [required] |

### Return type

**String**

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: aplication/json, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_list_of_tier_groups

> models::TierGroupPage get_list_of_tier_groups(pid, version)
List tier groups

Returns the list of tier groups defined within the loyalty program.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**version** | Option<**String**> | Select 'active' to retrieve list of all tier groups which are live for clients. Select draft to retrieve list of all non deleted tier groups. |  |[default to draft]

### Return type

[**models::TierGroupPage**](tierGroupPage.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_loyalty_program_tier

> models::LoyaltyTierPage get_loyalty_program_tier(pid, version)
List tiers

Returns the list of tiers defined within the loyalty program.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**version** | Option<**String**> | Select 'active' to retrieve list of all tiers which are live for clients. Select draft to retrieve list of all non deleted tiers. |  |[default to draft]

### Return type

[**models::LoyaltyTierPage**](loyaltyTierPage.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_tier_group

> models::TierGroup get_tier_group(pid, gid, version)
Get tier group

Returns tier group information.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**gid** | **uuid::Uuid** | Tier group ID | [required] |
**version** | Option<**String**> | Select active to retrieve active version of tier group. Select draft to retrieve latest changes in tier group. |  |[default to draft]

### Return type

[**models::TierGroup**](tierGroup.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_tier

> models::Tier update_tier(pid, tid, tier_request_put_payload)
Update tier

Modifies an existing tier for the specified tier group *(The changes will take effect with the next publication of the loyalty program)*

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**tid** | **uuid::Uuid** | Tier ID | [required] |
**tier_request_put_payload** | [**TierRequestPutPayload**](TierRequestPutPayload.md) |  | [required] |

### Return type

[**models::Tier**](tier.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_tier_group

> models::TierGroup update_tier_group(pid, gid, update_tier_group_request)
Update tier group

Updates a tier group from a loyalty program. *(The changes will take effect with the next publication of the loyalty program)*

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**gid** | **uuid::Uuid** | Tier group ID | [required] |
**update_tier_group_request** | [**UpdateTierGroupRequest**](UpdateTierGroupRequest.md) | Tier group update payload | [required] |

### Return type

[**models::TierGroup**](tierGroup.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


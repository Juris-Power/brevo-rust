# \RewardApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**complete_redeem_transaction**](RewardApi.md#complete_redeem_transaction) | **POST** /loyalty/offer/programs/{pid}/rewards/redeem/{tid}/complete | Complete redeem voucher request
[**create_reward**](RewardApi.md#create_reward) | **POST** /loyalty/offer/programs/{pid}/offers | Create a reward
[**create_voucher**](RewardApi.md#create_voucher) | **POST** /loyalty/offer/programs/{pid}/rewards/attribute | Create a voucher
[**get_code_count**](RewardApi.md#get_code_count) | **GET** /loyalty/offer/programs/{pid}/code-pools/{cpid}/codes-count | Get code count
[**loyalty_offer_programs_pid_offers_get**](RewardApi.md#loyalty_offer_programs_pid_offers_get) | **GET** /loyalty/offer/programs/{pid}/offers | Get Reward Page API
[**loyalty_offer_programs_pid_rewards_rid_get**](RewardApi.md#loyalty_offer_programs_pid_rewards_rid_get) | **GET** /loyalty/offer/programs/{pid}/rewards/{rid} | Get reward information
[**loyalty_offer_programs_pid_vouchers_get**](RewardApi.md#loyalty_offer_programs_pid_vouchers_get) | **GET** /loyalty/offer/programs/{pid}/vouchers | Get voucher for a contact
[**redeem_voucher**](RewardApi.md#redeem_voucher) | **POST** /loyalty/offer/programs/{pid}/rewards/redeem | Create redeem voucher request
[**revoke_vouchers**](RewardApi.md#revoke_vouchers) | **DELETE** /loyalty/offer/programs/{pid}/rewards/revoke | Revoke vouchers
[**validate_reward**](RewardApi.md#validate_reward) | **POST** /loyalty/offer/programs/{pid}/rewards/validate | Validate a reward



## complete_redeem_transaction

> models::MainPeriodRedeem complete_redeem_transaction(pid, tid)
Complete redeem voucher request

Completes voucher redeem request.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**tid** | **String** | Redeem transaction ID | [required] |

### Return type

[**models::MainPeriodRedeem**](main.redeem.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_reward

> models::MainPeriodCreateRewardResponse create_reward(pid, main_period_create_reward_payload)
Create a reward

Creates a new reward in the loyalty program.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**main_period_create_reward_payload** | [**MainPeriodCreateRewardPayload**](MainPeriodCreateRewardPayload.md) |  | [required] |

### Return type

[**models::MainPeriodCreateRewardResponse**](main.createRewardResponse.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_voucher

> models::MainPeriodRewardAttribution create_voucher(pid, main_period_attribute_reward_payload)
Create a voucher

Create a voucher and attribute it to a specific membership.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**main_period_attribute_reward_payload** | [**MainPeriodAttributeRewardPayload**](MainPeriodAttributeRewardPayload.md) |  | [required] |

### Return type

[**models::MainPeriodRewardAttribution**](main.rewardAttribution.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_code_count

> models::MainPeriodCodeCountHttpResponse get_code_count(pid, cpid)
Get code count

Get code count

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**cpid** | **uuid::Uuid** | Code Pool ID | [required] |

### Return type

[**models::MainPeriodCodeCountHttpResponse**](main.codeCountHttpResponse.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## loyalty_offer_programs_pid_offers_get

> models::MainPeriodRewardPage loyalty_offer_programs_pid_offers_get(pid, limit, offset, state, version)
Get Reward Page API

Returns a reward page

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**limit** | Option<**i32**> | Page size |  |[default to 25]
**offset** | Option<**i32**> | Pagination offset |  |[default to 0]
**state** | Option<**String**> | State of the reward |  |[default to all]
**version** | Option<**String**> | Version |  |[default to draft]

### Return type

[**models::MainPeriodRewardPage**](main.rewardPage.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## loyalty_offer_programs_pid_rewards_rid_get

> models::MainPeriodReward loyalty_offer_programs_pid_rewards_rid_get(pid, rid, version)
Get reward information

Returns reward information.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**rid** | **uuid::Uuid** | Reward ID | [required] |
**version** | Option<**String**> | Version |  |[default to draft]

### Return type

[**models::MainPeriodReward**](main.reward.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## loyalty_offer_programs_pid_vouchers_get

> models::MainPeriodModelContactRewardsResp loyalty_offer_programs_pid_vouchers_get(pid, contact_id, limit, offset, sort, sort_field, metadata_key_value, reward_id)
Get voucher for a contact

Get voucher for a contact

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**contact_id** | **i32** | Contact ID | [required] |
**limit** | Option<**i32**> | Page size |  |[default to 25]
**offset** | Option<**i32**> | Pagination offset |  |[default to 0]
**sort** | Option<**String**> | Sort order |  |[default to desc]
**sort_field** | Option<**String**> | Sort field |  |[default to updatedAt]
**metadata_key_value** | Option<**String**> | Metadata value for a Key filter |  |
**reward_id** | Option<**String**> | Reward ID |  |

### Return type

[**models::MainPeriodModelContactRewardsResp**](main.modelContactRewardsResp.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## redeem_voucher

> models::MainPeriodRedeem redeem_voucher(pid, main_period_create_redeem_payload)
Create redeem voucher request

Creates a request to redeem a voucher.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**main_period_create_redeem_payload** | [**MainPeriodCreateRedeemPayload**](MainPeriodCreateRedeemPayload.md) |  | [required] |

### Return type

[**models::MainPeriodRedeem**](main.redeem.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## revoke_vouchers

> revoke_vouchers(pid, attributed_reward_ids)
Revoke vouchers

Revoke attributed vouchers.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**attributed_reward_ids** | Option<**String**> | Reward Attribution IDs (comma seperated) |  |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## validate_reward

> models::MainPeriodRewardValidate validate_reward(pid, main_period_validate_reward_payload)
Validate a reward

Validates a reward.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pid** | **uuid::Uuid** | Loyalty Program ID | [required] |
**main_period_validate_reward_payload** | [**MainPeriodValidateRewardPayload**](MainPeriodValidateRewardPayload.md) |  | [required] |

### Return type

[**models::MainPeriodRewardValidate**](main.rewardValidate.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


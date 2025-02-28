# \MasterAccountApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**corporate_group_id_delete**](MasterAccountApi.md#corporate_group_id_delete) | **DELETE** /corporate/group/{id} | Delete a group
[**corporate_group_id_get**](MasterAccountApi.md#corporate_group_id_get) | **GET** /corporate/group/{id} | GET a group details
[**corporate_group_id_put**](MasterAccountApi.md#corporate_group_id_put) | **PUT** /corporate/group/{id} | Update a group of sub-accounts
[**corporate_group_post**](MasterAccountApi.md#corporate_group_post) | **POST** /corporate/group | Create a group of sub-accounts
[**corporate_group_unlink_group_id_sub_accounts_put**](MasterAccountApi.md#corporate_group_unlink_group_id_sub_accounts_put) | **PUT** /corporate/group/unlink/{groupId}/subAccounts | Delete sub-account from group
[**corporate_ip_get**](MasterAccountApi.md#corporate_ip_get) | **GET** /corporate/ip | List of all IPs
[**corporate_master_account_get**](MasterAccountApi.md#corporate_master_account_get) | **GET** /corporate/masterAccount | Get the details of requested master account
[**corporate_sso_token_post**](MasterAccountApi.md#corporate_sso_token_post) | **POST** /corporate/ssoToken | Generate SSO token to access admin account
[**corporate_sub_account_get**](MasterAccountApi.md#corporate_sub_account_get) | **GET** /corporate/subAccount | Get the list of all the sub-accounts of the master account.
[**corporate_sub_account_id_applications_toggle_put**](MasterAccountApi.md#corporate_sub_account_id_applications_toggle_put) | **PUT** /corporate/subAccount/{id}/applications/toggle | Enable/disable sub-account application(s)
[**corporate_sub_account_id_delete**](MasterAccountApi.md#corporate_sub_account_id_delete) | **DELETE** /corporate/subAccount/{id} | Delete a sub-account
[**corporate_sub_account_id_get**](MasterAccountApi.md#corporate_sub_account_id_get) | **GET** /corporate/subAccount/{id} | Get sub-account details
[**corporate_sub_account_id_plan_put**](MasterAccountApi.md#corporate_sub_account_id_plan_put) | **PUT** /corporate/subAccount/{id}/plan | Update sub-account plan
[**corporate_sub_account_ip_associate_post**](MasterAccountApi.md#corporate_sub_account_ip_associate_post) | **POST** /corporate/subAccount/ip/associate | Associate an IP to sub-accounts
[**corporate_sub_account_ip_dissociate_put**](MasterAccountApi.md#corporate_sub_account_ip_dissociate_put) | **PUT** /corporate/subAccount/ip/dissociate | Dissociate an IP to sub-accounts
[**corporate_sub_account_key_post**](MasterAccountApi.md#corporate_sub_account_key_post) | **POST** /corporate/subAccount/key | Create an API key for a sub-account
[**corporate_sub_account_post**](MasterAccountApi.md#corporate_sub_account_post) | **POST** /corporate/subAccount | Create a new sub-account under a master account.
[**corporate_sub_account_sso_token_post**](MasterAccountApi.md#corporate_sub_account_sso_token_post) | **POST** /corporate/subAccount/ssoToken | Generate SSO token to access sub-account
[**corporate_sub_accounts_plan_put**](MasterAccountApi.md#corporate_sub_accounts_plan_put) | **PUT** /corporate/subAccounts/plan | Update sub-accounts plan
[**corporate_user_email_permissions_put**](MasterAccountApi.md#corporate_user_email_permissions_put) | **PUT** /corporate/user/{email}/permissions | Change admin user permissions
[**corporate_user_invitation_action_email_put**](MasterAccountApi.md#corporate_user_invitation_action_email_put) | **PUT** /corporate/user/invitation/{action}/{email} | Resend / cancel admin user invitation
[**corporate_user_revoke_email_delete**](MasterAccountApi.md#corporate_user_revoke_email_delete) | **DELETE** /corporate/user/revoke/{email} | Revoke an admin user
[**get_account_activity**](MasterAccountApi.md#get_account_activity) | **GET** /organization/activities | Get user activity logs
[**get_corporate_invited_users_list**](MasterAccountApi.md#get_corporate_invited_users_list) | **GET** /corporate/invited/users | Get the list of all admin users
[**get_corporate_user_permission**](MasterAccountApi.md#get_corporate_user_permission) | **GET** /corporate/user/{email}/permissions | Check admin user permissions
[**get_sub_account_groups**](MasterAccountApi.md#get_sub_account_groups) | **GET** /corporate/groups | Get the list of groups
[**invite_admin_user**](MasterAccountApi.md#invite_admin_user) | **POST** /corporate/user/invitation/send | Send invitation to an admin user



## corporate_group_id_delete

> corporate_group_id_delete(id)
Delete a group

This endpoint allows you to delete a group of sub-organizations. When a group is deleted, the sub-organizations are no longer part of this group. The users associated with the group are no longer associated with the group once deleted.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | Id of the group | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_group_id_get

> models::CorporateGroupDetailsResponse corporate_group_id_get(id)
GET a group details

This endpoint allows you to retrieve a specific group’s information such as the list of sub-organizations and the user associated with the group.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | Id of the group of sub-organization | [required] |

### Return type

[**models::CorporateGroupDetailsResponse**](corporateGroupDetailsResponse.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_group_id_put

> corporate_group_id_put(id, corporate_group_id_put_request)
Update a group of sub-accounts

This endpoint allows to update a group of sub-accounts

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | Id of the group | [required] |
**corporate_group_id_put_request** | [**CorporateGroupIdPutRequest**](CorporateGroupIdPutRequest.md) | Group details to be updated. | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_group_post

> models::CorporateGroupPost201Response corporate_group_post(corporate_group_post_request)
Create a group of sub-accounts

This endpoint allows to create a group of sub-accounts

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**corporate_group_post_request** | Option<[**CorporateGroupPostRequest**](CorporateGroupPostRequest.md)> |  |  |

### Return type

[**models::CorporateGroupPost201Response**](_corporate_group_post_201_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_group_unlink_group_id_sub_accounts_put

> corporate_group_unlink_group_id_sub_accounts_put(group_id, corporate_group_unlink_group_id_sub_accounts_put_request)
Delete sub-account from group

This endpoint allows you to remove a sub-organization from a group.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**group_id** | **String** | Group id | [required] |
**corporate_group_unlink_group_id_sub_accounts_put_request** | [**CorporateGroupUnlinkGroupIdSubAccountsPutRequest**](CorporateGroupUnlinkGroupIdSubAccountsPutRequest.md) | List of sub-account ids | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_ip_get

> Vec<models::CorporateIpGet200ResponseInner> corporate_ip_get()
List of all IPs

This endpoint allows you to retrieve the list of active IPs on your Admin account

### Parameters

This endpoint does not need any parameter.

### Return type

[**Vec<models::CorporateIpGet200ResponseInner>**](_corporate_ip_get_200_response_inner.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_master_account_get

> models::MasterDetailsResponse corporate_master_account_get()
Get the details of requested master account

This endpoint will provide the details of the master account.

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::MasterDetailsResponse**](masterDetailsResponse.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_sso_token_post

> models::GetSsoToken corporate_sso_token_post(corporate_sso_token_post_request)
Generate SSO token to access admin account

This endpoint generates an SSO token to authenticate and access the admin account using the endpoint https://account-app.brevo.com/account/login/corporate/sso/[token], where [token] will be replaced by the actual token.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**corporate_sso_token_post_request** | Option<[**CorporateSsoTokenPostRequest**](CorporateSsoTokenPostRequest.md)> |  |  |

### Return type

[**models::GetSsoToken**](getSsoToken.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_sub_account_get

> models::SubAccountsResponse corporate_sub_account_get(offset, limit)
Get the list of all the sub-accounts of the master account.

This endpoint will provide the list all the sub-accounts of the master account.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**offset** | **i32** | Index of the first sub-account in the page | [required] |
**limit** | **i32** | Number of sub-accounts to be displayed on each page | [required] |

### Return type

[**models::SubAccountsResponse**](subAccountsResponse.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_sub_account_id_applications_toggle_put

> corporate_sub_account_id_applications_toggle_put(id, sub_account_apps_toggle_request)
Enable/disable sub-account application(s)

API endpoints for the Corporate owner to enable/disable applications on the sub-account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i64** | Id of the sub-account organization (mandatory) | [required] |
**sub_account_apps_toggle_request** | [**SubAccountAppsToggleRequest**](SubAccountAppsToggleRequest.md) | List of applications to activate or deactivate on a sub-account | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_sub_account_id_delete

> corporate_sub_account_id_delete(id)
Delete a sub-account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i64** | Id of the sub-account organization to be deleted | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_sub_account_id_get

> models::SubAccountDetailsResponse corporate_sub_account_id_get(id)
Get sub-account details

This endpoint will provide the details for the specified sub-account company

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i64** | Id of the sub-account organization | [required] |

### Return type

[**models::SubAccountDetailsResponse**](subAccountDetailsResponse.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_sub_account_id_plan_put

> corporate_sub_account_id_plan_put(id, sub_account_update_plan_request)
Update sub-account plan

This endpoint will update the sub-account plan. On the Corporate solution new version v2, you can set an unlimited number of credits in your sub-organization. Please pass the value “-1\" to set the consumable in unlimited mode.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **i64** | Id of the sub-account organization | [required] |
**sub_account_update_plan_request** | [**SubAccountUpdatePlanRequest**](SubAccountUpdatePlanRequest.md) | Values to update a sub-account plan | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_sub_account_ip_associate_post

> serde_json::Value corporate_sub_account_ip_associate_post(corporate_sub_account_ip_associate_post_request)
Associate an IP to sub-accounts

This endpoint allows to associate an IP to sub-accounts

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**corporate_sub_account_ip_associate_post_request** | Option<[**CorporateSubAccountIpAssociatePostRequest**](CorporateSubAccountIpAssociatePostRequest.md)> |  |  |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_sub_account_ip_dissociate_put

> corporate_sub_account_ip_dissociate_put(corporate_sub_account_ip_dissociate_put_request)
Dissociate an IP to sub-accounts

This endpoint allows to dissociate an IP from sub-accounts

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**corporate_sub_account_ip_dissociate_put_request** | Option<[**CorporateSubAccountIpDissociatePutRequest**](CorporateSubAccountIpDissociatePutRequest.md)> |  |  |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_sub_account_key_post

> models::CreateApiKeyResponse corporate_sub_account_key_post(corporate_sub_account_key_post_request)
Create an API key for a sub-account

This endpoint will generate an API v3 key for a sub account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**corporate_sub_account_key_post_request** | Option<[**CorporateSubAccountKeyPostRequest**](CorporateSubAccountKeyPostRequest.md)> |  |  |

### Return type

[**models::CreateApiKeyResponse**](createApiKeyResponse.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_sub_account_post

> models::CreateSubAccountResponse corporate_sub_account_post(create_sub_account)
Create a new sub-account under a master account.

This endpoint will create a new sub-account under a master account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_sub_account** | [**CreateSubAccount**](CreateSubAccount.md) | Request body with sub-account organization name | [required] |

### Return type

[**models::CreateSubAccountResponse**](createSubAccountResponse.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_sub_account_sso_token_post

> models::GetSsoToken corporate_sub_account_sso_token_post(corporate_sub_account_sso_token_post_request)
Generate SSO token to access sub-account

This endpoint generates an sso token to authenticate and access a sub-account of the master using the account endpoint https://account-app.brevo.com/account/login/sub-account/sso/[token], where [token] will be replaced by the actual token.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**corporate_sub_account_sso_token_post_request** | Option<[**CorporateSubAccountSsoTokenPostRequest**](CorporateSubAccountSsoTokenPostRequest.md)> |  |  |

### Return type

[**models::GetSsoToken**](getSsoToken.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_sub_accounts_plan_put

> corporate_sub_accounts_plan_put(sub_accounts_update_plan_request)
Update sub-accounts plan

This endpoint will update multiple sub-accounts plan. On the Corporate solution new version v2, you can set an unlimited number of credits in your sub-organization. Please pass the value “-1\" to set the consumable in unlimited mode.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**sub_accounts_update_plan_request** | [**SubAccountsUpdatePlanRequest**](SubAccountsUpdatePlanRequest.md) | Values to update sub-accounts plan | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_user_email_permissions_put

> corporate_user_email_permissions_put(email, corporate_user_email_permissions_put_request)
Change admin user permissions

This endpoint will allow you to change the permissions of Admin users of your Admin account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**email** | **String** | Email address of Admin user | [required] |
**corporate_user_email_permissions_put_request** | [**CorporateUserEmailPermissionsPutRequest**](CorporateUserEmailPermissionsPutRequest.md) | Values to update an admin user permissions | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_user_invitation_action_email_put

> models::CorporateUserInvitationActionEmailPut200Response corporate_user_invitation_action_email_put(action, email)
Resend / cancel admin user invitation

This endpoint will allow the user to: - Resend an admin user invitation - Cancel an admin user invitation 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**action** | **String** | Action to be performed (cancel / resend) | [required] |
**email** | **String** | Email address of the recipient | [required] |

### Return type

[**models::CorporateUserInvitationActionEmailPut200Response**](_corporate_user_invitation__action___email__put_200_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## corporate_user_revoke_email_delete

> corporate_user_revoke_email_delete(email)
Revoke an admin user

This endpoint allows to revoke/remove an invited member of your Admin account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**email** | **String** | Email of the invited user | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account_activity

> models::GetAccountActivity get_account_activity(start_date, end_date, email, limit, offset)
Get user activity logs

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**start_date** | Option<**String**> | Mandatory if endDate is used. Enter start date in UTC date (YYYY-MM-DD) format to filter the activity in your account. Maximum time period that can be selected is one month. Additionally, you can retrieve activity logs from the past 12 months from the date of your search. |  |
**end_date** | Option<**String**> | Mandatory if startDate is used. Enter end date in UTC date (YYYY-MM-DD) format to filter the activity in your account. Maximum time period that can be selected is one month. |  |
**email** | Option<**String**> | Enter the user's email address to filter their activity in the account. |  |
**limit** | Option<**i64**> | Number of documents per page |  |[default to 10]
**offset** | Option<**i64**> | Index of the first document in the page. |  |[default to 0]

### Return type

[**models::GetAccountActivity**](getAccountActivity.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_corporate_invited_users_list

> models::GetCorporateInvitedUsersList get_corporate_invited_users_list()
Get the list of all admin users

This endpoint allows you to list all Admin users of your Admin account

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::GetCorporateInvitedUsersList**](getCorporateInvitedUsersList.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_corporate_user_permission

> models::GetCorporateUserPermission get_corporate_user_permission(email)
Check admin user permissions

This endpoint will provide the list of admin user permissions

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**email** | **String** | Email of the invited user. | [required] |

### Return type

[**models::GetCorporateUserPermission**](getCorporateUserPermission.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_sub_account_groups

> Vec<models::GetSubAccountGroups200ResponseInner> get_sub_account_groups()
Get the list of groups

This endpoint allows you to list all groups created on your Admin account.

### Parameters

This endpoint does not need any parameter.

### Return type

[**Vec<models::GetSubAccountGroups200ResponseInner>**](getSubAccountGroups_200_response_inner.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## invite_admin_user

> models::CorporateGroupPost201Response invite_admin_user(invite_admin_user)
Send invitation to an admin user

`This endpoint allows you to invite a member to manage the Admin account  Features and their respective permissions are as below:  - `my_plan`:   - \"all\" - `api`:   - \"none\" - `user_management`:   - \"all\" - `app_management` | Not available in ENTv2:   - \"all\" - `sub_organization_groups`   - \"create\"   - \"edit_delete\" - `create_sub_organizations`   - \"all\" - `manage_sub_organizations`   - \"all\" - `analytics`   - \"download_data\"   - \"create_alerts\"   - \"my_looks\"   - \"explore_create\" - `security`   - \"all\"  **Note**: - If `all_features_access: false` then only privileges are required otherwise if `true` then it's assumed that all permissions will be there for the invited admin user. 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**invite_admin_user** | [**InviteAdminUser**](InviteAdminUser.md) | Payload to send an invitation | [required] |

### Return type

[**models::CorporateGroupPost201Response**](_corporate_group_post_201_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


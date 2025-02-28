# \UserApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**edit_user_permission**](UserApi.md#edit_user_permission) | **POST** /organization/user/update/permissions | Update permission for a user
[**get_invited_users_list**](UserApi.md#get_invited_users_list) | **GET** /organization/invited/users | Get the list of all your users
[**get_user_permission**](UserApi.md#get_user_permission) | **GET** /organization/user/{email}/permissions | Check user permission
[**inviteuser**](UserApi.md#inviteuser) | **POST** /organization/user/invitation/send | Send invitation to user
[**put_revoke_user_permission**](UserApi.md#put_revoke_user_permission) | **PUT** /organization/user/invitation/revoke/{email} | Revoke user permission
[**putresendcancelinvitation**](UserApi.md#putresendcancelinvitation) | **PUT** /organization/user/invitation/{action}/{email} | Resend / Cancel invitation



## edit_user_permission

> models::UpdateUserResponse edit_user_permission(inviteuser)
Update permission for a user

`Feature` - A Feature represents a specific functionality like Email campaign, Deals, Calls, Automations, etc. on Brevo. While inviting a user, determine which feature you want to manage access to. You must specify the feature accurately to avoid errors.  `Permission` - A Permission defines the level of access or control a user has over a specific feature. While inviting user, decide on the permission level required for the selected feature. Make sure the chosen permission is related to the selected feature.  Features and their respective permissions are as below:  - `email_campaigns`:   - \"create_edit_delete\"   - \"send_schedule_suspend\" - `sms_campaigns`:   - \"create_edit_delete\"   - \"send_schedule_suspend\" - `contacts`:   - \"view\"   - \"create_edit_delete\"   - \"import\"   - \"export\"   - \"list_and_attributes\"   - \"forms\" - `templates`:   - \"create_edit_delete\"   - \"activate_deactivate\" - `workflows`:   - \"create_edit_delete\"   - \"activate_deactivate_pause\"   - \"settings\" - `facebook_ads`:   - \"create_edit_delete\"   - \"schedule_pause\" - `landing_pages`:   - \"all\" - `transactional_emails`:   - \"settings\"   - \"logs\" - `smtp_api`:   - \"smtp\"   - \"api_keys\"   - \"authorized_ips\" - `user_management`:   - \"all\" - `sales_platform`:   - \"create_edit_deals\"   - \"delete_deals\"   - \"manage_others_deals_tasks\"   - \"reports\"   - \"settings\" - `phone`:   - \"all\" - `conversations`:   - \"access\"   - \"assign\"   - \"configure\" - `senders_domains_dedicated_ips`:   - \"senders_management\"   - \"domains_management\"   - \"dedicated_ips_management\" - `push_notifications`:   - \"view\"   - \"create_edit_delete\"   - \"send\"   - \"settings\" - `companies`:   - \"manage_owned_companies\"   - \"manage_other_companies\"   - \"settings\"  **Note**: - The privileges array remains the same as in the send invitation; the user simply needs to provide the permissions that need to be updated. - The availability of feature and its permission depends on your current plan. Please select the features and permissions accordingly. 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**inviteuser** | [**Inviteuser**](Inviteuser.md) | Values to create an invitation | [required] |

### Return type

[**models::UpdateUserResponse**](updateUserResponse.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_invited_users_list

> models::GetInvitedUsersList get_invited_users_list()
Get the list of all your users

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::GetInvitedUsersList**](getInvitedUsersList.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_user_permission

> models::GetUserPermission get_user_permission(email)
Check user permission

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**email** | **String** | Email of the invited user. | [required] |

### Return type

[**models::GetUserPermission**](getUserPermission.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## inviteuser

> models::InviteuserResponse inviteuser(inviteuser)
Send invitation to user

`Feature` - A Feature represents a specific functionality like Email campaign, Deals, Calls, Automations, etc. on Brevo. While inviting a user, determine which feature you want to manage access to. You must specify the feature accurately to avoid errors.  `Permission` - A Permission defines the level of access or control a user has over a specific feature. While inviting user, decide on the permission level required for the selected feature. Make sure the chosen permission is related to the selected feature.  Features and their respective permissions are as below:  - `email_campaigns`:   - \"create_edit_delete\"   - \"send_schedule_suspend\" - `sms_campaigns`:   - \"create_edit_delete\"   - \"send_schedule_suspend\" - `contacts`:   - \"view\"   - \"create_edit_delete\"   - \"import\"   - \"export\"   - \"list_and_attributes\"   - \"forms\" - `templates`:   - \"create_edit_delete\"   - \"activate_deactivate\" - `workflows`:   - \"create_edit_delete\"   - \"activate_deactivate_pause\"   - \"settings\" - `facebook_ads`:   - \"create_edit_delete\"   - \"schedule_pause\" - `landing_pages`:   - \"all\" - `transactional_emails`:   - \"settings\"   - \"logs\" - `smtp_api`:   - \"smtp\"   - \"api_keys\"   - \"authorized_ips\" - `user_management`:   - \"all\" - `sales_platform`:   - \"create_edit_deals\"   - \"delete_deals\"   - \"manage_others_deals_tasks\"   - \"reports\"   - \"settings\" - `phone`:   - \"all\" - `conversations`:   - \"access\"   - \"assign\"   - \"configure\" - `senders_domains_dedicated_ips`:   - \"senders_management\"   - \"domains_management\"   - \"dedicated_ips_management\" - `push_notifications`:   - \"view\"   - \"create_edit_delete\"   - \"send\"   - \"settings\" - `companies`:   - \"manage_owned_companies\"   - \"manage_other_companies\"   - \"settings\"  **Note**: - If `all_features_access: false` then only privileges are required otherwise if `true` then it's assumed that all permissions will be there for the invited user. - The availability of feature and its permission depends on your current plan. Please select the features and permissions accordingly. 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**inviteuser** | [**Inviteuser**](Inviteuser.md) | Values to create an invitation | [required] |

### Return type

[**models::InviteuserResponse**](inviteuserResponse.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## put_revoke_user_permission

> models::PutRevokeUserPermissionResponse put_revoke_user_permission(email)
Revoke user permission

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**email** | **String** | Email of the invited user. | [required] |

### Return type

[**models::PutRevokeUserPermissionResponse**](putRevokeUserPermissionResponse.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## putresendcancelinvitation

> models::PutresendcancelinvitationResponse putresendcancelinvitation(action, email)
Resend / Cancel invitation

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**action** | **String** | action | [required] |
**email** | **String** | Email of the invited user. | [required] |

### Return type

[**models::PutresendcancelinvitationResponse**](putresendcancelinvitationResponse.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


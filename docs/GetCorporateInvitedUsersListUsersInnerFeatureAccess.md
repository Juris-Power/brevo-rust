# GetCorporateInvitedUsersListUsersInnerFeatureAccess

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_management** | Option<**Vec<String>**> | User management accessiblity. | [optional]
**api_keys** | Option<**Vec<String>**> | Api keys accessiblity. | [optional]
**my_plan** | Option<**Vec<String>**> | My plan accessiblity. | [optional]
**apps_management** | Option<**Vec<String>**> | Apps management accessiblity | Not available in ENTv2 | [optional]
**sub_organization_groups** | Option<**Vec<String>**> | Group creation, modification or deletion accessibility | [optional]
**create_sub_organizations** | Option<**Vec<String>**> | Authorization to create sub-organization in the admin account. If the user creating the sub-organization, belongs to a group, the user must choose a group at the sub-organization creation. | [optional]
**manage_sub_organizations** | Option<**Vec<String>**> | Authorization to manage and access sub-organizations in the admin account. | [optional]
**analytics** | Option<**Vec<String>**> | Analytics dashboard accessibility | [optional]
**security** | Option<**Vec<String>**> | Security page accessibility | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



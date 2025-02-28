# CompaniesPostRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **String** | Name of company | 
**attributes** | Option<[**serde_json::Value**](.md)> | Attributes for company creation | [optional]
**country_code** | Option<**i64**> | Country code if phone_number is passed in attributes. | [optional]
**linked_contacts_ids** | Option<**Vec<i64>**> | Contact ids to be linked with company | [optional]
**linked_deals_ids** | Option<**Vec<String>**> | Deal ids to be linked with company | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



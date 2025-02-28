# CompaniesIdPatchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | Option<**String**> | Name of company | [optional]
**attributes** | Option<[**serde_json::Value**](.md)> | Attributes for company update | [optional]
**country_code** | Option<**i64**> | Country code if phone_number is passed in attributes. | [optional]
**linked_contacts_ids** | Option<**Vec<i64>**> | Warning - Using PATCH on linkedContactIds replaces the list of linked contacts. Omitted IDs will be removed. | [optional]
**linked_deals_ids** | Option<**Vec<String>**> | Warning - Using PATCH on linkedDealsIds replaces the list of linked contacts. Omitted IDs will be removed. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



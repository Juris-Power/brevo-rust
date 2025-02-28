# CrmDealsPostRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **String** | Name of deal | 
**attributes** | Option<[**serde_json::Value**](.md)> | Attributes for deal creation  To assign owner of a Deal you can send attributes.deal_owner and utilize the account email or ID.  If you want to create a deal on a specific pipeline and stage you can use the following attributes `pipeline` and `deal_stage`.  Pipeline and deal_stage are ids you can fetch using this endpoint `/crm/pipeline/details/{pipelineID}`  | [optional]
**linked_contacts_ids** | Option<**Vec<i64>**> | Contact ids to be linked with deal | [optional]
**linked_companies_ids** | Option<**Vec<String>**> | Company ids to be linked with deal | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



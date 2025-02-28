# CrmDealsIdPatchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | Option<**String**> | Name of deal | [optional]
**attributes** | Option<[**serde_json::Value**](.md)> | Attributes for deal update  To assign owner of a Deal you can send attributes.deal_owner and utilize the account email or ID.  If you wish to update the pipeline of a deal you need to provide the `pipeline` and the `deal_stage`  Pipeline and deal_stage are ids you can fetch using this endpoint `/crm/pipeline/details/{pipelineID}`  | [optional]
**linked_contact_ids** | Option<**Vec<i64>**> | Warning - Using PATCH on linkedContactIds replaces the list of linked contacts. Omitted IDs will be removed. | [optional]
**linked_companies_ids** | Option<**Vec<String>**> | Warning - Using PATCH on linkedCompaniesIds replaces the list of linked contacts. Omitted IDs will be removed. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



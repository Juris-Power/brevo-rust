# Getrecords200ResponseRecordsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | Option<**String**> | Timestamp when the object record was created | [optional]
**updated_at** | Option<**String**> | Timestamp when the object record was last updated | [optional]
**identifiers** | Option<[**models::Getrecords200ResponseRecordsInnerIdentifiers**](getrecords_200_response_records_inner_identifiers.md)> |  | [optional]
**attributes** | Option<[**serde_json::Value**](.md)> | Attributes attached with the object record. Only the already created attributes will be used with records. Minimum 1 attribute is required.  | [optional]
**associations** | Option<[**Vec<models::Getrecords200ResponseRecordsInnerAssociationsInner>**](getrecords_200_response_records_inner_associations_inner.md)> | List of associations for the object record. If association query param is true it will return 5 associated records per association. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



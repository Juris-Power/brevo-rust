# TierForContact

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Unique identifier for the assigned tier | [optional]
**loyalty_program_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Associated loyalty program Id | [optional]
**group_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Group Id to which the tier is associated | [optional]
**contact_id** | Option<**i32**> | Contact to which the tier is assigned | [optional]
**meta** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> | object | [optional]
**created_at** | Option<**String**> |  | [optional]
**updated_at** | Option<**String**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



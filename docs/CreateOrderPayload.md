# CreateOrderPayload

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **f64** | Order amount (must be non-zero). | 
**balance_definition_id** | **String** | Unique identifier (UUID) of the associated balance definition. | 
**contact_id** | **i32** | Unique identifier of the contact placing the order (must be ≥ 1). | 
**due_at** | **String** | RFC3339 timestamp specifying when the order is due. | 
**expires_at** | Option<**String**> | Optional RFC3339 timestamp defining order expiration. | [optional]
**meta** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> | Optional metadata associated with the order. | [optional]
**source** | **String** | Specifies the origin of the order (`engine` or `user`). | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



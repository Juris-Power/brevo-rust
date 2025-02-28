# Transaction

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | Option<**f64**> | The transaction amount. | [optional]
**balance_definition_id** | Option<**String**> | Unique identifier (UUID) of the associated balance definition. | [optional]
**cancelled_at** | Option<**String**> | Timestamp when the transaction was canceled (nullable). | [optional]
**completed_at** | Option<**String**> | Timestamp when the transaction was completed (nullable). | [optional]
**contact_id** | Option<**i32**> | Unique identifier of the contact associated with the transaction. | [optional]
**created_at** | Option<**String**> | Timestamp when the transaction was created. | [optional]
**event_time** | Option<**String**> | Optional timestamp indicating when the transaction event occurred. | [optional]
**expiration_date** | Option<**String**> | Expiry date of the transaction (nullable). | [optional]
**id** | Option<**String**> | Unique identifier (UUID) of the transaction. | [optional]
**loyalty_program_id** | Option<**String**> | Unique identifier (UUID) of the associated loyalty program. | [optional]
**meta** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> | Optional metadata associated with the transaction. | [optional]
**reject_reason** | Option<**String**> | Reason for rejection if the transaction was declined (nullable). | [optional]
**rejected_at** | Option<**String**> | Timestamp when the transaction was rejected (nullable). | [optional]
**status** | Option<**String**> | The current status of the transaction (e.g., pending, completed, rejected). | [optional]
**updated_at** | Option<**String**> | Timestamp when the transaction was last updated. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



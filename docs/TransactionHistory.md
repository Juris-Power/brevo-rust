# TransactionHistory

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | Option<**f64**> | The transaction amount. | [optional]
**balance_expiration_date** | Option<**String**> | Expiration date of the balance associated with this transaction. | [optional]
**cancelled_at** | Option<**String**> | Timestamp when the transaction was canceled, if applicable. | [optional]
**completed_at** | Option<**String**> | Timestamp when the transaction was successfully completed. | [optional]
**created_at** | Option<**String**> | Timestamp when the transaction was initiated. | [optional]
**id** | Option<**String**> | Unique identifier of the transaction. | [optional]
**meta** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> | Optional metadata associated with the transaction. | [optional]
**reject_reason** | Option<**String**> | Reason for rejection, if the transaction was declined. | [optional]
**rejected_at** | Option<**String**> | Timestamp when the transaction was rejected. | [optional]
**status** | Option<**String**> | Current status of the transaction (e.g., pending, completed, rejected). | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# TransactionHistoryResp

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**balance_definition_id** | Option<**String**> | Unique identifier of the associated balance definition. | [optional]
**contact_id** | Option<**i32**> | Unique identifier of the contact related to the transactions. | [optional]
**count** | Option<**i32**> | Total number of transactions in the history. | [optional]
**loyalty_program_id** | Option<**String**> | Unique identifier of the associated loyalty program. | [optional]
**transaction_history** | Option<[**Vec<models::TransactionHistory>**](transactionHistory.md)> | List of past transactions associated with the balance. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



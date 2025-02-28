# BalanceLimit

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**balance_definition_id** | Option<**String**> | balance definition ID | [optional]
**constraint_type** | Option<**String**> | Defines the type of constraint (e.g., transaction-based or amount-based). | [optional]
**created_at** | **String** | Timestamp of when the balance limit was created. | 
**duration_unit** | Option<**String**> | Time unit for the balance limit (day, week, month, year). | [optional]
**duration_value** | Option<**i32**> | Number of time units the balance limit applies to. | [optional]
**id** | Option<**String**> | Unique identifier for the balance limit. | [optional]
**sliding_schedule** | Option<**bool**> | Indicates if the limit resets periodically based on a sliding schedule. | [optional]
**transaction_type** | Option<**String**> | Specifies whether the limit applies to credit or debit transactions. | [optional]
**updated_at** | **String** | Timestamp of the last update to the balance limit. | 
**value** | Option<**i32**> | The maximum allowed value for the defined constraint. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# MainPeriodRedeem

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cancelled_at** | Option<**String**> | Timestamp when the redemption was cancelled | [optional]
**completed_at** | Option<**String**> | Timestamp when the redemption was completed | [optional]
**contact_id** | Option<**i64**> | Unique identifier for the contact | [optional]
**created_at** | Option<**String**> | Timestamp when the redemption was created | [optional]
**debit_transaction_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Unique identifier for the debit transaction | [optional]
**expires_at** | Option<**String**> | Timestamp when the redemption expires | [optional]
**id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Unique identifier for the redemption | [optional]
**loyalty_program_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Unique identifier for the loyalty program | [optional]
**meta** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> | Additional metadata associated with the redemption | [optional]
**reject_reason** | Option<**String**> | Reason for rejection if the redemption was rejected | [optional]
**rejected_at** | Option<**String**> | Timestamp when the redemption was rejected | [optional]
**reward_attribution_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Unique identifier for the reward attribution | [optional]
**status** | Option<**String**> | Current status of the redemption | [optional]
**updated_at** | Option<**String**> | Timestamp when the redemption was last updated | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



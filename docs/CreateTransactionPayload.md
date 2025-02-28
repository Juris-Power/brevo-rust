# CreateTransactionPayload

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**loyalty_subscription_id** | Option<**String**> | Unique identifier for the loyalty subscription (required unless `contactId` is provided). | [optional]
**amount** | **f64** | Transaction amount (must be provided). | 
**auto_complete** | Option<**bool**> | Whether the transaction should be automatically completed. | [optional]
**balance_definition_id** | **String** | Unique identifier (UUID) of the associated balance definition. | 
**balance_expiry_in_minutes** | Option<**i32**> | Optional expiry time for the balance in minutes (must be greater than 0 if provided). | [optional]
**contact_id** | Option<**i32**> | Unique identifier of the contact involved in the transaction (required unless `LoyaltySubscriptionId` is provided). | [optional]
**event_time** | Option<**String**> | Optional timestamp specifying when the transaction occurred. | [optional]
**meta** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> | Optional metadata associated with the transaction. | [optional]
**ttl** | Option<**i32**> | Optional time-to-live for the transaction (must be greater than 0 if provided). | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



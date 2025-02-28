# MainPeriodCreateRedeemPayload

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**attributed_reward_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Unique identifier for the attributed reward | [optional]
**code** | Option<**String**> | Redemption code for the reward | [optional]
**contact_id** | Option<**i64**> | Unique identifier for the contact | [optional]
**loyalty_subscription_id** | Option<**String**> | Identifier for the loyalty subscription | [optional]
**meta** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> | Additional metadata associated with the redeem request | [optional]
**order** | Option<[**models::MainPeriodOrderPayload**](main.orderPayload.md)> | Order details for the redemption | [optional]
**reward_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Unique identifier for the reward | [optional]
**ttl** | Option<**i32**> | Time to live in seconds for the redemption request | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



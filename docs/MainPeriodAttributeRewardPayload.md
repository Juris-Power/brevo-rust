# MainPeriodAttributeRewardPayload

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | Option<**f64**> | Value of the selected reward config | [optional]
**code** | Option<**String**> | Code generated to attribute reward to a contact | [optional]
**contact_id** | Option<**i64**> | Contact to attribute the reward | [optional]
**expiration_date** | Option<**String**> | Reward expiration date | [optional]
**loyalty_subscription_id** | Option<**String**> | One of contactId or loyaltySubscriptionId is required | [optional]
**meta** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> | Offer meta information (key/value object) | [optional]
**reward_id** | [**uuid::Uuid**](uuid::Uuid.md) | Reward id | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



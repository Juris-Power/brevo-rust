# Tier

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tier_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Tier id | [optional]
**name** | Option<**String**> | Tier name | [optional]
**image_ref** | Option<**String**> | Tier image reference | [optional]
**loyalty_program_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Associated loyalty program Id | [optional]
**group_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Associated group Id | [optional]
**created_at** | Option<**String**> |  | [optional]
**updated_at** | Option<**String**> |  | [optional]
**access_conditions** | Option<[**Vec<models::TierAccessConditionsInner>**](tier_accessConditions_inner.md)> | Conditions required to access this tier | [optional]
**tier_rewards** | Option<[**Vec<models::TierTierRewardsInner>**](tier_tierRewards_inner.md)> | Rewards associated with this tier | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



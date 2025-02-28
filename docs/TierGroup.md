# TierGroup

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Tier group unique identifier | [optional]
**name** | Option<**String**> | Tier group name | [optional]
**tier_order** | Option<[**Vec<uuid::Uuid>**](uuid::Uuid.md)> | Order of the tiers in the group in ascending order | [optional]
**loyalty_program_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Associated loyalty program Id | [optional]
**upgrade_strategy** | Option<**String**> | Select real_time to upgrade tier on real time balance updates. Select membership_anniversary to upgrade tier on subscription anniversary. Select tier_anniversary to upgrade tier on tier anniversary. | [optional][default to RealTime]
**downgrade_strategy** | Option<**String**> | Select real_time to downgrade tier on real time balance updates. Select membership_anniversary to downgrade tier on subscription anniversary. Select tier_anniversary to downgrade tier on tier anniversary. | [optional][default to RealTime]
**created_at** | Option<**String**> | Timestamp when the tier group was created | [optional]
**updated_at** | Option<**String**> | Timestamp when the tier group was last updated | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



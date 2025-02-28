# UpdateTierGroupRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **String** | Name of the tier group | 
**tier_order** | [**Vec<uuid::Uuid>**](uuid::Uuid.md) | Order of the tiers in the group in ascending order | 
**upgrade_strategy** | **String** | Select real_time to upgrade tier on real time balance updates. Select membership_anniversary to upgrade tier on subscription anniversary. Select tier_anniversary to upgrade tier on tier anniversary. | [default to RealTime]
**downgrade_strategy** | **String** | Select real_time to downgrade tier on real time balance updates. Select membership_anniversary to downgrade tier on subscription anniversary. Select tier_anniversary to downgrade tier on tier anniversary. | [default to RealTime]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CreateEmailCampaignRecipients

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**exclusion_list_ids** | Option<**Vec<i64>**> | List ids to exclude from the campaign | [optional]
**list_ids** | Option<**Vec<i64>**> | **Mandatory if scheduledAt is not empty**. List Ids to send the campaign to  | [optional]
**segment_ids** | Option<**Vec<i64>**> | **Mandatory if listIds are not used**. Segment ids to send the campaign to.  | [optional]
**exclusion_segment_ids** | Option<**Vec<i64>**> | Segment ids which have to be excluded from a campaign.  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



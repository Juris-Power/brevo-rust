# GetWhatsappCampaignsCampaignsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **i64** | ID of the WhatsApp Campaign | 
**campaign_name** | **String** | Name of the WhatsApp Campaign | 
**template_id** | **String** | Id of the WhatsApp template | 
**campaign_status** | **String** | Status of the WhatsApp Campaign | 
**scheduled_at** | **String** | UTC date-time on which WhatsApp campaign is scheduled. Should be in YYYY-MM-DDTHH:mm:ss.SSSZ format | 
**error_reason** | Option<**String**> | Error Reason associated with the WhatsApp campaign sending | [optional]
**invalidated_contacts** | Option<**i64**> | Count of invalidated contacts | [optional]
**read_percentage** | Option<**f32**> | Read percentage of the the WhatsApp campaign created | [optional]
**stats** | Option<[**models::WhatsappCampStats**](WhatsappCampStats.md)> |  | [optional]
**created_at** | **String** | Creation UTC date-time of the WhatsApp template (YYYY-MM-DDTHH:mm:ss.SSSZ) | 
**modified_at** | **String** | UTC date-time of last modification of the WhatsApp template (YYYY-MM-DDTHH:mm:ss.SSSZ) | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



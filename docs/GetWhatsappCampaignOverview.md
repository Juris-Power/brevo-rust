# GetWhatsappCampaignOverview

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **i64** | ID of the WhatsApp Campaign | 
**campaign_name** | **String** | Name of the WhatsApp Campaign | 
**campaign_status** | **String** | Status of the WhatsApp Campaign | 
**scheduled_at** | Option<**String**> | UTC date-time on which WhatsApp campaign is scheduled. Should be in YYYY-MM-DDTHH:mm:ss.SSSZ format | [optional]
**sender_number** | **String** | Sender of the WhatsApp Campaign | 
**stats** | Option<[**models::WhatsappCampStats**](WhatsappCampStats.md)> |  | [optional]
**template** | [**models::WhatsappCampTemplate**](WhatsappCampTemplate.md) |  | 
**created_at** | **String** | Creation UTC date-time of the WhatsApp campaign (YYYY-MM-DDTHH:mm:ss.SSSZ) | 
**modified_at** | **String** | UTC date-time of last modification of the WhatsApp campaign (YYYY-MM-DDTHH:mm:ss.SSSZ) | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



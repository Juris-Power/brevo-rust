# SendWhatsappMessageTemplate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template_id** | **i32** | ID of the template to send | 
**sender_number** | **String** | WhatsApp Number with country code. Example, 85264318721 | 
**params** | Option<[**serde_json::Value**](.md)> | Pass the set of attributes to customize the template. For example, {\"FNAME\":\"Joe\", \"LNAME\":\"Doe\"}. | [optional]
**contact_numbers** | **Vec<String>** | List of phone numbers of the contacts | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



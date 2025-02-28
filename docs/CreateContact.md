# CreateContact

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | Option<**String**> | Email address of the user. **Mandatory if \"ext_id\"  & \"SMS\" field is not passed.**  | [optional]
**ext_id** | Option<**String**> | Pass your own Id to create a contact. | [optional]
**attributes** | Option<[**std::collections::HashMap<String, models::CreateDoiContactAttributesValue>**](createDoiContact_attributes_value.md)> | Pass the set of attributes and their values. The attribute's parameter should be passed in capital letter while creating a contact. Values that don't match the attribute type (e.g. text or string in a date attribute) will be ignored. **These attributes must be present in your Brevo account.**. For eg: **{\"FNAME\":\"Elly\", \"LNAME\":\"Roger\", \"COUNTRIES\":[\"India\",\"China\"]}**  | [optional]
**email_blacklisted** | Option<**bool**> | Set this field to blacklist the contact for emails (emailBlacklisted = true) | [optional]
**sms_blacklisted** | Option<**bool**> | Set this field to blacklist the contact for SMS (smsBlacklisted = true) | [optional]
**list_ids** | Option<**Vec<i64>**> | Ids of the lists to add the contact to | [optional]
**update_enabled** | Option<**bool**> | Facilitate to update the existing contact in the same request (updateEnabled = true) | [optional][default to false]
**smtp_blacklist_sender** | Option<**Vec<String>**> | transactional email forbidden sender for contact. Use only for email Contact ( only available if updateEnabled = true ) | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



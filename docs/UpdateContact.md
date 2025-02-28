# UpdateContact

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**attributes** | Option<[**std::collections::HashMap<String, models::CreateDoiContactAttributesValue>**](createDoiContact_attributes_value.md)> | Pass the set of attributes to be updated. **These attributes must be present in your account**. To update existing email address of a contact with the new one please pass EMAIL in attributes. For example, **{ \"EMAIL\":\"newemail@domain.com\", \"FNAME\":\"Ellie\", \"LNAME\":\"Roger\", \"COUNTRIES\":[\"India\",\"China\"]}**. The attribute's parameter should be passed in capital letter while updating a contact. Values that don't match the attribute type (e.g. text or string in a date attribute) will be ignored. Keep in mind transactional attributes can be updated the same way as normal attributes. Mobile Number in **SMS** field should be passed with proper country code. For example: **{\"SMS\":\"+91xxxxxxxxxx\"} or {\"SMS\":\"0091xxxxxxxxxx\"}**  | [optional]
**ext_id** | Option<**String**> | Pass your own Id to update ext_id of a contact. | [optional]
**email_blacklisted** | Option<**bool**> | Set/unset this field to blacklist/allow the contact for emails (emailBlacklisted = true) | [optional]
**sms_blacklisted** | Option<**bool**> | Set/unset this field to blacklist/allow the contact for SMS (smsBlacklisted = true) | [optional]
**list_ids** | Option<**Vec<i64>**> | Ids of the lists to add the contact to | [optional]
**unlink_list_ids** | Option<**Vec<i64>**> | Ids of the lists to remove the contact from | [optional]
**smtp_blacklist_sender** | Option<**Vec<String>**> | transactional email forbidden sender for contact. Use only for email Contact | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



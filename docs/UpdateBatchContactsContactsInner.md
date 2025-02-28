# UpdateBatchContactsContactsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | Option<**String**> | Email address of the user to be updated (For each operation only pass one of the supported contact identifiers. Email, id or sms) | [optional]
**id** | Option<**i64**> | id of the user to be updated (For each operation only pass one of the supported contact identifiers. Email, id or sms) | [optional]
**sms** | Option<**String**> | SMS of the user to be updated (For each operation only pass one of the supported contact identifiers. Email, id or sms) | [optional]
**ext_id** | Option<**String**> | Pass your own Id to update ext_id of a contact. | [optional]
**attributes** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> | Pass the set of attributes to be updated. **These attributes must be present in your account**. To update existing email address of a contact with the new one please pass EMAIL in attribtes. For example, **{ \"EMAIL\":\"newemail@domain.com\", \"FNAME\":\"Ellie\", \"LNAME\":\"Roger\"}**. Keep in mind transactional attributes can be updated the same way as normal attributes. Mobile Number in **SMS** field should be passed with proper country code. For example: **{\"SMS\":\"+91xxxxxxxxxx\"} or {\"SMS\":\"0091xxxxxxxxxx\"}**  | [optional]
**email_blacklisted** | Option<**bool**> | Set/unset this field to blacklist/allow the contact for emails (emailBlacklisted = true) | [optional]
**sms_blacklisted** | Option<**bool**> | Set/unset this field to blacklist/allow the contact for SMS (smsBlacklisted = true) | [optional]
**list_ids** | Option<**Vec<i64>**> | Ids of the lists to add the contact to | [optional]
**unlink_list_ids** | Option<**Vec<i64>**> | Ids of the lists to remove the contact from | [optional]
**smtp_blacklist_sender** | Option<**Vec<String>**> | transactional email forbidden sender for contact. Use only for email Contact | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



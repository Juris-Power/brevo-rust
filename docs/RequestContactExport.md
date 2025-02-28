# RequestContactExport

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**export_attributes** | Option<**Vec<String>**> | List of all the attributes that you want to export. **These attributes must be present in your contact database. It is required if exportMandatoryAttributes is set false. ** For example: **['fname', 'lname', 'email']**  | [optional]
**custom_contact_filter** | [**models::RequestContactExportCustomContactFilter**](requestContactExport_customContactFilter.md) |  | 
**notify_url** | Option<**String**> | Webhook that will be called once the export process is finished. For reference, https://help.brevo.com/hc/en-us/articles/360007666479 | [optional]
**export_mandatory_attributes** | Option<**bool**> | To export mandatory attributes like EMAIL, ADDED_TIME, MODIFIED_TIME | [optional][default to true]
**export_subscription_status** | Option<**Vec<String>**> | Export subscription status of contacts for email & sms marketting. Pass email_marketing to obtain the marketing email subscription status & sms_marketing to retrieve the marketing SMS status of the contact. | [optional]
**export_metadata** | Option<**Vec<String>**> | Export metadata of contacts such as _listIds, ADDED_TIME, MODIFIED_TIME. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



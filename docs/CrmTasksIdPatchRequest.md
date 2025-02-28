# CrmTasksIdPatchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | Option<**String**> | Name of task | [optional]
**duration** | Option<**i64**> | Duration of task in milliseconds [1 minute = 60000 ms] | [optional]
**task_type_id** | Option<**String**> | Id for type of task e.g Call / Email / Meeting etc. | [optional]
**date** | Option<**String**> | Task date/time | [optional]
**notes** | Option<**String**> | Notes added to a task | [optional]
**done** | Option<**bool**> | Task marked as done | [optional]
**assign_to_id** | Option<**String**> | To assign a task to a user you can use either the account email or ID. | [optional]
**contacts_ids** | Option<**Vec<i32>**> | Contact ids for contacts linked to this task | [optional]
**deals_ids** | Option<**Vec<String>**> | Deal ids for deals a task is linked to | [optional]
**companies_ids** | Option<**Vec<String>**> | Companies ids for companies a task is linked to | [optional]
**reminder** | Option<[**models::TaskReminder**](TaskReminder.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# Note

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> | Unique note Id | [optional]
**text** | **String** | Text content of a note | 
**contact_ids** | Option<**Vec<i32>**> | Contact ids linked to a note | [optional]
**deal_ids** | Option<**Vec<String>**> | Deal ids linked to a note | [optional]
**author_id** | Option<[**serde_json::Value**](.md)> | Account details of user which created the note | [optional]
**created_at** | Option<**String**> | Note created date/time | [optional]
**updated_at** | Option<**String**> | Note updated date/time | [optional]
**pinned_at** | Option<**String**> | Note pinned date/time | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



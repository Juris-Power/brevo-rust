# TemplatePreviewRequestBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template_id** | **i32** | ID of the template to preview | 
**email** | Option<**String**> | Email of the contact.(Required if params not provided) | [optional]
**params** | Option<[**serde_json::Value**](.md)> | Key-value pairs of dynamic parameters for template rendering.(Required if email not provided) for example **{\"Firstname\":\"John\", \"Lastname\":\"Doe\"}** | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



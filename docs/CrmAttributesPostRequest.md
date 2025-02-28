# CrmAttributesPostRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**label** | **String** | The label for the attribute (max 50 characters, cannot be empty) | 
**attribute_type** | **String** | The type of attribute (must be one of the defined enums) | 
**description** | Option<**String**> | A description of the attribute | [optional]
**options_labels** | Option<**Vec<String>**> | Options for multi-choice or single-select attributes | [optional]
**object_type** | **String** | The type of object the attribute belongs to (prefilled with `companies` or `deal`, mandatory) | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



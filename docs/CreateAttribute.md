# CreateAttribute

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | Option<**String**> | Value of the attribute. **Use only if the attribute's category is 'calculated' or 'global'**  | [optional]
**is_recurring** | Option<**bool**> | Type of the attribute. **Use only if the attribute's category is 'calculated' or 'global'**  | [optional]
**enumeration** | Option<[**Vec<models::CreateAttributeEnumerationInner>**](createAttribute_enumeration_inner.md)> | List of values and labels that the attribute can take. **Use only if the attribute's category is \"category\"**. For example: **[{\"value\":1, \"label\":\"male\"}, {\"value\":2, \"label\":\"female\"}]**  | [optional]
**multi_category_options** | Option<**Vec<String>**> | List of options you want to add for multiple-choice attribute. **Use only if the attribute's category is \"normal\" and attribute's type is \"multiple-choice\".** For example: **[\"USA\",\"INDIA\"]**  | [optional]
**r#type** | Option<**String**> | Type of the attribute. **Use only if the attribute's category is 'normal', 'category' or 'transactional'** Type **user and multiple-choice** is only available if the category is **normal** attribute Type **id** is only available if the category is **transactional** attribute Type **category** is only available if the category is **category** attribute  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



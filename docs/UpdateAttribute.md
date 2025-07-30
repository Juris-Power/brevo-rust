# UpdateAttribute

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | Option<**String**> | Value of the attribute to update. **Use only if the attribute's category is 'calculated' or 'global'**  | [optional]
**enumeration** | Option<[**Vec<models::UpdateAttributeEnumerationInner>**](updateAttribute_enumeration_inner.md)> | List of the values and labels that the attribute can take. **Use only if the attribute's category is \"category\"**. None of the category options can exceed max 200 characters. For example, **[{\"value\":1, \"label\":\"male\"}, {\"value\":2, \"label\":\"female\"}]**  | [optional]
**multi_category_options** | Option<**Vec<String>**> | Use this option to add multiple-choice attributes options only if the attribute's category is \"normal\". **This option is specifically designed for updating multiple-choice attributes. None of the multicategory options can exceed max 200 characters.** For example: **[\"USA\",\"INDIA\"]**  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



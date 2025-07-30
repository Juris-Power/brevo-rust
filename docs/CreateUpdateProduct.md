# CreateUpdateProduct

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **String** | Product ID for which you requested the details | 
**name** | **String** | Mandatory in case of creation**. Name of the product for which you requested the details | 
**url** | Option<**String**> | URL to the product | [optional]
**image_url** | Option<**String**> | Absolute URL to the cover image of the product | [optional]
**sku** | Option<**String**> | Product identifier from the shop | [optional]
**price** | Option<**f32**> | Price of the product | [optional]
**categories** | Option<**Vec<String>**> | Category ID-s of the product | [optional]
**parent_id** | Option<**String**> | Parent product id of the product | [optional]
**meta_info** | Option<[**std::collections::HashMap<String, models::GetContactInfoIdentifierParameter>**](getContactInfo_identifier_parameter.md)> | Meta data of product such as description, vendor, producer, stock level. The size of cumulative metaInfo shall not exceed **1000 KB**. Maximum length of metaInfo object can be 20. | [optional]
**update_enabled** | Option<**bool**> | Facilitate to update the existing category in the same request (updateEnabled = true) | [optional][default to false]
**deleted_at** | Option<**String**> | UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ) of the product deleted from the shop's database | [optional]
**is_deleted** | Option<**bool**> | product deleted from the shop's database | [optional]
**stock** | Option<**f64**> | Current stock value of the product from the shop's database | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



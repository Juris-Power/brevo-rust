# GetProductDetails

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **String** | Product ID for which you requested the details | 
**name** | **String** | Name of the product for which you requested the details | 
**created_at** | **String** | Creation UTC date-time of the product (YYYY-MM-DDTHH:mm:ss.SSSZ) | 
**modified_at** | **String** | Last modification UTC date-time of the product (YYYY-MM-DDTHH:mm:ss.SSSZ) | 
**url** | Option<**String**> | URL to the product | [optional]
**image_url** | Option<**String**> | Absolute URL to the cover image of the product | [optional]
**sku** | Option<**String**> | Product identifier from the shop | [optional]
**price** | Option<**f32**> | Price of the product | [optional]
**categories** | Option<**Vec<String>**> | Category ID-s of the product | [optional]
**parent_id** | Option<**String**> | Parent product id of the product | [optional]
**s3_original** | Option<**String**> | S3 url of original image | [optional]
**s3_thumb_analytics** | **String** | S3 thumbnail url of original image in 120x120 dimension for analytics section | 
**s3_thumb_editor** | **String** | S3 thumbnail url of original image in 600x400 dimension for editor section | 
**meta_info** | Option<[**serde_json::Value**](.md)> | Meta data of product such as description, vendor, producer, stock level, etc. | [optional]
**is_deleted** | Option<**bool**> | product deleted from the shop's database | [optional]
**stock** | Option<**f64**> | Current stock value of the product from the shop's database | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# Order

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **String** | Unique ID of the order. | 
**created_at** | **String** | Event occurrence UTC date-time (YYYY-MM-DDTHH:mm:ssZ), when order is actually created. | 
**updated_at** | **String** | Event updated UTC date-time (YYYY-MM-DDTHH:mm:ssZ), when the status of the order is actually changed/updated. | 
**status** | **String** | State of the order. | 
**amount** | **f64** | Total amount of the order, including all shipping expenses, tax and the price of items. | 
**store_id** | Option<**String**> | ID of store where the order is placed | [optional]
**identifiers** | Option<[**models::OrderIdentifiers**](order_identifiers.md)> |  | [optional]
**products** | [**Vec<models::OrderProductsInner>**](order_products_inner.md) |  | 
**billing** | Option<[**models::OrderBilling**](order_billing.md)> |  | [optional]
**coupons** | Option<**Vec<String>**> | Coupons applied to the order. Stored case insensitive. | [optional]
**meta_info** | Option<[**std::collections::HashMap<String, models::OrderMetaInfoValue>**](order_metaInfo_value.md)> | Meta data of order to store additional detal such as custom message, customer type, source. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



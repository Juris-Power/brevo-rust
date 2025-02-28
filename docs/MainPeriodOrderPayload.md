# MainPeriodOrderPayload

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | Option<**f64**> | Total amount of the order | [optional]
**billing** | Option<[**models::MainPeriodBillingPayload**](main.billingPayload.md)> | Billing information for the order | [optional]
**contact_id** | Option<**i64**> | Unique identifier for the contact | [optional]
**coupons** | Option<**Vec<String>**> | List of coupon codes applied to the order | [optional]
**created_at** | Option<**String**> | Timestamp when the order was created | [optional]
**email** | Option<**String**> | Email address associated with the order | [optional]
**id** | Option<**String**> | Unique identifier for the order | [optional]
**identifiers** | Option<[**models::MainPeriodIdentifiersPayload**](main.identifiersPayload.md)> | Additional identifiers for the order | [optional]
**products** | Option<[**Vec<models::MainPeriodProductPayload>**](main.productPayload.md)> | List of products in the order | [optional]
**status** | Option<**String**> | Current status of the order | [optional]
**store_id** | Option<**String**> | Identifier for the store where the order was placed | [optional]
**updated_at** | Option<**String**> | Timestamp when the order was last updated | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



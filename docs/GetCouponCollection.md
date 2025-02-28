# GetCouponCollection

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **String** | The id of the collection. | 
**name** | **String** | The name of the collection. | 
**default_coupon** | **String** | The default coupon of the collection. | 
**created_at** | **String** | Datetime on which the collection was created. | 
**total_coupons** | **i64** | Total number of coupons in the collection. | 
**remaining_coupons** | **i64** | Number of coupons that have not been sent yet. | 
**expiration_date** | Option<**String**> | Expiration date for the coupon collection in RFC3339 format. | [optional]
**remaining_days_alert** | Option<**i32**> | If present, an email notification is going to be sent the defined amount of days before to the expiration date. | [optional]
**remaining_coupons_alert** | Option<**i32**> | If present, an email notification is going to be sent when the total number of available coupons falls below the defined threshold. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



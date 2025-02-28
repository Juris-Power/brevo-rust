# CreatePaymentRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference** | **String** | Reference of the payment request, it will appear on the payment page.  | 
**cart** | [**models::Cart**](cart.md) |  | 
**contact_id** | **i64** | Brevo ID of the contact requested to pay.  | 
**description** | Option<**String**> | description of payment request  | [optional]
**notification** | Option<[**models::Notification**](notification.md)> |  | [optional]
**configuration** | Option<[**models::Configuration**](configuration.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



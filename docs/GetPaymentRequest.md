# GetPaymentRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference** | **String** | Reference of the payment request, it will appear on the payment page.  | 
**status** | **String** | Status of the payment request. | 
**configuration** | Option<[**models::Configuration**](configuration.md)> |  | [optional]
**contact_id** | Option<**i64**> | Brevo ID of the contact requested to pay.  | [optional]
**number_of_reminders_sent** | Option<**i64**> | number of reminders sent.  | [optional]
**cart** | [**models::Cart**](cart.md) |  | 
**notification** | [**models::Notification**](notification.md) |  | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



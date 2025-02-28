# \PaymentsApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_payment_request**](PaymentsApi.md#create_payment_request) | **POST** /payments/requests | Create a payment request
[**delete_payment_request**](PaymentsApi.md#delete_payment_request) | **DELETE** /payments/requests/{id} | Delete a payment request.
[**get_payment_request**](PaymentsApi.md#get_payment_request) | **GET** /payments/requests/{id} | Get payment request details



## create_payment_request

> models::CreatePaymentResponse create_payment_request(create_payment_request)
Create a payment request

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_payment_request** | [**CreatePaymentRequest**](CreatePaymentRequest.md) | Create a payment request  | [required] |

### Return type

[**models::CreatePaymentResponse**](createPaymentResponse.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_payment_request

> delete_payment_request(id)
Delete a payment request.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** | ID of the payment request. | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_payment_request

> models::GetPaymentRequest get_payment_request(id)
Get payment request details

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | Id of the payment Request | [required] |

### Return type

[**models::GetPaymentRequest**](getPaymentRequest.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


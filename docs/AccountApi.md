# \AccountApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_account**](AccountApi.md#get_account) | **GET** /account | Get your account information, plan and credits details
[**get_account_activity**](AccountApi.md#get_account_activity) | **GET** /organization/activities | Get user activity logs



## get_account

> models::GetAccount get_account()
Get your account information, plan and credits details

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::GetAccount**](getAccount.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_account_activity

> models::GetAccountActivity get_account_activity(start_date, end_date, email, limit, offset)
Get user activity logs

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**start_date** | Option<**String**> | Mandatory if endDate is used. Enter start date in UTC date (YYYY-MM-DD) format to filter the activity in your account. Maximum time period that can be selected is one month. Additionally, you can retrieve activity logs from the past 12 months from the date of your search. |  |
**end_date** | Option<**String**> | Mandatory if startDate is used. Enter end date in UTC date (YYYY-MM-DD) format to filter the activity in your account. Maximum time period that can be selected is one month. |  |
**email** | Option<**String**> | Enter the user's email address to filter their activity in the account. |  |
**limit** | Option<**i64**> | Number of documents per page |  |[default to 10]
**offset** | Option<**i64**> | Index of the first document in the page. |  |[default to 0]

### Return type

[**models::GetAccountActivity**](getAccountActivity.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


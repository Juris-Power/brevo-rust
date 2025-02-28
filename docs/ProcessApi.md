# \ProcessApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_process**](ProcessApi.md#get_process) | **GET** /processes/{processId} | Return the informations for a process
[**get_processes**](ProcessApi.md#get_processes) | **GET** /processes | Return all the processes for your account



## get_process

> models::GetProcess get_process(process_id)
Return the informations for a process

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**process_id** | **i64** | Id of the process | [required] |

### Return type

[**models::GetProcess**](getProcess.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_processes

> models::GetProcesses get_processes(limit, offset, sort)
Return all the processes for your account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**limit** | Option<**i64**> | Number limitation for the result returned |  |[default to 10]
**offset** | Option<**i64**> | Beginning point in the list to retrieve from. |  |[default to 0]
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed |  |[default to desc]

### Return type

[**models::GetProcesses**](getProcesses.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


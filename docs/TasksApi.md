# \TasksApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**crm_tasks_get**](TasksApi.md#crm_tasks_get) | **GET** /crm/tasks | Get all tasks
[**crm_tasks_id_delete**](TasksApi.md#crm_tasks_id_delete) | **DELETE** /crm/tasks/{id} | Delete a task
[**crm_tasks_id_get**](TasksApi.md#crm_tasks_id_get) | **GET** /crm/tasks/{id} | Get a task
[**crm_tasks_id_patch**](TasksApi.md#crm_tasks_id_patch) | **PATCH** /crm/tasks/{id} | Update a task
[**crm_tasks_post**](TasksApi.md#crm_tasks_post) | **POST** /crm/tasks | Create a task
[**crm_tasktypes_get**](TasksApi.md#crm_tasktypes_get) | **GET** /crm/tasktypes | Get all task types



## crm_tasks_get

> models::TaskList crm_tasks_get(filter_left_square_bracket_type_right_square_bracket, filter_left_square_bracket_status_right_square_bracket, filter_left_square_bracket_date_right_square_bracket, filter_left_square_bracket_assign_to_right_square_bracket, filter_left_square_bracket_contacts_right_square_bracket, filter_left_square_bracket_deals_right_square_bracket, filter_left_square_bracket_companies_right_square_bracket, date_from, date_to, offset, limit, sort, sort_by)
Get all tasks

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**filter_left_square_bracket_type_right_square_bracket** | Option<**String**> | Filter by task type (ID) |  |
**filter_left_square_bracket_status_right_square_bracket** | Option<**String**> | Filter by task status |  |
**filter_left_square_bracket_date_right_square_bracket** | Option<**String**> | Filter by date |  |
**filter_left_square_bracket_assign_to_right_square_bracket** | Option<**String**> | Filter by the \"assignTo\" ID. You can utilize account emails for the \"assignTo\" attribute. |  |
**filter_left_square_bracket_contacts_right_square_bracket** | Option<**String**> | Filter by contact ids |  |
**filter_left_square_bracket_deals_right_square_bracket** | Option<**String**> | Filter by deals ids |  |
**filter_left_square_bracket_companies_right_square_bracket** | Option<**String**> | Filter by companies ids |  |
**date_from** | Option<**i32**> | dateFrom to date range filter type (timestamp in milliseconds) |  |
**date_to** | Option<**i32**> | dateTo to date range filter type (timestamp in milliseconds) |  |
**offset** | Option<**i64**> | Index of the first document of the page |  |
**limit** | Option<**i64**> | Number of documents per page |  |[default to 50]
**sort** | Option<**String**> | Sort the results in the ascending/descending order. Default order is **descending** by creation if `sort` is not passed |  |
**sort_by** | Option<**String**> | The field used to sort field names. |  |

### Return type

[**models::TaskList**](TaskList.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_tasks_id_delete

> crm_tasks_id_delete(id)
Delete a task

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** |  | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_tasks_id_get

> models::Task crm_tasks_id_get(id)
Get a task

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** |  | [required] |

### Return type

[**models::Task**](Task.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_tasks_id_patch

> crm_tasks_id_patch(id, crm_tasks_id_patch_request)
Update a task

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** |  | [required] |
**crm_tasks_id_patch_request** | [**CrmTasksIdPatchRequest**](CrmTasksIdPatchRequest.md) | Updated task details. | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_tasks_post

> models::CrmTasksPost201Response crm_tasks_post(crm_tasks_post_request)
Create a task

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crm_tasks_post_request** | [**CrmTasksPostRequest**](CrmTasksPostRequest.md) | Task name. | [required] |

### Return type

[**models::CrmTasksPost201Response**](_crm_tasks_post_201_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_tasktypes_get

> models::TaskTypes crm_tasktypes_get()
Get all task types

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::TaskTypes**](TaskTypes.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


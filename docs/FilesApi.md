# \FilesApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**crm_files_get**](FilesApi.md#crm_files_get) | **GET** /crm/files | Get all files
[**crm_files_id_data_get**](FilesApi.md#crm_files_id_data_get) | **GET** /crm/files/{id}/data | Get file details
[**crm_files_id_delete**](FilesApi.md#crm_files_id_delete) | **DELETE** /crm/files/{id} | Delete a file
[**crm_files_id_get**](FilesApi.md#crm_files_id_get) | **GET** /crm/files/{id} | Download a file
[**crm_files_post**](FilesApi.md#crm_files_post) | **POST** /crm/files | Upload a file



## crm_files_get

> Vec<models::FileData> crm_files_get(entity, entity_ids, date_from, date_to, offset, limit, sort)
Get all files

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**entity** | Option<**String**> | Filter by file entity type |  |
**entity_ids** | Option<**String**> | Filter by file entity IDs |  |
**date_from** | Option<**i32**> | dateFrom to date range filter type (timestamp in milliseconds) |  |
**date_to** | Option<**i32**> | dateTo to date range filter type (timestamp in milliseconds) |  |
**offset** | Option<**i64**> | Index of the first document of the page |  |
**limit** | Option<**i64**> | Number of documents per page |  |[default to 50]
**sort** | Option<**String**> | Sort the results in the ascending/descending order. Default order is **descending** by creation if `sort` is not passed |  |

### Return type

[**Vec<models::FileData>**](FileData.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_files_id_data_get

> models::FileData crm_files_id_data_get(id)
Get file details

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | File id to get file data. | [required] |

### Return type

[**models::FileData**](FileData.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_files_id_delete

> crm_files_id_delete(id)
Delete a file

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | File id to delete. | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_files_id_get

> models::FileDownloadableLink crm_files_id_get(id)
Download a file

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | File id to download. | [required] |

### Return type

[**models::FileDownloadableLink**](FileDownloadableLink.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_files_post

> models::FileData crm_files_post(file, deal_id, contact_id, company_id)
Upload a file

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**file** | **std::path::PathBuf** | File data to create a file. | [required] |
**deal_id** | Option<**String**> |  |  |
**contact_id** | Option<**i64**> |  |  |
**company_id** | Option<**String**> |  |  |

### Return type

[**models::FileData**](FileData.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


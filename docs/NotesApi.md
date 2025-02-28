# \NotesApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**crm_notes_get**](NotesApi.md#crm_notes_get) | **GET** /crm/notes | Get all notes
[**crm_notes_id_delete**](NotesApi.md#crm_notes_id_delete) | **DELETE** /crm/notes/{id} | Delete a note
[**crm_notes_id_get**](NotesApi.md#crm_notes_id_get) | **GET** /crm/notes/{id} | Get a note
[**crm_notes_id_patch**](NotesApi.md#crm_notes_id_patch) | **PATCH** /crm/notes/{id} | Update a note
[**crm_notes_post**](NotesApi.md#crm_notes_post) | **POST** /crm/notes | Create a note



## crm_notes_get

> Vec<models::Note> crm_notes_get(entity, entity_ids, date_from, date_to, offset, limit, sort)
Get all notes

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**entity** | Option<**String**> | Filter by note entity type |  |
**entity_ids** | Option<**String**> | Filter by note entity IDs |  |
**date_from** | Option<**i32**> | dateFrom to date range filter type (timestamp in milliseconds) |  |
**date_to** | Option<**i32**> | dateTo to date range filter type (timestamp in milliseconds) |  |
**offset** | Option<**i64**> | Index of the first document of the page |  |
**limit** | Option<**i64**> | Number of documents per page |  |[default to 50]
**sort** | Option<**String**> | Sort the results in the ascending/descending order. Default order is **descending** by creation if `sort` is not passed |  |

### Return type

[**Vec<models::Note>**](Note.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_notes_id_delete

> crm_notes_id_delete(id)
Delete a note

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | Note ID to delete | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_notes_id_get

> models::Note crm_notes_id_get(id)
Get a note

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | Note ID to get | [required] |

### Return type

[**models::Note**](Note.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_notes_id_patch

> crm_notes_id_patch(id, note_data)
Update a note

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | Note ID to update | [required] |
**note_data** | [**NoteData**](NoteData.md) | Note data to update a note. | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_notes_post

> models::NoteId crm_notes_post(note_data)
Create a note

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**note_data** | [**NoteData**](NoteData.md) | Note data to create a note. | [required] |

### Return type

[**models::NoteId**](NoteId.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


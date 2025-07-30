# \CustomObjectsApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getrecords**](CustomObjectsApi.md#getrecords) | **GET** /objects/{object_type}/records | Get the list of object records and total records count for an object.
[**upsertrecords**](CustomObjectsApi.md#upsertrecords) | **POST** /objects/{object_type}/batch/upsert | Create/Update object records in bulk



## getrecords

> models::Getrecords200Response getrecords(object_type, limit, page_num, sort, association)
Get the list of object records and total records count for an object.

This API retrieves a list of object records along with their associated records and provides the total count of records for the specified object.  **Note**: Contact as object type is not supported in this endpoint. 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**object_type** | **String** | object type for the attribute | [required] |
**limit** | **i64** | Number of records returned per page | [required] |
**page_num** | **i64** | Page number for pagination. It's used to fetch the object records on a provided page number. Must be a valid positive integer. | [required] |
**sort** | Option<**String**> | Sort order, must be 'asc' or 'desc'. Default to 'desc' if not provided. |  |[default to desc]
**association** | Option<**String**> | Whether to include associations, must be 'true' or 'false'. Default to 'false' if not provided. |  |

### Return type

[**models::Getrecords200Response**](getrecords_200_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## upsertrecords

> models::Upsertrecords202Response upsertrecords(object_type, upsertrecords_request)
Create/Update object records in bulk

This API allows bulk upsert of object records in a single request. Each object record may include   - Attributes   - Identifiers   - Associations  **Response:**   The API processes the request asynchronously and returns a processId that you can use to track the background process status.  **API and Schema Limitation:**   - Size:       - Max 1000 objects records per request       - Max request body size: 1 MB    - Max 500 attributes defined per object record upsert request     - This is coherent with schema limitation: an object cannot have more than 500 attributes.     - Worth noting: Nothing happens If an attribute is mentioned in the request, but was not previously defined for the object schema (no error, no attribute creation)    - Max 10 associations defined per object record upsert request     - This is coherent with schema limitation: an object cannot have more than 10 associations with other objects. and each object record can be linked to max 10 other records.  **Errors:**     - Make sure both object records exist before associating them, else the API will return an error.     - This route does not create objects. The object where the object records are upserted by this API must be created already else the API will return an error \"invalid object type\". 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**object_type** | **String** | object type for the attribute | [required] |
**upsertrecords_request** | [**UpsertrecordsRequest**](UpsertrecordsRequest.md) | Payload for batch upsert object records with associations | [required] |

### Return type

[**models::Upsertrecords202Response**](upsertrecords_202_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


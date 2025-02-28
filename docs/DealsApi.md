# \DealsApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**crm_attributes_deals_get**](DealsApi.md#crm_attributes_deals_get) | **GET** /crm/attributes/deals | Get deal attributes
[**crm_attributes_post**](DealsApi.md#crm_attributes_post) | **POST** /crm/attributes | Create a company/deal attribute
[**crm_deals_get**](DealsApi.md#crm_deals_get) | **GET** /crm/deals | Get all deals
[**crm_deals_id_delete**](DealsApi.md#crm_deals_id_delete) | **DELETE** /crm/deals/{id} | Delete a deal
[**crm_deals_id_get**](DealsApi.md#crm_deals_id_get) | **GET** /crm/deals/{id} | Get a deal
[**crm_deals_id_patch**](DealsApi.md#crm_deals_id_patch) | **PATCH** /crm/deals/{id} | Update a deal
[**crm_deals_import_post**](DealsApi.md#crm_deals_import_post) | **POST** /crm/deals/import | Import deals(creation and updation)
[**crm_deals_link_unlink_id_patch**](DealsApi.md#crm_deals_link_unlink_id_patch) | **PATCH** /crm/deals/link-unlink/{id} | Link and Unlink a deal with contacts and companies
[**crm_deals_post**](DealsApi.md#crm_deals_post) | **POST** /crm/deals | Create a deal
[**crm_pipeline_details_all_get**](DealsApi.md#crm_pipeline_details_all_get) | **GET** /crm/pipeline/details/all | Get all pipelines
[**crm_pipeline_details_get**](DealsApi.md#crm_pipeline_details_get) | **GET** /crm/pipeline/details | Get pipeline stages
[**crm_pipeline_details_pipeline_id_get**](DealsApi.md#crm_pipeline_details_pipeline_id_get) | **GET** /crm/pipeline/details/{pipelineID} | Get a pipeline



## crm_attributes_deals_get

> Vec<models::DealAttributesInner> crm_attributes_deals_get()
Get deal attributes

### Parameters

This endpoint does not need any parameter.

### Return type

[**Vec<models::DealAttributesInner>**](DealAttributes_inner.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_attributes_post

> models::CrmAttributesPost200Response crm_attributes_post(crm_attributes_post_request)
Create a company/deal attribute

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crm_attributes_post_request** | [**CrmAttributesPostRequest**](CrmAttributesPostRequest.md) | Attribute creation data for a company/deal. | [required] |

### Return type

[**models::CrmAttributesPost200Response**](_crm_attributes_post_200_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_deals_get

> models::DealsList crm_deals_get(filters_left_square_bracket_attributes_period_deal_name_right_square_bracket, filters_left_square_bracket_linked_companies_ids_right_square_bracket, filters_left_square_bracket_linked_contacts_ids_right_square_bracket, modified_since, created_since, offset, limit, sort)
Get all deals

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**filters_left_square_bracket_attributes_period_deal_name_right_square_bracket** | Option<**String**> | Filter by attributes. If you have a filter for the owner on your end, please send it as filters[attributes.deal_owner] and utilize the account email for the filtering. |  |
**filters_left_square_bracket_linked_companies_ids_right_square_bracket** | Option<**String**> | Filter by linked companies ids |  |
**filters_left_square_bracket_linked_contacts_ids_right_square_bracket** | Option<**String**> | Filter by linked companies ids |  |
**modified_since** | Option<**String**> | Filter (urlencoded) the contacts modified after a given UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ). Prefer to pass your timezone in date-time format for accurate result. |  |
**created_since** | Option<**String**> | Filter (urlencoded) the contacts created after a given UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ). Prefer to pass your timezone in date-time format for accurate result. |  |
**offset** | Option<**i64**> | Index of the first document of the page |  |
**limit** | Option<**i64**> | Number of documents per page |  |
**sort** | Option<**String**> | Sort the results in the ascending/descending order. Default order is **descending** by creation if `sort` is not passed |  |

### Return type

[**models::DealsList**](DealsList.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_deals_id_delete

> crm_deals_id_delete(id)
Delete a deal

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


## crm_deals_id_get

> models::Deal crm_deals_id_get(id)
Get a deal

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** |  | [required] |

### Return type

[**models::Deal**](Deal.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_deals_id_patch

> crm_deals_id_patch(id, crm_deals_id_patch_request)
Update a deal

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** |  | [required] |
**crm_deals_id_patch_request** | [**CrmDealsIdPatchRequest**](CrmDealsIdPatchRequest.md) | Updated deal details. | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_deals_import_post

> models::CompaniesImportPost200Response crm_deals_import_post(file, mapping)
Import deals(creation and updation)

Import deals from a CSV file with mapping options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**file** | Option<**std::path::PathBuf**> | The CSV file to upload.The file should have the first row as the mapping attribute. Some default attribute names are (a) deal_id [brevo mongoID to update deals] (b) associated_contact (c) associated_company (f) any other attribute with internal name  |  |
**mapping** | Option<[**serde_json::Value**](serde_json::Value.md)> | The mapping options in JSON format. Here is an example of the JSON structure:   ```json {   \\\"link_entities\\\": true, // Determines whether to link related entities during the import process   \\\"unlink_entities\\\": false, // Determines whether to unlink related entities during the import process   \\\"update_existing_records\\\": true, // Determines whether to update based on company ID or treat every row as create   \\\"unset_empty_attributes\\\": false // Determines whether to unset a specific attribute during update if the values input is blank }  ```  |  |

### Return type

[**models::CompaniesImportPost200Response**](_companies_import_post_200_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_deals_link_unlink_id_patch

> crm_deals_link_unlink_id_patch(id, crm_deals_link_unlink_id_patch_request)
Link and Unlink a deal with contacts and companies

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** |  | [required] |
**crm_deals_link_unlink_id_patch_request** | [**CrmDealsLinkUnlinkIdPatchRequest**](CrmDealsLinkUnlinkIdPatchRequest.md) | Linked / Unlinked contacts and companies ids. | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_deals_post

> models::CrmDealsPost201Response crm_deals_post(crm_deals_post_request)
Create a deal

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**crm_deals_post_request** | [**CrmDealsPostRequest**](CrmDealsPostRequest.md) | Deal create data. | [required] |

### Return type

[**models::CrmDealsPost201Response**](_crm_deals_post_201_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_pipeline_details_all_get

> Vec<models::Pipeline> crm_pipeline_details_all_get()
Get all pipelines

### Parameters

This endpoint does not need any parameter.

### Return type

[**Vec<models::Pipeline>**](Pipeline.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_pipeline_details_get

> models::Pipeline crm_pipeline_details_get()
Get pipeline stages

This endpoint is deprecated. Prefer /crm/pipeline/details/{pipelineID} instead.

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::Pipeline**](Pipeline.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_pipeline_details_pipeline_id_get

> Vec<models::Pipeline> crm_pipeline_details_pipeline_id_get(pipeline_id)
Get a pipeline

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**pipeline_id** | **String** |  | [required] |

### Return type

[**Vec<models::Pipeline>**](Pipeline.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


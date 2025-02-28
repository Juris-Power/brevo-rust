# \CompaniesApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**companies_get**](CompaniesApi.md#companies_get) | **GET** /companies | Get all Companies
[**companies_id_delete**](CompaniesApi.md#companies_id_delete) | **DELETE** /companies/{id} | Delete a company
[**companies_id_get**](CompaniesApi.md#companies_id_get) | **GET** /companies/{id} | Get a company
[**companies_id_patch**](CompaniesApi.md#companies_id_patch) | **PATCH** /companies/{id} | Update a company
[**companies_import_post**](CompaniesApi.md#companies_import_post) | **POST** /companies/import | Import companies(creation and updation)
[**companies_link_unlink_id_patch**](CompaniesApi.md#companies_link_unlink_id_patch) | **PATCH** /companies/link-unlink/{id} | Link and Unlink company with contact and deal
[**companies_post**](CompaniesApi.md#companies_post) | **POST** /companies | Create a company
[**crm_attributes_companies_get**](CompaniesApi.md#crm_attributes_companies_get) | **GET** /crm/attributes/companies | Get company attributes
[**crm_attributes_post**](CompaniesApi.md#crm_attributes_post) | **POST** /crm/attributes | Create a company/deal attribute



## companies_get

> models::CompaniesList companies_get(filters, linked_contacts_ids, linked_deals_ids, modified_since, created_since, page, limit, sort, sort_by)
Get all Companies

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**filters** | Option<**String**> | Filter by attrbutes. If you have filter for owner on your side please send it as {\"attributes.owner\":\"6299dcf3874a14eacbc65c46\"} |  |
**linked_contacts_ids** | Option<**i64**> | Filter by linked contacts ids |  |
**linked_deals_ids** | Option<**String**> | Filter by linked Deals ids |  |
**modified_since** | Option<**String**> | Filter (urlencoded) the contacts modified after a given UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ). Prefer to pass your timezone in date-time format for accurate result. |  |
**created_since** | Option<**String**> | Filter (urlencoded) the contacts created after a given UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ). Prefer to pass your timezone in date-time format for accurate result. |  |
**page** | Option<**i64**> | Index of the first document of the page |  |
**limit** | Option<**i64**> | Number of documents per page |  |
**sort** | Option<**String**> | Sort the results in the ascending/descending order. Default order is **descending** by creation if `sort` is not passed |  |
**sort_by** | Option<**String**> | The field used to sort field names. |  |

### Return type

[**models::CompaniesList**](CompaniesList.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## companies_id_delete

> companies_id_delete(id)
Delete a company

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | Company ID to delete | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## companies_id_get

> models::Company companies_id_get(id)
Get a company

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | Get Company Details | [required] |

### Return type

[**models::Company**](Company.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## companies_id_patch

> models::Company companies_id_patch(id, companies_id_patch_request)
Update a company

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** |  | [required] |
**companies_id_patch_request** | [**CompaniesIdPatchRequest**](CompaniesIdPatchRequest.md) | Updated company details. | [required] |

### Return type

[**models::Company**](Company.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## companies_import_post

> models::CompaniesImportPost200Response companies_import_post(file, mapping)
Import companies(creation and updation)

Import companies from a CSV file with mapping options.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**file** | Option<**std::path::PathBuf**> | The CSV file to upload.The file should have the first row as the mapping attribute. Some default attribute names are (a) company_id [brevo mongoID to update deals] (b) associated_contact (c) associated_deal (f) any other attribute with internal name  |  |
**mapping** | Option<[**serde_json::Value**](serde_json::Value.md)> | The mapping options in JSON format. Here is an example of the JSON structure: ```json {   \\\"link_entities\\\": true, // Determines whether to link related entities during the import process   \\\"unlink_entities\\\": false, // Determines whether to unlink related entities during the import process   \\\"update_existing_records\\\": true, // Determines whether to update based on company ID or treat every row as create   \\\"unset_empty_attributes\\\": false // Determines whether to unset a specific attribute during update if the values input is blank } ```  |  |

### Return type

[**models::CompaniesImportPost200Response**](_companies_import_post_200_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## companies_link_unlink_id_patch

> companies_link_unlink_id_patch(id, companies_link_unlink_id_patch_request)
Link and Unlink company with contact and deal

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** |  | [required] |
**companies_link_unlink_id_patch_request** | [**CompaniesLinkUnlinkIdPatchRequest**](CompaniesLinkUnlinkIdPatchRequest.md) | Linked / Unlinked contacts and deals ids. | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## companies_post

> models::CompaniesPost200Response companies_post(companies_post_request)
Create a company

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**companies_post_request** | [**CompaniesPostRequest**](CompaniesPostRequest.md) | Company create data. | [required] |

### Return type

[**models::CompaniesPost200Response**](_companies_post_200_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## crm_attributes_companies_get

> Vec<models::CompanyAttributesInner> crm_attributes_companies_get()
Get company attributes

### Parameters

This endpoint does not need any parameter.

### Return type

[**Vec<models::CompanyAttributesInner>**](CompanyAttributes_inner.md)

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


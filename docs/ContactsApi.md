# \ContactsApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_contact_to_list**](ContactsApi.md#add_contact_to_list) | **POST** /contacts/lists/{listId}/contacts/add | Add existing contacts to a list
[**create_attribute**](ContactsApi.md#create_attribute) | **POST** /contacts/attributes/{attributeCategory}/{attributeName} | Create contact attribute
[**create_contact**](ContactsApi.md#create_contact) | **POST** /contacts | Create a contact
[**create_doi_contact**](ContactsApi.md#create_doi_contact) | **POST** /contacts/doubleOptinConfirmation | Create Contact via DOI (Double-Opt-In) Flow
[**create_folder**](ContactsApi.md#create_folder) | **POST** /contacts/folders | Create a folder
[**create_list**](ContactsApi.md#create_list) | **POST** /contacts/lists | Create a list
[**delete_attribute**](ContactsApi.md#delete_attribute) | **DELETE** /contacts/attributes/{attributeCategory}/{attributeName} | Delete an attribute
[**delete_contact**](ContactsApi.md#delete_contact) | **DELETE** /contacts/{identifier} | Delete a contact
[**delete_folder**](ContactsApi.md#delete_folder) | **DELETE** /contacts/folders/{folderId} | Delete a folder (and all its lists)
[**delete_list**](ContactsApi.md#delete_list) | **DELETE** /contacts/lists/{listId} | Delete a list
[**delete_multi_attribute_options**](ContactsApi.md#delete_multi_attribute_options) | **DELETE** /contacts/attributes/{attributeType}/{multipleChoiceAttribute}/{multipleChoiceAttributeOption} | Delete a multiple-choice attribute option
[**get_attributes**](ContactsApi.md#get_attributes) | **GET** /contacts/attributes | List all attributes
[**get_contact_info**](ContactsApi.md#get_contact_info) | **GET** /contacts/{identifier} | Get a contact's details
[**get_contact_stats**](ContactsApi.md#get_contact_stats) | **GET** /contacts/{identifier}/campaignStats | Get email campaigns' statistics for a contact
[**get_contacts**](ContactsApi.md#get_contacts) | **GET** /contacts | Get all the contacts
[**get_contacts_from_list**](ContactsApi.md#get_contacts_from_list) | **GET** /contacts/lists/{listId}/contacts | Get contacts in a list
[**get_folder**](ContactsApi.md#get_folder) | **GET** /contacts/folders/{folderId} | Returns a folder's details
[**get_folder_lists**](ContactsApi.md#get_folder_lists) | **GET** /contacts/folders/{folderId}/lists | Get lists in a folder
[**get_folders**](ContactsApi.md#get_folders) | **GET** /contacts/folders | Get all folders
[**get_list**](ContactsApi.md#get_list) | **GET** /contacts/lists/{listId} | Get a list's details
[**get_lists**](ContactsApi.md#get_lists) | **GET** /contacts/lists | Get all the lists
[**get_segments**](ContactsApi.md#get_segments) | **GET** /contacts/segments | Get all the segments
[**import_contacts**](ContactsApi.md#import_contacts) | **POST** /contacts/import | Import contacts
[**remove_contact_from_list**](ContactsApi.md#remove_contact_from_list) | **POST** /contacts/lists/{listId}/contacts/remove | Delete a contact from a list
[**request_contact_export**](ContactsApi.md#request_contact_export) | **POST** /contacts/export | Export contacts
[**update_attribute**](ContactsApi.md#update_attribute) | **PUT** /contacts/attributes/{attributeCategory}/{attributeName} | Update contact attribute
[**update_batch_contacts**](ContactsApi.md#update_batch_contacts) | **POST** /contacts/batch | Update multiple contacts
[**update_contact**](ContactsApi.md#update_contact) | **PUT** /contacts/{identifier} | Update a contact
[**update_folder**](ContactsApi.md#update_folder) | **PUT** /contacts/folders/{folderId} | Update a folder
[**update_list**](ContactsApi.md#update_list) | **PUT** /contacts/lists/{listId} | Update a list



## add_contact_to_list

> models::PostContactInfo add_contact_to_list(list_id, add_contact_to_list_request)
Add existing contacts to a list

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**list_id** | **i64** | Id of the list | [required] |
**add_contact_to_list_request** | [**AddContactToListRequest**](AddContactToListRequest.md) | Emails addresses OR IDs OR EXT_ID attributes of the contacts | [required] |

### Return type

[**models::PostContactInfo**](postContactInfo.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_attribute

> create_attribute(attribute_category, attribute_name, create_attribute)
Create contact attribute

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**attribute_category** | **String** | Category of the attribute | [required] |
**attribute_name** | **String** | Name of the attribute | [required] |
**create_attribute** | [**CreateAttribute**](CreateAttribute.md) | Values to create an attribute | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_contact

> models::CreateUpdateContactModel create_contact(create_contact)
Create a contact

Creates new contacts on Brevo. Contacts can be created by passing either - <br><br> 1. email address of the contact (email_id),  <br> 2. phone number of the contact (to be passed as \"SMS\" field in \"attributes\" along with proper country code), For example- {\"SMS\":\"+91xxxxxxxxxx\"} or {\"SMS\":\"0091xxxxxxxxxx\"} <br> 3. ext_id <br>

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_contact** | [**CreateContact**](CreateContact.md) | Values to create a contact | [required] |

### Return type

[**models::CreateUpdateContactModel**](createUpdateContactModel.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_doi_contact

> create_doi_contact(create_doi_contact)
Create Contact via DOI (Double-Opt-In) Flow

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_doi_contact** | [**CreateDoiContact**](CreateDoiContact.md) | Values to create the Double opt-in (DOI) contact | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_folder

> models::CreateModel create_folder(create_folder)
Create a folder

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_folder** | [**CreateUpdateFolder**](CreateUpdateFolder.md) | Name of the folder | [required] |

### Return type

[**models::CreateModel**](createModel.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_list

> models::CreateModel create_list(create_list)
Create a list

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_list** | [**CreateList**](CreateList.md) | Values to create a list | [required] |

### Return type

[**models::CreateModel**](createModel.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_attribute

> delete_attribute(attribute_category, attribute_name)
Delete an attribute

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**attribute_category** | **String** | Category of the attribute | [required] |
**attribute_name** | **String** | Name of the existing attribute | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_contact

> delete_contact(identifier, identifier_type)
Delete a contact

There are 2 ways to delete a contact <br><br> Option 1- https://api.brevo.com/v3/contacts/{identifier} <br><br> Option 2- https://api.brevo.com/v3/contacts/{identifier}?identifierType={} <br> <br> Option 1 only works if identifierType is email_id (for EMAIL) or contact_id (for ID of the contact),where you can directly pass the value of EMAIL and ID of the contact.   <br><br> Option 2 works for all identifierType, use email_id for EMAIL attribute, contact_id for ID of the contact, ext_id for EXT_ID attribute, phone_id for SMS attribute, whatsapp_id for WHATSAPP attribute, landline_number_id for LANDLINE_NUMBER attribute.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**identifier** | [**GetContactInfoIdentifierParameter**](.md) | Email (urlencoded) OR ID of the contact OR EXT_ID attribute (urlencoded) | [required] |
**identifier_type** | Option<**String**> | email_id for Email, contact_id for ID of the contact, ext_id for EXT_ID attribute, phone_id for SMS attribute, whatsapp_id for WHATSAPP attribute, landline_number_id for LANDLINE_NUMBER attribute |  |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_folder

> delete_folder(folder_id)
Delete a folder (and all its lists)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**folder_id** | **i64** | Id of the folder | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_list

> delete_list(list_id)
Delete a list

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**list_id** | **i64** | Id of the list | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_multi_attribute_options

> delete_multi_attribute_options(attribute_type, multiple_choice_attribute, multiple_choice_attribute_option)
Delete a multiple-choice attribute option

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**attribute_type** | **String** | Type of the attribute | [required] |
**multiple_choice_attribute** | **String** | Name of the existing muliple-choice attribute | [required] |
**multiple_choice_attribute_option** | **String** | Name of the existing multiple-choice attribute option that you want to delete | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_attributes

> models::GetAttributes get_attributes()
List all attributes

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::GetAttributes**](getAttributes.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_info

> models::GetExtendedContactDetails get_contact_info(identifier, identifier_type, start_date, end_date)
Get a contact's details

There are 2 ways to get a contact <br><br> Option 1- https://api.brevo.com/v3/contacts/{identifier} <br><br> Option 2- https://api.brevo.com/v3/contacts/{identifier}?identifierType={} <br> <br> Option 1 only works if identifierType is email_id (for EMAIL), phone_id (for SMS) or contact_id (for ID of the contact),where you can directly pass the value of EMAIL, SMS and ID of the contact.   <br><br> Option 2 works for all identifierType, use email_id for EMAIL attribute, phone_id for SMS attribute, contact_id for ID of the contact, ext_id for EXT_ID attribute, whatsapp_id for WHATSAPP attribute, landline_number_id for LANDLINE_NUMBER attribute <br><br>Along with the contact details, this endpoint will show the statistics of contact for the recent 90 days by default. To fetch the earlier statistics, please use Get contact campaign stats ``https://developers.brevo.com/reference/contacts-7#getcontactstats`` endpoint with the appropriate date ranges.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**identifier** | [**GetContactInfoIdentifierParameter**](.md) | Email (urlencoded) OR ID of the contact OR its SMS attribute value OR EXT_ID attribute (urlencoded) | [required] |
**identifier_type** | Option<**String**> | email_id for Email, phone_id for SMS attribute, contact_id for ID of the contact, ext_id for EXT_ID attribute, whatsapp_id for WHATSAPP attribute, landline_number_id for LANDLINE_NUMBER attribute |  |
**start_date** | Option<**String**> | **Mandatory if endDate is used.** Starting date (YYYY-MM-DD) of the statistic events specific to campaigns. Must be lower than equal to endDate  |  |
**end_date** | Option<**String**> | **Mandatory if startDate is used.** Ending date (YYYY-MM-DD) of the statistic events specific to campaigns. Must be greater than equal to startDate.  |  |

### Return type

[**models::GetExtendedContactDetails**](getExtendedContactDetails.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contact_stats

> models::GetContactCampaignStats get_contact_stats(identifier, start_date, end_date)
Get email campaigns' statistics for a contact

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**identifier** | [**GetContactInfoIdentifierParameter**](.md) | Email (urlencoded) OR ID of the contact | [required] |
**start_date** | Option<**String**> | **Mandatory if endDate is used.** Starting date (YYYY-MM-DD) of the statistic events specific to campaigns. Must be lower than equal to endDate  |  |
**end_date** | Option<**String**> | **Mandatory if startDate is used.** Ending date (YYYY-MM-DD) of the statistic events specific to campaigns. Must be greater than equal to startDate. Maximum difference between startDate and endDate should not be greater than 90 days  |  |

### Return type

[**models::GetContactCampaignStats**](getContactCampaignStats.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contacts

> models::GetContacts get_contacts(limit, offset, modified_since, created_since, sort, segment_id, list_ids, filter)
Get all the contacts

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**limit** | Option<**i64**> | Number of documents per page |  |[default to 50]
**offset** | Option<**i64**> | Index of the first document of the page |  |[default to 0]
**modified_since** | Option<**String**> | Filter (urlencoded) the contacts modified after a given UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ). **Prefer to pass your timezone in date-time format for accurate result.**  |  |
**created_since** | Option<**String**> | Filter (urlencoded) the contacts created after a given UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ). **Prefer to pass your timezone in date-time format for accurate result.**  |  |
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed |  |[default to desc]
**segment_id** | Option<**i64**> | Id of the segment. **Either listIds or segmentId can be passed.** |  |
**list_ids** | Option<[**Vec<i64>**](i64.md)> | Ids of the list. **Either listIds or segmentId can be passed.** |  |
**filter** | Option<**String**> | Filter the contacts on the basis of attributes. **Allowed operator: equals. For multiple-choice options, the filter will apply an AND condition between the options. For category attributes, the filter will work with both id and value. (e.g. filter=equals(FIRSTNAME,\"Antoine\"), filter=equals(B1, true), filter=equals(DOB, \"1989-11-23\"), filter=equals(GENDER, \"1\"), filter=equals(GENDER, \"MALE\"), filter=equals(COUNTRY,\"USA, INDIA\")**  |  |

### Return type

[**models::GetContacts**](getContacts.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_contacts_from_list

> models::GetContacts get_contacts_from_list(list_id, modified_since, limit, offset, sort)
Get contacts in a list

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**list_id** | **i64** | Id of the list | [required] |
**modified_since** | Option<**String**> | Filter (urlencoded) the contacts modified after a given UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ). **Prefer to pass your timezone in date-time format for accurate result.**  |  |
**limit** | Option<**i64**> | Number of documents per page |  |[default to 50]
**offset** | Option<**i64**> | Index of the first document of the page |  |[default to 0]
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed |  |[default to desc]

### Return type

[**models::GetContacts**](getContacts.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_folder

> models::GetFolder get_folder(folder_id)
Returns a folder's details

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**folder_id** | **i64** | id of the folder | [required] |

### Return type

[**models::GetFolder**](getFolder.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_folder_lists

> models::GetFolderLists get_folder_lists(folder_id, limit, offset, sort)
Get lists in a folder

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**folder_id** | **i64** | Id of the folder | [required] |
**limit** | Option<**i64**> | Number of documents per page |  |[default to 10]
**offset** | Option<**i64**> | Index of the first document of the page |  |[default to 0]
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed |  |[default to desc]

### Return type

[**models::GetFolderLists**](getFolderLists.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_folders

> models::GetFolders get_folders(limit, offset, sort)
Get all folders

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**limit** | Option<**i64**> | Number of documents per page |  |[default to 10]
**offset** | Option<**i64**> | Index of the first document of the page |  |[default to 0]
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed |  |[default to desc]

### Return type

[**models::GetFolders**](getFolders.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_list

> models::GetExtendedList get_list(list_id, start_date, end_date)
Get a list's details

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**list_id** | **i64** | Id of the list | [required] |
**start_date** | Option<**String**> | **Mandatory if endDate is used**. Ending (urlencoded) UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ) to aggregate the sent email campaigns for a specific list id. **Prefer to pass your timezone in date-time format for accurate result**  |  |
**end_date** | Option<**String**> | **Mandatory if startDate is used**. Ending (urlencoded) UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ) to aggregate the sent email campaigns for a specific list id. **Prefer to pass your timezone in date-time format for accurate result**  |  |

### Return type

[**models::GetExtendedList**](getExtendedList.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_lists

> models::GetLists get_lists(limit, offset, sort)
Get all the lists

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**limit** | Option<**i64**> | Number of documents per page |  |[default to 10]
**offset** | Option<**i64**> | Index of the first document of the page |  |[default to 0]
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed |  |[default to desc]

### Return type

[**models::GetLists**](getLists.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_segments

> models::GetSegments get_segments(limit, offset, sort)
Get all the segments

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**limit** | Option<**i64**> | Number of documents per page |  |[default to 10]
**offset** | Option<**i64**> | Index of the first document of the page |  |[default to 0]
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed |  |[default to desc]

### Return type

[**models::GetSegments**](getSegments.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## import_contacts

> models::CreatedProcessId import_contacts(request_contact_import)
Import contacts

It returns the background process ID which on completion calls the notify URL that you have set in the input.  **Note**: - Any contact attribute that doesn't exist in your account will be ignored at import end. 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**request_contact_import** | [**RequestContactImport**](RequestContactImport.md) | Values to import contacts in Brevo. To know more about the expected format, please have a look at ``https://help.brevo.com/hc/en-us/articles/209499265-Build-contacts-lists-for-your-email-marketing-campaigns`` | [required] |

### Return type

[**models::CreatedProcessId**](createdProcessId.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## remove_contact_from_list

> models::PostContactInfo remove_contact_from_list(list_id, contact_emails)
Delete a contact from a list

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**list_id** | **i64** | Id of the list | [required] |
**contact_emails** | [**RemoveContactFromListRequest**](RemoveContactFromListRequest.md) | Emails adresses OR IDs OR EXT_ID attributes of the contacts OR 'all' true | [required] |

### Return type

[**models::PostContactInfo**](postContactInfo.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## request_contact_export

> models::CreatedProcessId request_contact_export(request_contact_export)
Export contacts

It returns the background process ID which on completion calls the notify URL that you have set in the input. File will be available in csv.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**request_contact_export** | [**RequestContactExport**](RequestContactExport.md) | Values to request a contact export | [required] |

### Return type

[**models::CreatedProcessId**](createdProcessId.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_attribute

> update_attribute(attribute_category, attribute_name, update_attribute)
Update contact attribute

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**attribute_category** | **String** | Category of the attribute | [required] |
**attribute_name** | **String** | Name of the existing attribute | [required] |
**update_attribute** | [**UpdateAttribute**](UpdateAttribute.md) | Values to update an attribute | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_batch_contacts

> update_batch_contacts(update_batch_contacts)
Update multiple contacts

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**update_batch_contacts** | [**UpdateBatchContacts**](UpdateBatchContacts.md) | Values to update multiple contacts | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_contact

> update_contact(identifier, update_contact, identifier_type)
Update a contact

There are 2 ways to update a contact <br><br> Option 1- https://api.brevo.com/v3/contacts/{identifier} <br><br> Option 2- https://api.brevo.com/v3/contacts/{identifier}?identifierType={} <br> <br> Option 1 only works if identifierType is email_id (for EMAIL) or contact_id (for ID of the contact),where you can directly pass the value of EMAIL and ID of the contact.   <br><br> Option 2 works for all identifierType, use email_id for EMAIL attribute, contact_id for ID of the contact, ext_id for EXT_ID attribute, phone_id for SMS attribute, whatsapp_id for WHATSAPP attribute, landline_number_id for LANDLINE attribute

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**identifier** | [**GetContactInfoIdentifierParameter**](.md) | Email (urlencoded) OR ID of the contact OR EXT_ID attribute (urlencoded) OR its SMS attribute value OR its WHATSAPP attribute value OR its LANDLINE attribute value | [required] |
**update_contact** | [**UpdateContact**](UpdateContact.md) | Values to update a contact | [required] |
**identifier_type** | Option<**String**> | email_id for Email, contact_id for ID of the contact, ext_id for EXT_ID attribute, phone_id for SMS attribute, whatsapp_id for WHATSAPP attribute, landline_number_id for LANDLINE attribute |  |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_folder

> update_folder(folder_id, update_folder)
Update a folder

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**folder_id** | **i64** | Id of the folder | [required] |
**update_folder** | [**CreateUpdateFolder**](CreateUpdateFolder.md) | Name of the folder | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_list

> update_list(list_id, update_list)
Update a list

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**list_id** | **i64** | Id of the list | [required] |
**update_list** | [**UpdateList**](UpdateList.md) | Values to update a list | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


# \WhatsAppCampaignsApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_whats_app_campaign**](WhatsAppCampaignsApi.md#create_whats_app_campaign) | **POST** /whatsappCampaigns | Create and Send a WhatsApp campaign
[**create_whats_app_template**](WhatsAppCampaignsApi.md#create_whats_app_template) | **POST** /whatsappCampaigns/template | Create a WhatsApp template
[**delete_whats_app_campaign**](WhatsAppCampaignsApi.md#delete_whats_app_campaign) | **DELETE** /whatsappCampaigns/{campaignId} | Delete a WhatsApp campaign
[**get_whats_app_campaign**](WhatsAppCampaignsApi.md#get_whats_app_campaign) | **GET** /whatsappCampaigns/{campaignId} | Get a WhatsApp campaign
[**get_whats_app_campaigns**](WhatsAppCampaignsApi.md#get_whats_app_campaigns) | **GET** /whatsappCampaigns | Return all your created WhatsApp campaigns
[**get_whats_app_config**](WhatsAppCampaignsApi.md#get_whats_app_config) | **GET** /whatsappCampaigns/config | Get your WhatsApp API account information
[**get_whats_app_templates**](WhatsAppCampaignsApi.md#get_whats_app_templates) | **GET** /whatsappCampaigns/template-list | Return all your created WhatsApp templates
[**send_whats_app_template_approval**](WhatsAppCampaignsApi.md#send_whats_app_template_approval) | **POST** /whatsappCampaigns/template/approval/{templateId} | Send your WhatsApp template for approval
[**update_whats_app_campaign**](WhatsAppCampaignsApi.md#update_whats_app_campaign) | **PUT** /whatsappCampaigns/{campaignId} | Update a WhatsApp campaign



## create_whats_app_campaign

> models::CreateModel create_whats_app_campaign(create_whats_app_campaign)
Create and Send a WhatsApp campaign

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_whats_app_campaign** | [**CreateWhatsAppCampaign**](CreateWhatsAppCampaign.md) | Values to create a WhatsApp Campaign | [required] |

### Return type

[**models::CreateModel**](createModel.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_whats_app_template

> models::CreateModel create_whats_app_template(create_whats_app_template)
Create a WhatsApp template

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_whats_app_template** | [**CreateWhatsAppTemplate**](CreateWhatsAppTemplate.md) | Values to create a WhatsApp template | [required] |

### Return type

[**models::CreateModel**](createModel.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_whats_app_campaign

> delete_whats_app_campaign(campaign_id)
Delete a WhatsApp campaign

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**campaign_id** | **i64** | id of the campaign | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_whats_app_campaign

> models::GetWhatsappCampaignOverview get_whats_app_campaign(campaign_id)
Get a WhatsApp campaign

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**campaign_id** | **i64** | Id of the campaign | [required] |

### Return type

[**models::GetWhatsappCampaignOverview**](getWhatsappCampaignOverview.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_whats_app_campaigns

> models::GetWhatsappCampaigns get_whats_app_campaigns(start_date, end_date, limit, offset, sort)
Return all your created WhatsApp campaigns

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**start_date** | Option<**String**> | **Mandatory if endDate is used**. Starting (urlencoded) UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ) to filter the WhatsApp campaigns created. **Prefer to pass your timezone in date-time format for accurate result**  |  |
**end_date** | Option<**String**> | **Mandatory if startDate is used**. Ending (urlencoded) UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ) to filter the WhatsApp campaigns created. **Prefer to pass your timezone in date-time format for accurate result**  |  |
**limit** | Option<**i64**> | Number of documents per page |  |[default to 50]
**offset** | Option<**i64**> | Index of the first document in the page |  |[default to 0]
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record modification. Default order is **descending** if `sort` is not passed |  |[default to desc]

### Return type

[**models::GetWhatsappCampaigns**](getWhatsappCampaigns.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_whats_app_config

> models::GetWhatsAppConfig get_whats_app_config()
Get your WhatsApp API account information

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::GetWhatsAppConfig**](getWhatsAppConfig.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_whats_app_templates

> models::GetWhatsappTemplates get_whats_app_templates(start_date, end_date, limit, offset, sort, source)
Return all your created WhatsApp templates

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**start_date** | Option<**String**> | **Mandatory if endDate is used**. Starting (urlencoded) UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ) to filter the templates created. **Prefer to pass your timezone in date-time format for accurate result**  |  |
**end_date** | Option<**String**> | **Mandatory if startDate is used**. Ending (urlencoded) UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ) to filter the templates created. **Prefer to pass your timezone in date-time format for accurate result**  |  |
**limit** | Option<**i64**> | Number of documents per page |  |[default to 50]
**offset** | Option<**i64**> | Index of the first document in the page |  |[default to 0]
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record modification. Default order is **descending** if `sort` is not passed |  |[default to desc]
**source** | Option<**String**> | source of the template |  |

### Return type

[**models::GetWhatsappTemplates**](getWhatsappTemplates.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## send_whats_app_template_approval

> send_whats_app_template_approval(template_id)
Send your WhatsApp template for approval

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_id** | **i64** | id of the template | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_whats_app_campaign

> update_whats_app_campaign(campaign_id, update_whats_app_campaign)
Update a WhatsApp campaign

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**campaign_id** | **i64** | id of the campaign | [required] |
**update_whats_app_campaign** | [**UpdateWhatsAppCampaign**](UpdateWhatsAppCampaign.md) | Values to update a WhatsApp Campaign | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


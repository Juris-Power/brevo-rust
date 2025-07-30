# \TransactionalEmailsApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**block_new_domain**](TransactionalEmailsApi.md#block_new_domain) | **POST** /smtp/blockedDomains | Add a new domain to the list of blocked domains
[**create_smtp_template**](TransactionalEmailsApi.md#create_smtp_template) | **POST** /smtp/templates | Create an email template
[**delete_blocked_domain**](TransactionalEmailsApi.md#delete_blocked_domain) | **DELETE** /smtp/blockedDomains/{domain} | Unblock an existing domain from the list of blocked domains
[**delete_hardbounces**](TransactionalEmailsApi.md#delete_hardbounces) | **POST** /smtp/deleteHardbounces | Delete hardbounces
[**delete_scheduled_email_by_id**](TransactionalEmailsApi.md#delete_scheduled_email_by_id) | **DELETE** /smtp/email/{identifier} | Delete scheduled emails by batchId or messageId
[**delete_smtp_template**](TransactionalEmailsApi.md#delete_smtp_template) | **DELETE** /smtp/templates/{templateId} | Delete an inactive email template
[**get_aggregated_smtp_report**](TransactionalEmailsApi.md#get_aggregated_smtp_report) | **GET** /smtp/statistics/aggregatedReport | Get your transactional email activity aggregated over a period of time
[**get_blocked_domains**](TransactionalEmailsApi.md#get_blocked_domains) | **GET** /smtp/blockedDomains | Get the list of blocked domains
[**get_email_event_report**](TransactionalEmailsApi.md#get_email_event_report) | **GET** /smtp/statistics/events | Get all your transactional email activity (unaggregated events)
[**get_scheduled_email_by_id**](TransactionalEmailsApi.md#get_scheduled_email_by_id) | **GET** /smtp/emailStatus/{identifier} | Fetch scheduled emails by batchId or messageId
[**get_smtp_report**](TransactionalEmailsApi.md#get_smtp_report) | **GET** /smtp/statistics/reports | Get your transactional email activity aggregated per day
[**get_smtp_template**](TransactionalEmailsApi.md#get_smtp_template) | **GET** /smtp/templates/{templateId} | Returns the template information
[**get_smtp_templates**](TransactionalEmailsApi.md#get_smtp_templates) | **GET** /smtp/templates | Get the list of email templates
[**get_transac_blocked_contacts**](TransactionalEmailsApi.md#get_transac_blocked_contacts) | **GET** /smtp/blockedContacts | Get the list of blocked or unsubscribed transactional contacts
[**get_transac_email_content**](TransactionalEmailsApi.md#get_transac_email_content) | **GET** /smtp/emails/{uuid} | Get the personalized content of a sent transactional email
[**get_transac_emails_list**](TransactionalEmailsApi.md#get_transac_emails_list) | **GET** /smtp/emails | Get the list of transactional emails on the basis of allowed filters
[**send_test_template**](TransactionalEmailsApi.md#send_test_template) | **POST** /smtp/templates/{templateId}/sendTest | Send a template to your test list
[**send_transac_email**](TransactionalEmailsApi.md#send_transac_email) | **POST** /smtp/email | Send a transactional email
[**smtp_blocked_contacts_email_delete**](TransactionalEmailsApi.md#smtp_blocked_contacts_email_delete) | **DELETE** /smtp/blockedContacts/{email} | Unblock or resubscribe a transactional contact
[**smtp_log_identifier_delete**](TransactionalEmailsApi.md#smtp_log_identifier_delete) | **DELETE** /smtp/log/{identifier} | Delete an SMTP transactional log
[**template_preview**](TransactionalEmailsApi.md#template_preview) | **POST** /smtp/template/preview | Generate the rendered preview of transactional template
[**update_smtp_template**](TransactionalEmailsApi.md#update_smtp_template) | **PUT** /smtp/templates/{templateId} | Update an email template



## block_new_domain

> block_new_domain(block_domain)
Add a new domain to the list of blocked domains

Blocks a new domain in order to avoid messages being sent to the same

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**block_domain** | [**BlockDomain**](BlockDomain.md) | Name of the domain to be blocked | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_smtp_template

> models::CreateModel create_smtp_template(create_smtp_template)
Create an email template

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_smtp_template** | [**CreateSmtpTemplate**](CreateSmtpTemplate.md) | values to update in transactional email template | [required] |

### Return type

[**models::CreateModel**](createModel.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_blocked_domain

> delete_blocked_domain(domain)
Unblock an existing domain from the list of blocked domains

Unblocks an existing domain from the list of blocked domains

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**domain** | **String** | The name of the domain to be deleted | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_hardbounces

> delete_hardbounces(delete_hardbounces)
Delete hardbounces

Delete hardbounces. To use carefully (e.g. in case of temporary ISP failures)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**delete_hardbounces** | Option<[**DeleteHardbounces**](DeleteHardbounces.md)> | values to delete hardbounces |  |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_scheduled_email_by_id

> delete_scheduled_email_by_id(identifier)
Delete scheduled emails by batchId or messageId

Delete scheduled batch of emails by batchId or single scheduled email by messageId

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**identifier** | **String** | The `batchId` of scheduled emails batch (Should be a valid UUIDv4) or the `messageId` of scheduled email. | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_smtp_template

> delete_smtp_template(template_id)
Delete an inactive email template

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


## get_aggregated_smtp_report

> models::GetAggregatedReport get_aggregated_smtp_report(start_date, end_date, days, tag)
Get your transactional email activity aggregated over a period of time

This endpoint will show the aggregated stats for past 90 days by default if `startDate` and `endDate` OR `days` is not passed. The date range can not exceed 90 days

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**start_date** | Option<**String**> | **Mandatory if endDate is used.** Starting date of the report (YYYY-MM-DD). Must be lower than equal to endDate  |  |
**end_date** | Option<**String**> | **Mandatory if startDate is used.** Ending date of the report (YYYY-MM-DD). Must be greater than equal to startDate  |  |
**days** | Option<**i64**> | Number of days in the past including today (positive integer). _Not compatible with 'startDate' and 'endDate'_  |  |
**tag** | Option<**String**> | Tag of the emails |  |

### Return type

[**models::GetAggregatedReport**](getAggregatedReport.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_blocked_domains

> models::GetBlockedDomains get_blocked_domains()
Get the list of blocked domains

Get the list of blocked domains

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::GetBlockedDomains**](getBlockedDomains.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_email_event_report

> models::GetEmailEventReport get_email_event_report(limit, offset, start_date, end_date, days, email, event, tags, message_id, template_id, sort)
Get all your transactional email activity (unaggregated events)

This endpoint will show the aggregated stats for past 30 days by default if `startDate` and `endDate` OR `days` is not passed. The date range can not exceed 90 days

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**limit** | Option<**i64**> | Number limitation for the result returned |  |[default to 2500]
**offset** | Option<**i64**> | Beginning point in the list to retrieve from. |  |[default to 0]
**start_date** | Option<**String**> | **Mandatory if endDate is used.** Starting date of the report (YYYY-MM-DD). Must be lower than equal to endDate  |  |
**end_date** | Option<**String**> | **Mandatory if startDate is used.** Ending date of the report (YYYY-MM-DD). Must be greater than equal to startDate  |  |
**days** | Option<**i64**> | Number of days in the past including today (positive integer). _Not compatible with 'startDate' and 'endDate'_  |  |
**email** | Option<**String**> | Filter the report for a specific email addresses |  |
**event** | Option<**String**> | Filter the report for a specific event type |  |
**tags** | Option<**String**> | Filter the report for tags (serialized and urlencoded array). To pass multiple tags, a format of string separated by commas is used such as **\"one, two, three\"** |  |
**message_id** | Option<**String**> | Filter on a specific message id |  |
**template_id** | Option<**i64**> | Filter on a specific template id |  |
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed |  |[default to desc]

### Return type

[**models::GetEmailEventReport**](getEmailEventReport.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_scheduled_email_by_id

> models::GetScheduledEmailById200Response get_scheduled_email_by_id(identifier, start_date, end_date, sort, status, limit, offset)
Fetch scheduled emails by batchId or messageId

Fetch scheduled batch of emails by batchId or single scheduled email by messageId (Can retrieve data upto 30 days old)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**identifier** | **String** | The `batchId` of scheduled emails batch (Should be a valid UUIDv4) or the `messageId` of scheduled email. | [required] |
**start_date** | Option<**String**> | Mandatory if `endDate` is used. Starting date (YYYY-MM-DD) from which you want to fetch the list. Can be maximum 30 days older tha current date. |  |
**end_date** | Option<**String**> | Mandatory if `startDate` is used. Ending date (YYYY-MM-DD) till which you want to fetch the list. Maximum time period that can be selected is one month. |  |
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed. Not valid when identifier is `messageId`. |  |[default to desc]
**status** | Option<**String**> | Filter the records by `status` of the scheduled email batch or message. Not valid when identifier is `messageId`. |  |
**limit** | Option<**i64**> | Number of documents returned per page. Not valid when identifier is `messageId`. |  |[default to 100]
**offset** | Option<**i64**> | Index of the first document on the page.  Not valid when identifier is `messageId`. |  |[default to 0]

### Return type

[**models::GetScheduledEmailById200Response**](getScheduledEmailById_200_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_smtp_report

> models::GetReports get_smtp_report(limit, offset, start_date, end_date, days, tag, sort)
Get your transactional email activity aggregated per day

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**limit** | Option<**i64**> | Number of documents returned per page |  |[default to 10]
**offset** | Option<**i64**> | Index of the first document on the page |  |[default to 0]
**start_date** | Option<**String**> | **Mandatory if endDate is used.** Starting date of the report (YYYY-MM-DD)  |  |
**end_date** | Option<**String**> | **Mandatory if startDate is used.** Ending date of the report (YYYY-MM-DD)  |  |
**days** | Option<**i64**> | Number of days in the past including today (positive integer). _Not compatible with 'startDate' and 'endDate'_  |  |
**tag** | Option<**String**> | Tag of the emails |  |
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed |  |[default to desc]

### Return type

[**models::GetReports**](getReports.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_smtp_template

> models::GetSmtpTemplateOverview get_smtp_template(template_id)
Returns the template information

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_id** | **i64** | id of the template | [required] |

### Return type

[**models::GetSmtpTemplateOverview**](getSmtpTemplateOverview.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_smtp_templates

> models::GetSmtpTemplates get_smtp_templates(template_status, limit, offset, sort)
Get the list of email templates

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_status** | Option<**bool**> | Filter on the status of the template. Active = true, inactive = false |  |
**limit** | Option<**i64**> | Number of documents returned per page |  |[default to 50]
**offset** | Option<**i64**> | Index of the first document in the page |  |[default to 0]
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed |  |[default to desc]

### Return type

[**models::GetSmtpTemplates**](getSmtpTemplates.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_transac_blocked_contacts

> models::GetTransacBlockedContacts get_transac_blocked_contacts(start_date, end_date, limit, offset, senders, sort)
Get the list of blocked or unsubscribed transactional contacts

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**start_date** | Option<**String**> | **Mandatory if endDate is used.** Starting date (YYYY-MM-DD) from which you want to fetch the blocked or unsubscribed contacts  |  |
**end_date** | Option<**String**> | **Mandatory if startDate is used.** Ending date (YYYY-MM-DD) till which you want to fetch the blocked or unsubscribed contacts  |  |
**limit** | Option<**i64**> | Number of documents returned per page |  |[default to 50]
**offset** | Option<**i64**> | Index of the first document on the page |  |[default to 0]
**senders** | Option<[**Vec<String>**](String.md)> | Comma separated list of emails of the senders from which contacts are blocked or unsubscribed |  |
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed |  |[default to desc]

### Return type

[**models::GetTransacBlockedContacts**](getTransacBlockedContacts.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_transac_email_content

> models::GetTransacEmailContent get_transac_email_content(uuid)
Get the personalized content of a sent transactional email

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**uuid** | **String** | Unique id of the transactional email that has been sent to a particular contact | [required] |

### Return type

[**models::GetTransacEmailContent**](getTransacEmailContent.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_transac_emails_list

> models::GetTransacEmailsList get_transac_emails_list(email, template_id, message_id, start_date, end_date, sort, limit, offset)
Get the list of transactional emails on the basis of allowed filters

This endpoint will show the list of emails for past 30 days by default. To retrieve emails before that time, please pass startDate and endDate in query filters.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**email** | Option<**String**> | **Mandatory if templateId and messageId are not passed in query filters.** Email address to which transactional email has been sent.  |  |
**template_id** | Option<**i64**> | **Mandatory if email and messageId are not passed in query filters.** Id of the template that was used to compose transactional email.  |  |
**message_id** | Option<**String**> | **Mandatory if templateId and email are not passed in query filters.** Message ID of the transactional email sent.  |  |
**start_date** | Option<**String**> | **Mandatory if endDate is used.** Starting date (YYYY-MM-DD) from which you want to fetch the list. **Maximum time period that can be selected is one month**.  |  |
**end_date** | Option<**String**> | **Mandatory if startDate is used.** Ending date (YYYY-MM-DD) till which you want to fetch the list. **Maximum time period that can be selected is one month.**  |  |
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed |  |[default to desc]
**limit** | Option<**i64**> | Number of documents returned per page |  |[default to 500]
**offset** | Option<**i64**> | Index of the first document in the page |  |[default to 0]

### Return type

[**models::GetTransacEmailsList**](getTransacEmailsList.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## send_test_template

> send_test_template(template_id, send_test_email)
Send a template to your test list

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_id** | **i64** | Id of the template | [required] |
**send_test_email** | [**SendTestEmail**](SendTestEmail.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## send_transac_email

> models::CreateSmtpEmail send_transac_email(send_smtp_email)
Send a transactional email

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**send_smtp_email** | [**SendSmtpEmail**](SendSmtpEmail.md) | Values to send a transactional email | [required] |

### Return type

[**models::CreateSmtpEmail**](createSmtpEmail.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## smtp_blocked_contacts_email_delete

> smtp_blocked_contacts_email_delete(email)
Unblock or resubscribe a transactional contact

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**email** | **String** | contact email (urlencoded) to unblock. | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## smtp_log_identifier_delete

> smtp_log_identifier_delete(identifier)
Delete an SMTP transactional log

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**identifier** | **String** | MessageId of the transactional log(s) to delete | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## template_preview

> models::TemplatePreviewModel template_preview(template_preview_request_body)
Generate the rendered preview of transactional template

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_preview_request_body** | Option<[**TemplatePreviewRequestBody**](TemplatePreviewRequestBody.md)> | Values to fetch Template preview | [required] |

### Return type

[**models::TemplatePreviewModel**](templatePreviewModel.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_smtp_template

> update_smtp_template(template_id, update_smtp_template)
Update an email template

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_id** | **i64** | id of the template | [required] |
**update_smtp_template** | [**UpdateSmtpTemplate**](UpdateSmtpTemplate.md) | values to update in transactional email template | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


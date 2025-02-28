# \DomainsApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**authenticate_domain**](DomainsApi.md#authenticate_domain) | **PUT** /senders/domains/{domainName}/authenticate | Authenticate a domain
[**create_domain**](DomainsApi.md#create_domain) | **POST** /senders/domains | Create a new domain
[**delete_domain**](DomainsApi.md#delete_domain) | **DELETE** /senders/domains/{domainName} | Delete a domain
[**get_domain_configuration**](DomainsApi.md#get_domain_configuration) | **GET** /senders/domains/{domainName} | Validate domain configuration
[**get_domains**](DomainsApi.md#get_domains) | **GET** /senders/domains | Get the list of all your domains



## authenticate_domain

> models::AuthenticateDomainModel authenticate_domain(domain_name)
Authenticate a domain

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**domain_name** | **String** | Domain name | [required] |

### Return type

[**models::AuthenticateDomainModel**](authenticateDomainModel.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_domain

> models::CreateDomainModel create_domain(domain)
Create a new domain

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**domain** | Option<[**CreateDomain**](CreateDomain.md)> | domain's name |  |

### Return type

[**models::CreateDomainModel**](createDomainModel.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_domain

> delete_domain(domain_name)
Delete a domain

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**domain_name** | **String** | Domain name | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_domain_configuration

> models::GetDomainConfigurationModel get_domain_configuration(domain_name)
Validate domain configuration

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**domain_name** | **String** | Domain name | [required] |

### Return type

[**models::GetDomainConfigurationModel**](getDomainConfigurationModel.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_domains

> models::GetDomainsList get_domains()
Get the list of all your domains

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::GetDomainsList**](getDomainsList.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


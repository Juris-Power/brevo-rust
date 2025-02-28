# \EcommerceApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_batch_order**](EcommerceApi.md#create_batch_order) | **POST** /orders/status/batch | Create orders in batch
[**create_order**](EcommerceApi.md#create_order) | **POST** /orders/status | Managing the status of the order
[**create_update_batch_category**](EcommerceApi.md#create_update_batch_category) | **POST** /categories/batch | Create categories in batch
[**create_update_batch_products**](EcommerceApi.md#create_update_batch_products) | **POST** /products/batch | Create products in batch
[**create_update_category**](EcommerceApi.md#create_update_category) | **POST** /categories | Create/Update a category
[**create_update_product**](EcommerceApi.md#create_update_product) | **POST** /products | Create/Update a product
[**ecommerce_activate_post**](EcommerceApi.md#ecommerce_activate_post) | **POST** /ecommerce/activate | Activate the eCommerce app
[**ecommerce_attribution_metrics_conversion_source_conversion_source_id_get**](EcommerceApi.md#ecommerce_attribution_metrics_conversion_source_conversion_source_id_get) | **GET** /ecommerce/attribution/metrics/{conversionSource}/{conversionSourceId} | Get detailed attribution metrics for a single Brevo campaign or workflow
[**ecommerce_attribution_metrics_get**](EcommerceApi.md#ecommerce_attribution_metrics_get) | **GET** /ecommerce/attribution/metrics | Get attribution metrics for one or more Brevo campaigns or workflows
[**ecommerce_attribution_products_conversion_source_conversion_source_id_get**](EcommerceApi.md#ecommerce_attribution_products_conversion_source_conversion_source_id_get) | **GET** /ecommerce/attribution/products/{conversionSource}/{conversionSourceId} | Get attributed product sales for a single Brevo campaign or workflow
[**ecommerce_config_display_currency_get**](EcommerceApi.md#ecommerce_config_display_currency_get) | **GET** /ecommerce/config/displayCurrency | Get the ISO 4217 compliant display currency code for your Brevo account
[**get_categories**](EcommerceApi.md#get_categories) | **GET** /categories | Return all your categories
[**get_category_info**](EcommerceApi.md#get_category_info) | **GET** /categories/{id} | Get a category details
[**get_orders**](EcommerceApi.md#get_orders) | **GET** /orders | Get order details
[**get_product_info**](EcommerceApi.md#get_product_info) | **GET** /products/{id} | Get a product's details
[**get_products**](EcommerceApi.md#get_products) | **GET** /products | Return all your products
[**set_config_display_currency**](EcommerceApi.md#set_config_display_currency) | **POST** /ecommerce/config/displayCurrency | Set the ISO 4217 compliant display currency code for your Brevo account



## create_batch_order

> models::CreatedBatchId create_batch_order(order_batch)
Create orders in batch

Create multiple orders at one time instead of one order at a time

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**order_batch** | [**OrderBatch**](OrderBatch.md) |  | [required] |

### Return type

[**models::CreatedBatchId**](createdBatchId.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_order

> create_order(order)
Managing the status of the order

Manages the transactional status of the order

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**order** | [**Order**](Order.md) |  | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_update_batch_category

> models::CreateUpdateBatchCategoryModel create_update_batch_category(create_update_batch_category)
Create categories in batch

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_update_batch_category** | [**CreateUpdateBatchCategory**](CreateUpdateBatchCategory.md) | Values to create a batch of categories | [required] |

### Return type

[**models::CreateUpdateBatchCategoryModel**](createUpdateBatchCategoryModel.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_update_batch_products

> models::CreateUpdateBatchProductsModel create_update_batch_products(create_update_batch_products)
Create products in batch

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_update_batch_products** | [**CreateUpdateBatchProducts**](CreateUpdateBatchProducts.md) | Values to create a batch of products | [required] |

### Return type

[**models::CreateUpdateBatchProductsModel**](createUpdateBatchProductsModel.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_update_category

> models::CreateCategoryModel create_update_category(create_update_category)
Create/Update a category

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_update_category** | [**CreateUpdateCategory**](CreateUpdateCategory.md) | Values to create/update a category | [required] |

### Return type

[**models::CreateCategoryModel**](createCategoryModel.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_update_product

> models::CreateProductModel create_update_product(create_update_product)
Create/Update a product

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_update_product** | [**CreateUpdateProduct**](CreateUpdateProduct.md) | Values to create/update a product | [required] |

### Return type

[**models::CreateProductModel**](createProductModel.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## ecommerce_activate_post

> ecommerce_activate_post()
Activate the eCommerce app

Getting access to Brevo eCommerce.

### Parameters

This endpoint does not need any parameter.

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## ecommerce_attribution_metrics_conversion_source_conversion_source_id_get

> models::EcommerceAttributionMetricsConversionSourceConversionSourceIdGet200Response ecommerce_attribution_metrics_conversion_source_conversion_source_id_get(conversion_source, conversion_source_id)
Get detailed attribution metrics for a single Brevo campaign or workflow

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**conversion_source** | **String** | The Brevo campaign type or workflow type for which data will be retrieved | [required] |
**conversion_source_id** | **String** | The Brevo campaign or automation workflow id for which data will be retrieved | [required] |

### Return type

[**models::EcommerceAttributionMetricsConversionSourceConversionSourceIdGet200Response**](_ecommerce_attribution_metrics__conversionSource___conversionSourceId__get_200_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## ecommerce_attribution_metrics_get

> models::EcommerceAttributionMetricsGet200Response ecommerce_attribution_metrics_get(period_from, period_to, email_campaign_id_left_square_bracket_right_square_bracket, sms_campaign_id_left_square_bracket_right_square_bracket, automation_workflow_email_id_left_square_bracket_right_square_bracket, automation_workflow_sms_id_left_square_bracket_right_square_bracket)
Get attribution metrics for one or more Brevo campaigns or workflows

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**period_from** | Option<**String**> | When getting metrics for a specific period, define the starting datetime in RFC3339 format |  |
**period_to** | Option<**String**> | When getting metrics for a specific period, define the end datetime in RFC3339 format |  |
**email_campaign_id_left_square_bracket_right_square_bracket** | Option<[**Vec<String>**](String.md)> | The email campaign ID(s) to get metrics for |  |
**sms_campaign_id_left_square_bracket_right_square_bracket** | Option<[**Vec<String>**](String.md)> | The SMS campaign ID(s) to get metrics for |  |
**automation_workflow_email_id_left_square_bracket_right_square_bracket** | Option<[**Vec<String>**](String.md)> | The automation workflow ID(s) to get email attribution metrics for |  |
**automation_workflow_sms_id_left_square_bracket_right_square_bracket** | Option<[**Vec<String>**](String.md)> | The automation workflow ID(s) to get SMS attribution metrics for |  |

### Return type

[**models::EcommerceAttributionMetricsGet200Response**](_ecommerce_attribution_metrics_get_200_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## ecommerce_attribution_products_conversion_source_conversion_source_id_get

> models::EcommerceAttributionProductsConversionSourceConversionSourceIdGet200Response ecommerce_attribution_products_conversion_source_conversion_source_id_get(conversion_source, conversion_source_id)
Get attributed product sales for a single Brevo campaign or workflow

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**conversion_source** | **String** | The Brevo campaign or automation workflow type for which data will be retrieved | [required] |
**conversion_source_id** | **String** | The Brevo campaign or automation workflow id for which data will be retrieved | [required] |

### Return type

[**models::EcommerceAttributionProductsConversionSourceConversionSourceIdGet200Response**](_ecommerce_attribution_products__conversionSource___conversionSourceId__get_200_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## ecommerce_config_display_currency_get

> models::EcommerceConfigDisplayCurrencyGet200Response ecommerce_config_display_currency_get()
Get the ISO 4217 compliant display currency code for your Brevo account

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::EcommerceConfigDisplayCurrencyGet200Response**](_ecommerce_config_displayCurrency_get_200_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_categories

> models::GetCategories get_categories(limit, offset, sort, ids, name, modified_since, created_since)
Return all your categories

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**limit** | Option<**i64**> | Number of documents per page |  |[default to 50]
**offset** | Option<**i64**> | Index of the first document in the page |  |[default to 0]
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed |  |[default to desc]
**ids** | Option<[**Vec<String>**](String.md)> | Filter by category ids |  |
**name** | Option<**String**> | Filter by category name |  |
**modified_since** | Option<**String**> | Filter (urlencoded) the categories modified after a given UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ). **Prefer to pass your timezone in date-time format for accurate result.**  |  |
**created_since** | Option<**String**> | Filter (urlencoded) the categories created after a given UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ). **Prefer to pass your timezone in date-time format for accurate result.**  |  |

### Return type

[**models::GetCategories**](getCategories.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_category_info

> models::GetCategoryDetails get_category_info(id)
Get a category details

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | Category ID | [required] |

### Return type

[**models::GetCategoryDetails**](getCategoryDetails.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_orders

> get_orders(limit, offset, sort, modified_since, created_since)
Get order details

Get all the orders

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**limit** | Option<**i64**> | Number of documents per page |  |[default to 50]
**offset** | Option<**i64**> | Index of the first document in the page |  |[default to 0]
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed |  |[default to desc]
**modified_since** | Option<**String**> | Filter (urlencoded) the orders modified after a given UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ). **Prefer to pass your timezone in date-time format for accurate result.**  |  |
**created_since** | Option<**String**> | Filter (urlencoded) the orders created after a given UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ). **Prefer to pass your timezone in date-time format for accurate result.**  |  |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_product_info

> models::GetProductDetails get_product_info(id)
Get a product's details

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | Product ID | [required] |

### Return type

[**models::GetProductDetails**](getProductDetails.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_products

> models::GetProducts get_products(limit, offset, sort, ids, name, price_left_square_bracket_lte_right_square_bracket, price_left_square_bracket_gte_right_square_bracket, price_left_square_bracket_lt_right_square_bracket, price_left_square_bracket_gt_right_square_bracket, price_left_square_bracket_eq_right_square_bracket, price_left_square_bracket_ne_right_square_bracket, categories, modified_since, created_since)
Return all your products

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**limit** | Option<**i64**> | Number of documents per page |  |[default to 50]
**offset** | Option<**i64**> | Index of the first document in the page |  |[default to 0]
**sort** | Option<**String**> | Sort the results in the ascending/descending order of record creation. Default order is **descending** if `sort` is not passed |  |[default to desc]
**ids** | Option<[**Vec<String>**](String.md)> | Filter by product ids |  |
**name** | Option<**String**> | Filter by product name, minimum 3 characters should be present for search |  |
**price_left_square_bracket_lte_right_square_bracket** | Option<**f64**> | Price filter for products less than and equals to particular amount |  |
**price_left_square_bracket_gte_right_square_bracket** | Option<**f64**> | Price filter for products greater than and equals to particular amount |  |
**price_left_square_bracket_lt_right_square_bracket** | Option<**f64**> | Price filter for products less than particular amount |  |
**price_left_square_bracket_gt_right_square_bracket** | Option<**f64**> | Price filter for products greater than particular amount |  |
**price_left_square_bracket_eq_right_square_bracket** | Option<**f64**> | Price filter for products equals to particular amount |  |
**price_left_square_bracket_ne_right_square_bracket** | Option<**f64**> | Price filter for products not equals to particular amount |  |
**categories** | Option<[**Vec<String>**](String.md)> | Filter by product categories |  |
**modified_since** | Option<**String**> | Filter (urlencoded) the orders modified after a given UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ). **Prefer to pass your timezone in date-time format for accurate result.**  |  |
**created_since** | Option<**String**> | Filter (urlencoded) the orders created after a given UTC date-time (YYYY-MM-DDTHH:mm:ss.SSSZ). **Prefer to pass your timezone in date-time format for accurate result.**  |  |

### Return type

[**models::GetProducts**](getProducts.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## set_config_display_currency

> models::EcommerceConfigDisplayCurrencyGet200Response set_config_display_currency(ecommerce_config_display_currency_get200_response)
Set the ISO 4217 compliant display currency code for your Brevo account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**ecommerce_config_display_currency_get200_response** | Option<[**EcommerceConfigDisplayCurrencyGet200Response**](EcommerceConfigDisplayCurrencyGet200Response.md)> | set ISO 4217 compliant display currency code payload |  |

### Return type

[**models::EcommerceConfigDisplayCurrencyGet200Response**](_ecommerce_config_displayCurrency_get_200_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


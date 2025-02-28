# \CouponsApi

All URIs are relative to *https://api.brevo.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_coupon_collection**](CouponsApi.md#create_coupon_collection) | **POST** /couponCollections | Create а coupon collection
[**create_coupons**](CouponsApi.md#create_coupons) | **POST** /coupons | Create coupons for a coupon collection
[**get_coupon_collection**](CouponsApi.md#get_coupon_collection) | **GET** /couponCollections/{id} | Get a coupon collection by id
[**get_coupon_collections**](CouponsApi.md#get_coupon_collections) | **GET** /couponCollections | Get all your coupon collections
[**update_coupon_collection**](CouponsApi.md#update_coupon_collection) | **PATCH** /couponCollections/{id} | Update a coupon collection by id



## create_coupon_collection

> models::CreateCouponCollection201Response create_coupon_collection(create_coupon_collection_request)
Create а coupon collection

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_coupon_collection_request** | [**CreateCouponCollectionRequest**](CreateCouponCollectionRequest.md) | Values to create a coupon collection | [required] |

### Return type

[**models::CreateCouponCollection201Response**](createCouponCollection_201_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_coupons

> create_coupons(create_coupons_request)
Create coupons for a coupon collection

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_coupons_request** | [**CreateCouponsRequest**](CreateCouponsRequest.md) | Values to create coupons | [required] |

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_coupon_collection

> models::GetCouponCollection get_coupon_collection(id)
Get a coupon collection by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | Id of the collection to return | [required] |

### Return type

[**models::GetCouponCollection**](getCouponCollection.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_coupon_collections

> models::GetCouponCollection get_coupon_collections(limit, offset, sort, sort_by)
Get all your coupon collections

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**limit** | Option<**i64**> | Number of documents returned per page |  |[default to 50]
**offset** | Option<**i64**> | Index of the first document on the page |  |[default to 0]
**sort** | Option<**String**> | Sort the results by creation time in ascending/descending order |  |[default to desc]
**sort_by** | Option<**String**> | The field used to sort coupon collections |  |[default to createdAt]

### Return type

[**models::GetCouponCollection**](getCouponCollection.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_coupon_collection

> models::UpdateCouponCollection200Response update_coupon_collection(id, update_coupon_collection_request)
Update a coupon collection by id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | Id of the collection to update | [required] |
**update_coupon_collection_request** | Option<[**UpdateCouponCollectionRequest**](UpdateCouponCollectionRequest.md)> | Values to update the coupon collection |  |

### Return type

[**models::UpdateCouponCollection200Response**](updateCouponCollection_200_response.md)

### Authorization

[api-key](../README.md#api-key)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


# GetAllExternalFeedsFeedsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **String** | ID of the feed | 
**name** | **String** | Name of the feed | 
**url** | **String** | URL of the feed | 
**auth_type** | **String** | Auth type of the feed: * `basic` * `token` * `noAuth`  | 
**username** | Option<**String**> | Username for authType `basic` | [optional]
**password** | Option<**String**> | Password for authType `basic` | [optional]
**token** | Option<**String**> | Token for authType `token` | [optional]
**headers** | [**Vec<models::GetExternalFeedByUuidHeadersInner>**](getExternalFeedByUUID_headers_inner.md) | Custom headers for the feed | 
**max_retries** | **i32** | Maximum number of retries on the feed url | [default to 5]
**cache** | **bool** | Toggle caching of feed url response | 
**created_at** | **String** | Datetime on which the feed was created | 
**modified_at** | **String** | Datetime on which the feed was modified | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



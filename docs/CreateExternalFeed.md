# CreateExternalFeed

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **String** | Name of the feed | 
**url** | **String** | URL of the feed | 
**auth_type** | Option<**String**> | Auth type of the feed:  * `basic`  * `token`  * `noAuth`  | [optional][default to NoAuth]
**username** | Option<**String**> | Username for authType `basic` | [optional]
**password** | Option<**String**> | Password for authType `basic` | [optional]
**token** | Option<**String**> | Token for authType `token` | [optional]
**headers** | Option<[**Vec<models::GetExternalFeedByUuidHeadersInner>**](getExternalFeedByUUID_headers_inner.md)> | Custom headers for the feed | [optional]
**max_retries** | Option<**i32**> | Maximum number of retries on the feed url | [optional][default to 5]
**cache** | Option<**bool**> | Toggle caching of feed url response | [optional][default to false]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CreateBalanceDefinitionPayload

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**balance_availability_duration_modifier** | Option<**String**> | Defines when the balance expires within the selected duration. | [optional]
**balance_availability_duration_unit** | Option<**String**> | Unit of time for balance validity. | [optional]
**balance_availability_duration_value** | Option<**i32**> | Number of time units before the balance expires. | [optional]
**balance_expiration_date** | Option<[**String**](string.md)> | Fixed expiration date (`dd/mm` format) as an alternative to duration-based expiry. | [optional]
**balance_option_amount_overtaking_strategy** | Option<**String**> | Defines whether partial credit is allowed when reaching max balance. | [optional]
**balance_option_credit_rounding** | Option<**String**> | Defines rounding strategy for credit transactions. | [optional]
**balance_option_debit_rounding** | Option<**String**> | Defines rounding strategy for debit transactions. | [optional]
**description** | Option<**String**> | Short description of the balance definition. | [optional]
**image_ref** | Option<**String**> | URL of an optional image reference. | [optional]
**max_amount** | Option<**f64**> | Maximum allowable balance amount. | [optional]
**max_credit_amount_limit** | Option<**f64**> | Maximum credit allowed per operation. | [optional]
**max_debit_amount_limit** | Option<**f64**> | Maximum debit allowed per operation. | [optional]
**meta** | Option<[**serde_json::Value**](.md)> | Additional metadata for the balance definition. | [optional]
**min_amount** | Option<**f64**> | Minimum allowable balance amount. | [optional]
**name** | **String** | Name of the balance definition. | 
**unit** | **String** | Unit of balance measurement. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



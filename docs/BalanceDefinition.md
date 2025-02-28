# BalanceDefinition

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**balance_availability_duration_modifier** | Option<**String**> | startOfPeriod depicts the balancy expiry on start of day/week/month/year. endOfPeriod depicts the balancy expiry on end of day/week/month/year | [optional]
**balance_availability_duration_unit** | Option<**String**> | Unit of time for the balance's availability (e.g., day/week/month/year). | [optional]
**balance_availability_duration_value** | Option<**i32**> | Number of days/weeks/month/year for balance expiry | [optional]
**balance_expiration_date** | Option<**String**> | Date when the balance expires and can no longer be used, in dd/mm format. The balance will be expired when this date appears next in the calendar and only one of balanceExpirationDate or balance availability fields can be used. | [optional]
**balance_option_amount_overtaking_strategy** | Option<**String**> | Partial enables partial credit of balance if maximum balance limit is reaching. Strict enables rejection of transaction if it will breach the max credit amount limit. | [optional]
**balance_option_credit_rounding** | Option<**String**> | Rounding strategy for credit transactions. | [optional]
**balance_option_debit_rounding** | Option<**String**> | Rounding strategy for debit transactions. | [optional]
**created_at** | Option<**String**> | Timestamp of balance definition creation. | [optional]
**deleted_at** | Option<**String**> | Timestamp of balance definition deletion (nullable). | [optional]
**description** | Option<**String**> | Short description of the balance definition. | [optional]
**id** | Option<**String**> | Unique identifier for the balance definition. | [optional]
**image_ref** | Option<**String**> | Optional image reference URL. | [optional]
**max_amount** | Option<**f64**> | Maximum allowable balance. | [optional]
**max_credit_amount_limit** | Option<**f64**> | Max credit allowed per operation. | [optional]
**max_debit_amount_limit** | Option<**f64**> | Max debit allowed per operation. | [optional]
**meta** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> | Additional metadata for the balance definition. | [optional]
**min_amount** | Option<**f64**> | Minimum allowable balance. | [optional]
**name** | Option<**String**> | Name of the balance definition. | [optional]
**unit** | Option<**String**> | Unit of balance (e.g., points, currency). | [optional]
**updated_at** | Option<**String**> | Timestamp of the last update. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



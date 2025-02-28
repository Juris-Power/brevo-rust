# MainPeriodRule

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**condition** | Option<[**models::MainPeriodRuleConditionResponse**](main.ruleConditionResponse.md)> | Selected rule condition | [optional]
**created_at** | Option<**String**> | Timestamp when the rule was created | [optional]
**description** | Option<**String**> | Description of the rule | [optional]
**event** | Option<[**models::MainPeriodRuleEventResponse**](main.ruleEventResponse.md)> | Selected event in the rule | [optional]
**is_internal** | Option<**bool**> | Metric to identify if it's an internal rule or not | [optional]
**loyalty_program_id** | Option<**String**> | Loyalty Program id to which current rule is associated | [optional]
**loyalty_version_id** | Option<**i32**> | Loyalty Version id to which current rule is associated | [optional]
**meta** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> | Additional data to define the rule | [optional]
**name** | Option<**String**> | Rule name | [optional]
**results** | Option<[**Vec<models::MainPeriodRuleResultResponse>**](main.ruleResultResponse.md)> | Results of the rule definition | [optional]
**rule_id** | Option<**String**> | Unique identifier for the rule | [optional]
**rule_type** | Option<**String**> | Type of the rule | [optional]
**updated_at** | Option<**String**> | Timestamp when the rule was updated | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



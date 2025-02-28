# MainPeriodReward

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**attribution_per_consumer** | Option<**i32**> | Maximum number of times a consumer can be attributed this reward | [optional]
**balance_definition_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Unique identifier for the balance definition | [optional]
**code** | Option<**String**> | Unique code for the reward | [optional]
**code_count** | Option<**i64**> | Total number of codes generated | [optional]
**code_generator_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Unique identifier for the code generator | [optional]
**code_pool_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Unique identifier for the code pool | [optional]
**config** | Option<**String**> | Configuration settings for the reward | [optional]
**created_at** | Option<**String**> | Timestamp when the reward was created | [optional]
**disabled_at** | Option<**String**> | Disabled date of the reward | [optional]
**end_date** | Option<**String**> | End date of the reward validity | [optional]
**expiration_date** | Option<**String**> | Expiration date of the reward | [optional]
**expiration_modifier** | Option<**String**> | Select startOfPeriod to configure rewards expiry on start of day/week/month/year. Select endOfPeriod to configure reward expiry on end of day/week/month/year, else select noModification | [optional][default to NoModification]
**expiration_unit** | Option<**String**> | Unit of time for the rewards's availability (e.g., day/week/month/year). | [optional]
**expiration_value** | Option<**i32**> | Number of days/weeks/month/year for reward expiry | [optional]
**generator** | Option<[**models::MainPeriodGenerator**](main.generator.md)> | object | [optional]
**id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Unique identifier for the reward | [optional]
**limits** | Option<[**Vec<models::MainPeriodLimit>**](main.limit.md)> | Attribution / Redeem Limits for the reward | [optional]
**loyalty_program_id** | Option<[**uuid::Uuid**](uuid::Uuid.md)> | Id of the loyalty program to which the current reward belongs to | [optional]
**meta** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> | Additional data for reward definition | [optional]
**name** | Option<**String**> | Name of the reward | [optional]
**products** | Option<[**Vec<models::MainPeriodProduct>**](main.product.md)> | Selected products for reward definition | [optional]
**public_description** | Option<**String**> | Public description for the reward | [optional]
**public_image** | Option<**String**> | Public Image for the reward | [optional]
**public_name** | Option<**String**> | Public name for the reward | [optional]
**redeem_per_consumer** | Option<**i32**> | Defines the redeem limit for the consumer | [optional]
**redeem_rules** | Option<**Vec<String>**> | Rules defined to redeem a reward | [optional]
**reward_configs** | Option<[**models::MainPeriodRewardConfigurations**](main.rewardConfigurations.md)> | object | [optional]
**rule** | Option<[**models::MainPeriodRule**](main.rule.md)> | Rule to define the reward | [optional]
**start_date** | Option<**String**> | Start date of attribution of the reward | [optional]
**subtract_balance_definition_id** | Option<**String**> | Id of the selected balance while redeeming / attributing a reward | [optional]
**subtract_balance_strategy** | Option<**String**> | Strategy of the Balance while redeeming / attributing a reward | [optional]
**subtract_balance_value** | Option<**i32**> | Amount of balance to be selected while redeeming / attributing a reward | [optional]
**subtract_total_balance** | Option<**bool**> | Value to indicate to subtract full balance or not | [optional]
**total_attribution** | Option<**i32**> | Defines the limit to which a consumer can attribute a reward | [optional]
**total_redeem** | Option<**i32**> | Defines the limit to which a consumer can redeem a reward | [optional]
**trigger_id** | Option<**String**> | Id of the Rule to be updated for that reward | [optional]
**unit** | Option<**String**> | Selected unit of the balance | [optional]
**updated_at** | Option<**String**> | Timestamp for when this reward was last updated. | [optional]
**value** | Option<**f64**> | Value of metric in selected config for reward definition | [optional]
**value_type** | Option<**String**> | Type of config selected for reward definition | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



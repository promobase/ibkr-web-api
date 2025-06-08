# AlertResponseConditionsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**condition_type** | **int** | Types: 1-Price, 3-Time, 4-Margin, 5-Trade, 6-Volume, 7: MTA market 8: MTA Position, 9: MTA Acc. Daily PN&amp;  | [optional] 
**conidex** | **str** | conid and exchange. Format supports conid or conid@exchange | [optional] 
**contract_description_1** | **str** | Format contract name | [optional] 
**condition_operator** | **str** | optional, operator for the current condition   * &gt;&#x3D; Greater than or equal to   * &lt;&#x3D; Less than or equal to  | [optional] 
**condition_trigger_method** | **str** | optional, only some type of conditions have triggerMethod | [optional] 
**condition_value** | **str** | can not be empty, can pass default value \&quot;*\&quot; | [optional] 
**condition_logic_bind** | **str** | Condition array should end with \&quot;n\&quot;   * a - AND   * o - OR   * n - END  | [optional] 
**condition_time_zone** | **str** | only needed for some MTA alert condition | [optional] 

## Example

```python
from ibkr_web_api.models.alert_response_conditions_inner import AlertResponseConditionsInner

# TODO update the JSON string below
json = "{}"
# create an instance of AlertResponseConditionsInner from a JSON string
alert_response_conditions_inner_instance = AlertResponseConditionsInner.from_json(json)
# print the JSON string representation of the object
print(AlertResponseConditionsInner.to_json())

# convert the object into a dict
alert_response_conditions_inner_dict = alert_response_conditions_inner_instance.to_dict()
# create an instance of AlertResponseConditionsInner from a dict
alert_response_conditions_inner_from_dict = AlertResponseConditionsInner.from_dict(alert_response_conditions_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



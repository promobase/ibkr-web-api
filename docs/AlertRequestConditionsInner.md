# AlertRequestConditionsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **int** | Types: 1-Price, 3-Time, 4-Margin, 5-Trade, 6-Volume, 7: MTA market 8: MTA Position, 9: MTA Acc. Daily PN&amp;  | [optional] 
**conidex** | **str** | conid and exchange. Format supports conid or conid@exchange | [optional] 
**operator** | **str** | optional, operator for the current condition, can be &gt;&#x3D; or &lt;&#x3D; | [optional] 
**trigger_method** | **str** | optional, only some type of conditions have triggerMethod | [optional] 
**value** | **str** | can not be empty, can pass default value \&quot;*\&quot; | [optional] 
**logic_bind** | **str** | \&quot;a\&quot; means \&quot;AND\&quot;, \&quot;o\&quot; means \&quot;OR\&quot;, \&quot;n\&quot; means \&quot;END\&quot;, the last one condition in the condition array should \&quot;n\&quot;  | [optional] 
**time_zone** | **str** | only needed for some MTA alert condition | [optional] 

## Example

```python
from openapi_client.models.alert_request_conditions_inner import AlertRequestConditionsInner

# TODO update the JSON string below
json = "{}"
# create an instance of AlertRequestConditionsInner from a JSON string
alert_request_conditions_inner_instance = AlertRequestConditionsInner.from_json(json)
# print the JSON string representation of the object
print(AlertRequestConditionsInner.to_json())

# convert the object into a dict
alert_request_conditions_inner_dict = alert_request_conditions_inner_instance.to_dict()
# create an instance of AlertRequestConditionsInner from a dict
alert_request_conditions_inner_from_dict = AlertRequestConditionsInner.from_dict(alert_request_conditions_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AlertResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account** | **str** | account id | [optional] 
**order_id** | **int** |  | [optional] 
**alert_name** | **str** | name of alert | [optional] 
**alert_message** | **str** | The message you want to receive via email or text message | [optional] 
**alert_active** | **int** | whether alert is active or not, so value can only be 0 or 1 | [optional] 
**alert_repeatable** | **int** | whether alert is repeatable or not, so value can only be 0 or 1 | [optional] 
**alert_email** | **str** | email address to receive alert | [optional] 
**alert_send_message** | **int** | whether allowing to send email or not, so value can only be 0 or 1,  | [optional] 
**tif** | **str** | time in force, can only be GTC or GTD | [optional] 
**expire_time** | **str** | format, YYYYMMDD-HH:mm:ss  | [optional] 
**order_status** | **str** | status of alert | [optional] 
**outside_rth** | **int** | value can only be 0 or 1, set to 1 if the alert can be triggered outside regular trading hours.  | [optional] 
**itws_orders_only** | **int** | value can only be 0 or 1, set to 1 to enable the alert only in IBKR mobile  | [optional] 
**alert_show_popup** | **int** | value can only be 0 or 1, set to 1 to allow to show alert in pop-ups | [optional] 
**alert_triggered** | **bool** | whether the alert has been triggered | [optional] 
**order_not_editable** | **bool** | whether the alert can be edited | [optional] 
**tool_id** | **int** | for MTA alert only, each user has a unique toolId and it will stay the same, do not send for normal alert  | [optional] 
**alert_play_audio** | **str** | audio message to play when alert is triggered | [optional] 
**alert_mta_currency** | **str** | MTA alert only | [optional] 
**alert_mta_defaults** | **str** | MTA alert only | [optional] 
**time_zone** | **str** | MTA alert only | [optional] 
**alert_default_type** | **str** | MTA alert only | [optional] 
**condition_size** | **int** | size of conditions array | [optional] 
**condition_outside_rth** | **int** | whether allowing the condition can be triggered outside of regular trading hours, 1 means allow | [optional] 
**conditions** | [**List[AlertResponseConditionsInner]**](AlertResponseConditionsInner.md) |  | [optional] 

## Example

```python
from ibkr_web_api.models.alert_response import AlertResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AlertResponse from a JSON string
alert_response_instance = AlertResponse.from_json(json)
# print the JSON string representation of the object
print(AlertResponse.to_json())

# convert the object into a dict
alert_response_dict = alert_response_instance.to_dict()
# create an instance of AlertResponse from a dict
alert_response_from_dict = AlertResponse.from_dict(alert_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



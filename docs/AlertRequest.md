# AlertRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**order_id** | **int** | orderId is required when modifying alert. You can get it from /iserver/account/:accountId/alerts  | [optional] 
**alert_name** | **str** | name of alert | [optional] 
**alert_message** | **str** | The message you want to receive via email or text message | [optional] 
**alert_repeatable** | **int** | whether alert is repeatable or not, so value can only be 0 or 1, this has to be 1 for MTA alert | [optional] 
**email** | **str** | email address to receive alert | [optional] 
**send_message** | **int** | whether allowing to send email or not, so value can only be 0 or 1,  | [optional] 
**tif** | **str** | time in force, can only be GTC or GTD | [optional] 
**expire_time** | **str** | format, YYYYMMDD-HH:mm:ss, please NOTE this will only work when tif is GTD  | [optional] 
**outside_rth** | **int** | value can only be 0 or 1, set to 1 if the alert can be triggered outside regular trading hours.  | [optional] 
**i_tws_orders_only** | **int** | value can only be 0 or 1, set to 1 to enable the alert only in IBKR mobile  | [optional] 
**show_popup** | **int** | value can only be 0 or 1, set to 1 to allow to show alert in pop-ups | [optional] 
**tool_id** | **int** | for MTA alert only, each user has a unique toolId and it will stay the same, do not send for normal alert  | [optional] 
**play_audio** | **str** | audio message to play when alert is triggered | [optional] 
**conditions** | [**List[AlertRequestConditionsInner]**](AlertRequestConditionsInner.md) |  | [optional] 

## Example

```python
from ibkr-web-api.models.alert_request import AlertRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AlertRequest from a JSON string
alert_request_instance = AlertRequest.from_json(json)
# print the JSON string representation of the object
print(AlertRequest.to_json())

# convert the object into a dict
alert_request_dict = alert_request_instance.to_dict()
# create an instance of AlertRequest from a dict
alert_request_from_dict = AlertRequest.from_dict(alert_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



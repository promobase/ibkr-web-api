# IserverAccountAccountIdAlertsGet200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**order_id** | **int** |  | [optional] 
**account** | **str** | account id | [optional] 
**alert_name** | **str** |  | [optional] 
**alert_active** | **int** | Value can only be 0 or 1, 1 means active | [optional] 
**order_time** | **str** | format, YYYYMMDD-HH:mm:ss, the time when you created the alert  | [optional] 
**alert_triggered** | **bool** | whether the alert has been triggered or not | [optional] 
**alert_repeatable** | **int** | whether the alert can be repeatable or not, value can be 1 or 0. 1 means true | [optional] 

## Example

```python
from ibkr_web_api.models.iserver_account_account_id_alerts_get200_response_inner import IserverAccountAccountIdAlertsGet200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of IserverAccountAccountIdAlertsGet200ResponseInner from a JSON string
iserver_account_account_id_alerts_get200_response_inner_instance = IserverAccountAccountIdAlertsGet200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(IserverAccountAccountIdAlertsGet200ResponseInner.to_json())

# convert the object into a dict
iserver_account_account_id_alerts_get200_response_inner_dict = iserver_account_account_id_alerts_get200_response_inner_instance.to_dict()
# create an instance of IserverAccountAccountIdAlertsGet200ResponseInner from a dict
iserver_account_account_id_alerts_get200_response_inner_from_dict = IserverAccountAccountIdAlertsGet200ResponseInner.from_dict(iserver_account_account_id_alerts_get200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



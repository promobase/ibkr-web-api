# IserverAccountAccountIdAlertPost200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**request_id** | **int** |  | [optional] 
**order_id** | **int** |  | [optional] 
**success** | **bool** |  | [optional] 
**text** | **str** |  | [optional] 
**order_status** | **str** |  | [optional] 
**warning_message** | **str** |  | [optional] 

## Example

```python
from ibkr-web-api.models.iserver_account_account_id_alert_post200_response import IserverAccountAccountIdAlertPost200Response

# TODO update the JSON string below
json = "{}"
# create an instance of IserverAccountAccountIdAlertPost200Response from a JSON string
iserver_account_account_id_alert_post200_response_instance = IserverAccountAccountIdAlertPost200Response.from_json(json)
# print the JSON string representation of the object
print(IserverAccountAccountIdAlertPost200Response.to_json())

# convert the object into a dict
iserver_account_account_id_alert_post200_response_dict = iserver_account_account_id_alert_post200_response_instance.to_dict()
# create an instance of IserverAccountAccountIdAlertPost200Response from a dict
iserver_account_account_id_alert_post200_response_from_dict = IserverAccountAccountIdAlertPost200Response.from_dict(iserver_account_account_id_alert_post200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# IserverAccountAccountIdAlertActivatePostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**alert_id** | **int** | alert id(order id) | [optional] 
**alert_active** | **int** | 1 to activate, 0 to deactivate | [optional] 

## Example

```python
from openapi_client.models.iserver_account_account_id_alert_activate_post_request import IserverAccountAccountIdAlertActivatePostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IserverAccountAccountIdAlertActivatePostRequest from a JSON string
iserver_account_account_id_alert_activate_post_request_instance = IserverAccountAccountIdAlertActivatePostRequest.from_json(json)
# print the JSON string representation of the object
print(IserverAccountAccountIdAlertActivatePostRequest.to_json())

# convert the object into a dict
iserver_account_account_id_alert_activate_post_request_dict = iserver_account_account_id_alert_activate_post_request_instance.to_dict()
# create an instance of IserverAccountAccountIdAlertActivatePostRequest from a dict
iserver_account_account_id_alert_activate_post_request_from_dict = IserverAccountAccountIdAlertActivatePostRequest.from_dict(iserver_account_account_id_alert_activate_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



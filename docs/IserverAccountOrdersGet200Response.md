# IserverAccountOrdersGet200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**filters** | **List[str]** |  | [optional] 
**orders** | [**List[IserverAccountOrdersGet200ResponseOrdersInner]**](IserverAccountOrdersGet200ResponseOrdersInner.md) |  | [optional] 
**snapshot** | **bool** | If live order update is a snapshot | [optional] 

## Example

```python
from openapi_client.models.iserver_account_orders_get200_response import IserverAccountOrdersGet200Response

# TODO update the JSON string below
json = "{}"
# create an instance of IserverAccountOrdersGet200Response from a JSON string
iserver_account_orders_get200_response_instance = IserverAccountOrdersGet200Response.from_json(json)
# print the JSON string representation of the object
print(IserverAccountOrdersGet200Response.to_json())

# convert the object into a dict
iserver_account_orders_get200_response_dict = iserver_account_orders_get200_response_instance.to_dict()
# create an instance of IserverAccountOrdersGet200Response from a dict
iserver_account_orders_get200_response_from_dict = IserverAccountOrdersGet200Response.from_dict(iserver_account_orders_get200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



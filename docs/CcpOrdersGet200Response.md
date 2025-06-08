# CcpOrdersGet200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**orders** | [**List[OrderData]**](OrderData.md) |  | [optional] 

## Example

```python
from ibkr-web-api.models.ccp_orders_get200_response import CcpOrdersGet200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CcpOrdersGet200Response from a JSON string
ccp_orders_get200_response_instance = CcpOrdersGet200Response.from_json(json)
# print the JSON string representation of the object
print(CcpOrdersGet200Response.to_json())

# convert the object into a dict
ccp_orders_get200_response_dict = ccp_orders_get200_response_instance.to_dict()
# create an instance of CcpOrdersGet200Response from a dict
ccp_orders_get200_response_from_dict = CcpOrdersGet200Response.from_dict(ccp_orders_get200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



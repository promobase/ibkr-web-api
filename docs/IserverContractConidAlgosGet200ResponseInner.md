# IserverContractConidAlgosGet200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**id** | **str** |  | [optional] 
**parameters** | [**List[IserverContractConidAlgosGet200ResponseInnerParametersInner]**](IserverContractConidAlgosGet200ResponseInnerParametersInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.iserver_contract_conid_algos_get200_response_inner import IserverContractConidAlgosGet200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of IserverContractConidAlgosGet200ResponseInner from a JSON string
iserver_contract_conid_algos_get200_response_inner_instance = IserverContractConidAlgosGet200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(IserverContractConidAlgosGet200ResponseInner.to_json())

# convert the object into a dict
iserver_contract_conid_algos_get200_response_inner_dict = iserver_contract_conid_algos_get200_response_inner_instance.to_dict()
# create an instance of IserverContractConidAlgosGet200ResponseInner from a dict
iserver_contract_conid_algos_get200_response_inner_from_dict = IserverContractConidAlgosGet200ResponseInner.from_dict(iserver_contract_conid_algos_get200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



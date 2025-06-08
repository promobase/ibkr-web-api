# Contract

Contains all details of the contract, including rules you can use when placing orders

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**r_t_h** | **bool** | true means you can trade outside RTH(regular trading hours) | [optional] 
**con_id** | **str** | same as that in request | [optional] 
**company_name** | **str** | Contracts company name | [optional] 
**exchange** | **str** |  | [optional] 
**local_symbol** | **str** | for exmple FB | [optional] 
**instrument_type** | **str** | for example STK | [optional] 
**currency** | **str** |  | [optional] 
**company_name** | **str** |  | [optional] 
**category** | **str** |  | [optional] 
**industry** | **str** |  | [optional] 
**rules** | [**ContractRules**](ContractRules.md) |  | [optional] 

## Example

```python
from ibkr-web-api.models.contract import Contract

# TODO update the JSON string below
json = "{}"
# create an instance of Contract from a JSON string
contract_instance = Contract.from_json(json)
# print the JSON string representation of the object
print(Contract.to_json())

# convert the object into a dict
contract_dict = contract_instance.to_dict()
# create an instance of Contract from a dict
contract_from_dict = Contract.from_dict(contract_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



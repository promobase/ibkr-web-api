# ContractRules


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**order_types** | **List[str]** |  | [optional] 
**order_types_outside** | **List[str]** |  | [optional] 
**default_size** | **float** | default quantity you can use to place an order | [optional] 
**size_increment** | **float** |  | [optional] 
**tif_types** | **List[str]** |  | [optional] 
**limit_price** | **float** | default limit price you can use to prefill your order | [optional] 
**stopprice** | **float** | default stop price you can use to prefill your order | [optional] 
**preview** | **bool** | if you can preview the order or not with the whatif endpoint | [optional] 
**display_size** | **str** |  | [optional] 
**increment** | **str** |  | [optional] 

## Example

```python
from ibkr_web_api.models.contract_rules import ContractRules

# TODO update the JSON string below
json = "{}"
# create an instance of ContractRules from a JSON string
contract_rules_instance = ContractRules.from_json(json)
# print the JSON string representation of the object
print(ContractRules.to_json())

# convert the object into a dict
contract_rules_dict = contract_rules_instance.to_dict()
# create an instance of ContractRules from a dict
contract_rules_from_dict = ContractRules.from_dict(contract_rules_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



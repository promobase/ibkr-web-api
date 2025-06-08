# IserverContractRulesPost200ResponseRulesInnerOrderDefaultsInnerStringInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**orth** | **bool** | Outside of Regular Trading Hours | [optional] 
**sp** | **str** | Stop Price value | [optional] 
**lp** | **str** | Limit Price value | [optional] 
**pc** | **str** | Price Cap value | [optional] 
**ta** | **str** | Trailing amount value | [optional] 
**tu** | **str** | Trailing unit | [optional] 
**roa** | **str** | Releative offset amount | [optional] 
**rop** | **str** | Relative offset percent | [optional] 
**tt** | **str** | Touch trigger price | [optional] 
**unp** | **bool** | Use Net Price for Bonds | [optional] 

## Example

```python
from openapi_client.models.iserver_contract_rules_post200_response_rules_inner_order_defaults_inner_string_inner import IserverContractRulesPost200ResponseRulesInnerOrderDefaultsInnerStringInner

# TODO update the JSON string below
json = "{}"
# create an instance of IserverContractRulesPost200ResponseRulesInnerOrderDefaultsInnerStringInner from a JSON string
iserver_contract_rules_post200_response_rules_inner_order_defaults_inner_string_inner_instance = IserverContractRulesPost200ResponseRulesInnerOrderDefaultsInnerStringInner.from_json(json)
# print the JSON string representation of the object
print(IserverContractRulesPost200ResponseRulesInnerOrderDefaultsInnerStringInner.to_json())

# convert the object into a dict
iserver_contract_rules_post200_response_rules_inner_order_defaults_inner_string_inner_dict = iserver_contract_rules_post200_response_rules_inner_order_defaults_inner_string_inner_instance.to_dict()
# create an instance of IserverContractRulesPost200ResponseRulesInnerOrderDefaultsInnerStringInner from a dict
iserver_contract_rules_post200_response_rules_inner_order_defaults_inner_string_inner_from_dict = IserverContractRulesPost200ResponseRulesInnerOrderDefaultsInnerStringInner.from_dict(iserver_contract_rules_post200_response_rules_inner_order_defaults_inner_string_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



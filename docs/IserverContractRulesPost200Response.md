# IserverContractRulesPost200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**rules** | [**List[IserverContractRulesPost200ResponseRulesInner]**](IserverContractRulesPost200ResponseRulesInner.md) |  | [optional] 

## Example

```python
from ibkr-web-api.models.iserver_contract_rules_post200_response import IserverContractRulesPost200Response

# TODO update the JSON string below
json = "{}"
# create an instance of IserverContractRulesPost200Response from a JSON string
iserver_contract_rules_post200_response_instance = IserverContractRulesPost200Response.from_json(json)
# print the JSON string representation of the object
print(IserverContractRulesPost200Response.to_json())

# convert the object into a dict
iserver_contract_rules_post200_response_dict = iserver_contract_rules_post200_response_instance.to_dict()
# create an instance of IserverContractRulesPost200Response from a dict
iserver_contract_rules_post200_response_from_dict = IserverContractRulesPost200Response.from_dict(iserver_contract_rules_post200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



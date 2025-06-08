# IserverContractRulesPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**conid** | **str** | IBKR contract identifier | 
**is_buy** | **bool** | Side of the market rules apply too. Set to **true** for Buy Orders, set to **false** for Sell Orders | 

## Example

```python
from ibkr_web_api.models.iserver_contract_rules_post_request import IserverContractRulesPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IserverContractRulesPostRequest from a JSON string
iserver_contract_rules_post_request_instance = IserverContractRulesPostRequest.from_json(json)
# print the JSON string representation of the object
print(IserverContractRulesPostRequest.to_json())

# convert the object into a dict
iserver_contract_rules_post_request_dict = iserver_contract_rules_post_request_instance.to_dict()
# create an instance of IserverContractRulesPostRequest from a dict
iserver_contract_rules_post_request_from_dict = IserverContractRulesPostRequest.from_dict(iserver_contract_rules_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



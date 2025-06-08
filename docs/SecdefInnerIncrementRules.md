# SecdefInnerIncrementRules

Price increment value contract trades.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**lower_edge** | **float** | The minimum contract price on the market that supports the specified increment. | [optional] 
**increment** | **float** | The minimum increment value for contract price. | [optional] 

## Example

```python
from openapi_client.models.secdef_inner_increment_rules import SecdefInnerIncrementRules

# TODO update the JSON string below
json = "{}"
# create an instance of SecdefInnerIncrementRules from a JSON string
secdef_inner_increment_rules_instance = SecdefInnerIncrementRules.from_json(json)
# print the JSON string representation of the object
print(SecdefInnerIncrementRules.to_json())

# convert the object into a dict
secdef_inner_increment_rules_dict = secdef_inner_increment_rules_instance.to_dict()
# create an instance of SecdefInnerIncrementRules from a dict
secdef_inner_increment_rules_from_dict = SecdefInnerIncrementRules.from_dict(secdef_inner_increment_rules_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



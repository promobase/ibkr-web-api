# WagersInner

List of wagers

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**conid** | **float** |  | [optional] 
**curr** | **str** |  | [optional] 
**desc** | **str** |  | [optional] 
**part** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.wagers_inner import WagersInner

# TODO update the JSON string below
json = "{}"
# create an instance of WagersInner from a JSON string
wagers_inner_instance = WagersInner.from_json(json)
# print the JSON string representation of the object
print(WagersInner.to_json())

# convert the object into a dict
wagers_inner_dict = wagers_inner_instance.to_dict()
# create an instance of WagersInner from a dict
wagers_inner_from_dict = WagersInner.from_dict(wagers_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AllocationInnerGroupShort

short positions allocation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**banks** | **float** |  | [optional] 
**airlines** | **float** |  | [optional] 
**internet** | **float** |  | [optional] 

## Example

```python
from ibkr_web_api.models.allocation_inner_group_short import AllocationInnerGroupShort

# TODO update the JSON string below
json = "{}"
# create an instance of AllocationInnerGroupShort from a JSON string
allocation_inner_group_short_instance = AllocationInnerGroupShort.from_json(json)
# print the JSON string representation of the object
print(AllocationInnerGroupShort.to_json())

# convert the object into a dict
allocation_inner_group_short_dict = allocation_inner_group_short_instance.to_dict()
# create an instance of AllocationInnerGroupShort from a dict
allocation_inner_group_short_from_dict = AllocationInnerGroupShort.from_dict(allocation_inner_group_short_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



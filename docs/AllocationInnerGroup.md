# AllocationInnerGroup

portfolio allocation by group

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**long** | [**AllocationInnerGroupLong**](AllocationInnerGroupLong.md) |  | [optional] 
**short** | [**AllocationInnerGroupShort**](AllocationInnerGroupShort.md) |  | [optional] 

## Example

```python
from ibkr_web_api.models.allocation_inner_group import AllocationInnerGroup

# TODO update the JSON string below
json = "{}"
# create an instance of AllocationInnerGroup from a JSON string
allocation_inner_group_instance = AllocationInnerGroup.from_json(json)
# print the JSON string representation of the object
print(AllocationInnerGroup.to_json())

# convert the object into a dict
allocation_inner_group_dict = allocation_inner_group_instance.to_dict()
# create an instance of AllocationInnerGroup from a dict
allocation_inner_group_from_dict = AllocationInnerGroup.from_dict(allocation_inner_group_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



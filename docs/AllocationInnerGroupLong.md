# AllocationInnerGroupLong

long positions allocation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**computers** | **float** |  | [optional] 
**semiconductors** | **float** |  | [optional] 
**others** | **float** |  | [optional] 
**chemicals** | **float** |  | [optional] 
**apparel** | **float** |  | [optional] 
**communications** | **float** |  | [optional] 

## Example

```python
from ibkr-web-api.models.allocation_inner_group_long import AllocationInnerGroupLong

# TODO update the JSON string below
json = "{}"
# create an instance of AllocationInnerGroupLong from a JSON string
allocation_inner_group_long_instance = AllocationInnerGroupLong.from_json(json)
# print the JSON string representation of the object
print(AllocationInnerGroupLong.to_json())

# convert the object into a dict
allocation_inner_group_long_dict = allocation_inner_group_long_instance.to_dict()
# create an instance of AllocationInnerGroupLong from a dict
allocation_inner_group_long_from_dict = AllocationInnerGroupLong.from_dict(allocation_inner_group_long_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



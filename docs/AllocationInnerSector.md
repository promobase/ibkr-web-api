# AllocationInnerSector

portfolio allocation by sector

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**long** | [**AllocationInnerSectorLong**](AllocationInnerSectorLong.md) |  | [optional] 
**short** | [**AllocationInnerSectorShort**](AllocationInnerSectorShort.md) |  | [optional] 

## Example

```python
from ibkr-web-api.models.allocation_inner_sector import AllocationInnerSector

# TODO update the JSON string below
json = "{}"
# create an instance of AllocationInnerSector from a JSON string
allocation_inner_sector_instance = AllocationInnerSector.from_json(json)
# print the JSON string representation of the object
print(AllocationInnerSector.to_json())

# convert the object into a dict
allocation_inner_sector_dict = allocation_inner_sector_instance.to_dict()
# create an instance of AllocationInnerSector from a dict
allocation_inner_sector_from_dict = AllocationInnerSector.from_dict(allocation_inner_sector_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



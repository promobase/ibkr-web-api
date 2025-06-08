# AllocationInnerSectorLong

long positions allocation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**others** | **float** |  | [optional] 
**utilities** | **float** |  | [optional] 
**energy** | **float** |  | [optional] 
**technology** | **float** |  | [optional] 
**financial** | **float** |  | [optional] 
**communications** | **float** |  | [optional] 

## Example

```python
from ibkr_web_api.models.allocation_inner_sector_long import AllocationInnerSectorLong

# TODO update the JSON string below
json = "{}"
# create an instance of AllocationInnerSectorLong from a JSON string
allocation_inner_sector_long_instance = AllocationInnerSectorLong.from_json(json)
# print the JSON string representation of the object
print(AllocationInnerSectorLong.to_json())

# convert the object into a dict
allocation_inner_sector_long_dict = allocation_inner_sector_long_instance.to_dict()
# create an instance of AllocationInnerSectorLong from a dict
allocation_inner_sector_long_from_dict = AllocationInnerSectorLong.from_dict(allocation_inner_sector_long_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



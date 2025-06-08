# AllocationInnerSectorShort

short positions allocation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**industrial** | **float** |  | [optional] 
**consumer** | **float** |  | [optional] 
**diversified** | **float** |  | [optional] 

## Example

```python
from ibkr_web_api.models.allocation_inner_sector_short import AllocationInnerSectorShort

# TODO update the JSON string below
json = "{}"
# create an instance of AllocationInnerSectorShort from a JSON string
allocation_inner_sector_short_instance = AllocationInnerSectorShort.from_json(json)
# print the JSON string representation of the object
print(AllocationInnerSectorShort.to_json())

# convert the object into a dict
allocation_inner_sector_short_dict = allocation_inner_sector_short_instance.to_dict()
# create an instance of AllocationInnerSectorShort from a dict
allocation_inner_sector_short_from_dict = AllocationInnerSectorShort.from_dict(allocation_inner_sector_short_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



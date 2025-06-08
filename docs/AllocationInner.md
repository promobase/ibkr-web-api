# AllocationInner

allocation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**asset_class** | [**AllocationInnerAssetClass**](AllocationInnerAssetClass.md) |  | [optional] 
**sector** | [**AllocationInnerSector**](AllocationInnerSector.md) |  | [optional] 
**group** | [**AllocationInnerGroup**](AllocationInnerGroup.md) |  | [optional] 

## Example

```python
from ibkr-web-api.models.allocation_inner import AllocationInner

# TODO update the JSON string below
json = "{}"
# create an instance of AllocationInner from a JSON string
allocation_inner_instance = AllocationInner.from_json(json)
# print the JSON string representation of the object
print(AllocationInner.to_json())

# convert the object into a dict
allocation_inner_dict = allocation_inner_instance.to_dict()
# create an instance of AllocationInner from a dict
allocation_inner_from_dict = AllocationInner.from_dict(allocation_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



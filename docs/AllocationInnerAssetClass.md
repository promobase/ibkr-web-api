# AllocationInnerAssetClass

portfolio allocation by asset class

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**long** | [**AllocationInnerAssetClassLong**](AllocationInnerAssetClassLong.md) |  | [optional] 
**short** | [**AllocationInnerAssetClassShort**](AllocationInnerAssetClassShort.md) |  | [optional] 

## Example

```python
from ibkr-web-api.models.allocation_inner_asset_class import AllocationInnerAssetClass

# TODO update the JSON string below
json = "{}"
# create an instance of AllocationInnerAssetClass from a JSON string
allocation_inner_asset_class_instance = AllocationInnerAssetClass.from_json(json)
# print the JSON string representation of the object
print(AllocationInnerAssetClass.to_json())

# convert the object into a dict
allocation_inner_asset_class_dict = allocation_inner_asset_class_instance.to_dict()
# create an instance of AllocationInnerAssetClass from a dict
allocation_inner_asset_class_from_dict = AllocationInnerAssetClass.from_dict(allocation_inner_asset_class_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



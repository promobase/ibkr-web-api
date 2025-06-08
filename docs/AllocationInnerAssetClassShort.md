# AllocationInnerAssetClassShort

short positions allocation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**stk** | **float** |  | [optional] 
**opt** | **float** |  | [optional] 
**fut** | **float** |  | [optional] 
**war** | **float** |  | [optional] 
**bond** | **float** |  | [optional] 
**cash** | **float** |  | [optional] 

## Example

```python
from ibkr-web-api.models.allocation_inner_asset_class_short import AllocationInnerAssetClassShort

# TODO update the JSON string below
json = "{}"
# create an instance of AllocationInnerAssetClassShort from a JSON string
allocation_inner_asset_class_short_instance = AllocationInnerAssetClassShort.from_json(json)
# print the JSON string representation of the object
print(AllocationInnerAssetClassShort.to_json())

# convert the object into a dict
allocation_inner_asset_class_short_dict = allocation_inner_asset_class_short_instance.to_dict()
# create an instance of AllocationInnerAssetClassShort from a dict
allocation_inner_asset_class_short_from_dict = AllocationInnerAssetClassShort.from_dict(allocation_inner_asset_class_short_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



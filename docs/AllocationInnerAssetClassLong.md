# AllocationInnerAssetClassLong

long positions allocation

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
from openapi_client.models.allocation_inner_asset_class_long import AllocationInnerAssetClassLong

# TODO update the JSON string below
json = "{}"
# create an instance of AllocationInnerAssetClassLong from a JSON string
allocation_inner_asset_class_long_instance = AllocationInnerAssetClassLong.from_json(json)
# print the JSON string representation of the object
print(AllocationInnerAssetClassLong.to_json())

# convert the object into a dict
allocation_inner_asset_class_long_dict = allocation_inner_asset_class_long_instance.to_dict()
# create an instance of AllocationInnerAssetClassLong from a dict
allocation_inner_asset_class_long_from_dict = AllocationInnerAssetClassLong.from_dict(allocation_inner_asset_class_long_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



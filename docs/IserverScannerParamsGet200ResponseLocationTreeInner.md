# IserverScannerParamsGet200ResponseLocationTreeInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**display_name** | **str** |  | [optional] 
**type** | **str** |  | [optional] 
**locations** | [**List[IserverScannerParamsGet200ResponseLocationTreeInnerLocationsInner]**](IserverScannerParamsGet200ResponseLocationTreeInnerLocationsInner.md) |  | [optional] 

## Example

```python
from ibkr_web_api.models.iserver_scanner_params_get200_response_location_tree_inner import IserverScannerParamsGet200ResponseLocationTreeInner

# TODO update the JSON string below
json = "{}"
# create an instance of IserverScannerParamsGet200ResponseLocationTreeInner from a JSON string
iserver_scanner_params_get200_response_location_tree_inner_instance = IserverScannerParamsGet200ResponseLocationTreeInner.from_json(json)
# print the JSON string representation of the object
print(IserverScannerParamsGet200ResponseLocationTreeInner.to_json())

# convert the object into a dict
iserver_scanner_params_get200_response_location_tree_inner_dict = iserver_scanner_params_get200_response_location_tree_inner_instance.to_dict()
# create an instance of IserverScannerParamsGet200ResponseLocationTreeInner from a dict
iserver_scanner_params_get200_response_location_tree_inner_from_dict = IserverScannerParamsGet200ResponseLocationTreeInner.from_dict(iserver_scanner_params_get200_response_location_tree_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



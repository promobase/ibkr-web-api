# IserverScannerParamsGet200ResponseScanTypeListInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**display_name** | **str** |  | [optional] 
**code** | **str** |  | [optional] 
**instruments** | **List[str]** |  | [optional] 

## Example

```python
from ibkr_web_api.models.iserver_scanner_params_get200_response_scan_type_list_inner import IserverScannerParamsGet200ResponseScanTypeListInner

# TODO update the JSON string below
json = "{}"
# create an instance of IserverScannerParamsGet200ResponseScanTypeListInner from a JSON string
iserver_scanner_params_get200_response_scan_type_list_inner_instance = IserverScannerParamsGet200ResponseScanTypeListInner.from_json(json)
# print the JSON string representation of the object
print(IserverScannerParamsGet200ResponseScanTypeListInner.to_json())

# convert the object into a dict
iserver_scanner_params_get200_response_scan_type_list_inner_dict = iserver_scanner_params_get200_response_scan_type_list_inner_instance.to_dict()
# create an instance of IserverScannerParamsGet200ResponseScanTypeListInner from a dict
iserver_scanner_params_get200_response_scan_type_list_inner_from_dict = IserverScannerParamsGet200ResponseScanTypeListInner.from_dict(iserver_scanner_params_get200_response_scan_type_list_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



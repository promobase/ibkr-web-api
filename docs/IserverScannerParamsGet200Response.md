# IserverScannerParamsGet200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**scan_type_list** | [**List[IserverScannerParamsGet200ResponseScanTypeListInner]**](IserverScannerParamsGet200ResponseScanTypeListInner.md) |  | [optional] 
**instrument_list** | [**List[IserverScannerParamsGet200ResponseInstrumentListInner]**](IserverScannerParamsGet200ResponseInstrumentListInner.md) |  | [optional] 
**filter_list** | [**List[IserverScannerParamsGet200ResponseFilterListInner]**](IserverScannerParamsGet200ResponseFilterListInner.md) |  | [optional] 
**location_tree** | [**List[IserverScannerParamsGet200ResponseLocationTreeInner]**](IserverScannerParamsGet200ResponseLocationTreeInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.iserver_scanner_params_get200_response import IserverScannerParamsGet200Response

# TODO update the JSON string below
json = "{}"
# create an instance of IserverScannerParamsGet200Response from a JSON string
iserver_scanner_params_get200_response_instance = IserverScannerParamsGet200Response.from_json(json)
# print the JSON string representation of the object
print(IserverScannerParamsGet200Response.to_json())

# convert the object into a dict
iserver_scanner_params_get200_response_dict = iserver_scanner_params_get200_response_instance.to_dict()
# create an instance of IserverScannerParamsGet200Response from a dict
iserver_scanner_params_get200_response_from_dict = IserverScannerParamsGet200Response.from_dict(iserver_scanner_params_get200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



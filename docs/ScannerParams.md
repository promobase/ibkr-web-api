# ScannerParams


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**instrument** | **str** | Contains an instrument, which to scan for. For example - \&quot;STK\&quot; | [optional] 
**type** | **str** | Specify the scan type to use. For example - \&quot;MOST_ACTIVE_USD\&quot; | [optional] 
**location** | **str** | Contains location code, where to look for specified instrument. For example - \&quot;STK.US.MAJOR\&quot; | [optional] 
**filter** | [**List[ScannerParamsFilterInner]**](ScannerParamsFilterInner.md) | Contains list of filters supported for the scanner | [optional] 

## Example

```python
from openapi_client.models.scanner_params import ScannerParams

# TODO update the JSON string below
json = "{}"
# create an instance of ScannerParams from a JSON string
scanner_params_instance = ScannerParams.from_json(json)
# print the JSON string representation of the object
print(ScannerParams.to_json())

# convert the object into a dict
scanner_params_dict = scanner_params_instance.to_dict()
# create an instance of ScannerParams from a dict
scanner_params_from_dict = ScannerParams.from_dict(scanner_params_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



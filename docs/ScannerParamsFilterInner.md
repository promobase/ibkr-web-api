# ScannerParamsFilterInner

Contains list of supported filters. The code of the filter along with user-specified value has to be sued to apply a filter to scanner query. For example - [{\"code\":\"usdVolume\",\"value\":500}]. You can also specify multiple filters - \"filter\":[{\"code\":\"value\"},{\"code\":\"value\"},{\"code\":\"value\"}]

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | [optional] 
**value** | **float** |  | [optional] 

## Example

```python
from ibkr_web_api.models.scanner_params_filter_inner import ScannerParamsFilterInner

# TODO update the JSON string below
json = "{}"
# create an instance of ScannerParamsFilterInner from a JSON string
scanner_params_filter_inner_instance = ScannerParamsFilterInner.from_json(json)
# print the JSON string representation of the object
print(ScannerParamsFilterInner.to_json())

# convert the object into a dict
scanner_params_filter_inner_dict = scanner_params_filter_inner_instance.to_dict()
# create an instance of ScannerParamsFilterInner from a dict
scanner_params_filter_inner_from_dict = ScannerParamsFilterInner.from_dict(scanner_params_filter_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ScannerResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total** | **int** |  | [optional] 
**size** | **int** |  | [optional] 
**offset** | **int** |  | [optional] 
**scan_time** | **str** |  | [optional] 
**id** | **float** |  | [optional] 
**position** | **str** |  | [optional] 
**contracts** | [**ScannerResultContracts**](ScannerResultContracts.md) |  | [optional] 

## Example

```python
from ibkr-web-api.models.scanner_result import ScannerResult

# TODO update the JSON string below
json = "{}"
# create an instance of ScannerResult from a JSON string
scanner_result_instance = ScannerResult.from_json(json)
# print the JSON string representation of the object
print(ScannerResult.to_json())

# convert the object into a dict
scanner_result_dict = scanner_result_instance.to_dict()
# create an instance of ScannerResult from a dict
scanner_result_from_dict = ScannerResult.from_dict(scanner_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ScannerResultContracts

Contains list of contracts matching the scanner query

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contract** | [**List[ScannerResultContractsContractInner]**](ScannerResultContractsContractInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.scanner_result_contracts import ScannerResultContracts

# TODO update the JSON string below
json = "{}"
# create an instance of ScannerResultContracts from a JSON string
scanner_result_contracts_instance = ScannerResultContracts.from_json(json)
# print the JSON string representation of the object
print(ScannerResultContracts.to_json())

# convert the object into a dict
scanner_result_contracts_dict = scanner_result_contracts_instance.to_dict()
# create an instance of ScannerResultContracts from a dict
scanner_result_contracts_from_dict = ScannerResultContracts.from_dict(scanner_result_contracts_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



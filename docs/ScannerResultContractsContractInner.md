# ScannerResultContractsContractInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**in_scan_time** | **str** |  | [optional] 
**distance** | **int** |  | [optional] 
**contract_id** | **int** |  | [optional] 

## Example

```python
from ibkr_web_api.models.scanner_result_contracts_contract_inner import ScannerResultContractsContractInner

# TODO update the JSON string below
json = "{}"
# create an instance of ScannerResultContractsContractInner from a JSON string
scanner_result_contracts_contract_inner_instance = ScannerResultContractsContractInner.from_json(json)
# print the JSON string representation of the object
print(ScannerResultContractsContractInner.to_json())

# convert the object into a dict
scanner_result_contracts_contract_inner_dict = scanner_result_contracts_contract_inner_instance.to_dict()
# create an instance of ScannerResultContractsContractInner from a dict
scanner_result_contracts_contract_inner_from_dict = ScannerResultContractsContractInner.from_dict(scanner_result_contracts_contract_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



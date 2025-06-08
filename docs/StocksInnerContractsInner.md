# StocksInnerContractsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**conid** | **int** | conid of the stock contract | [optional] 
**exchange** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.stocks_inner_contracts_inner import StocksInnerContractsInner

# TODO update the JSON string below
json = "{}"
# create an instance of StocksInnerContractsInner from a JSON string
stocks_inner_contracts_inner_instance = StocksInnerContractsInner.from_json(json)
# print the JSON string representation of the object
print(StocksInnerContractsInner.to_json())

# convert the object into a dict
stocks_inner_contracts_inner_dict = stocks_inner_contracts_inner_instance.to_dict()
# create an instance of StocksInnerContractsInner from a dict
stocks_inner_contracts_inner_from_dict = StocksInnerContractsInner.from_dict(stocks_inner_contracts_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



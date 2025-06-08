# StocksInner

future contract information

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | company name | [optional] 
**chinese_name** | **str** | company name in Chinese | [optional] 
**asset_class** | **str** |  | [optional] 
**contracts** | [**List[StocksInnerContractsInner]**](StocksInnerContractsInner.md) | array of contracts from different exchanges | [optional] 

## Example

```python
from ibkr-web-api.models.stocks_inner import StocksInner

# TODO update the JSON string below
json = "{}"
# create an instance of StocksInner from a JSON string
stocks_inner_instance = StocksInner.from_json(json)
# print the JSON string representation of the object
print(StocksInner.to_json())

# convert the object into a dict
stocks_inner_dict = stocks_inner_instance.to_dict()
# create an instance of StocksInner from a dict
stocks_inner_from_dict = StocksInner.from_dict(stocks_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



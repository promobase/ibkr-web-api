# FuturesInner

future contract information

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**symbol** | **str** |  | [optional] 
**conid** | **int** | conid of the future contract | [optional] 
**underlying_conid** | **int** |  | [optional] 
**expiration_date** | **str** |  | [optional] 
**ltd** | **str** | last trading day | [optional] 

## Example

```python
from ibkr-web-api.models.futures_inner import FuturesInner

# TODO update the JSON string below
json = "{}"
# create an instance of FuturesInner from a JSON string
futures_inner_instance = FuturesInner.from_json(json)
# print the JSON string representation of the object
print(FuturesInner.to_json())

# convert the object into a dict
futures_inner_dict = futures_inner_instance.to_dict()
# create an instance of FuturesInner from a dict
futures_inner_from_dict = FuturesInner.from_dict(futures_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



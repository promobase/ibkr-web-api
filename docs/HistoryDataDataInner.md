# HistoryDataDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**o** | **float** | open price | [optional] 
**c** | **float** | close price | [optional] 
**h** | **float** | high price | [optional] 
**l** | **float** | low price | [optional] 
**v** | **float** | volume | [optional] 
**t** | **float** | unix time stamp | [optional] 

## Example

```python
from ibkr-web-api.models.history_data_data_inner import HistoryDataDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of HistoryDataDataInner from a JSON string
history_data_data_inner_instance = HistoryDataDataInner.from_json(json)
# print the JSON string representation of the object
print(HistoryDataDataInner.to_json())

# convert the object into a dict
history_data_data_inner_dict = history_data_data_inner_instance.to_dict()
# create an instance of HistoryDataDataInner from a dict
history_data_data_inner_from_dict = HistoryDataDataInner.from_dict(history_data_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# HistoryResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bars** | [**HistoryResultBars**](HistoryResultBars.md) |  | [optional] 

## Example

```python
from ibkr-web-api.models.history_result import HistoryResult

# TODO update the JSON string below
json = "{}"
# create an instance of HistoryResult from a JSON string
history_result_instance = HistoryResult.from_json(json)
# print the JSON string representation of the object
print(HistoryResult.to_json())

# convert the object into a dict
history_result_dict = history_result_instance.to_dict()
# create an instance of HistoryResult from a dict
history_result_from_dict = HistoryResult.from_dict(history_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# HistoryResultBarsDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**t** | **float** | Time - Formatted in unix time in ms. | [optional] 
**o** | **float** | Open - First price returned for bar value. | [optional] 
**c** | **float** | Close - Last price returned for bar value. | [optional] 
**h** | **float** | High - High price returned for bar value. | [optional] 
**l** | **float** | Low - Last price returned for bar value. | [optional] 
**v** | **float** | Volume - Traded volume for bar value. | [optional] 

## Example

```python
from ibkr_web_api.models.history_result_bars_data_inner import HistoryResultBarsDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of HistoryResultBarsDataInner from a JSON string
history_result_bars_data_inner_instance = HistoryResultBarsDataInner.from_json(json)
# print the JSON string representation of the object
print(HistoryResultBarsDataInner.to_json())

# convert the object into a dict
history_result_bars_data_inner_dict = history_result_bars_data_inner_instance.to_dict()
# create an instance of HistoryResultBarsDataInner from a dict
history_result_bars_data_inner_from_dict = HistoryResultBarsDataInner.from_dict(history_result_bars_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



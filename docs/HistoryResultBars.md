# HistoryResultBars


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**open** | **float** | First price returned for bar value. | [optional] 
**start_time** | **str** | Start Time in the format YYYYMMDD. | [optional] 
**start_time_val** | **int** | Start Time Value - Formatted in unix time in ms. | [optional] 
**end_time** | **str** | End Time in the format YYYYMMDD. | [optional] 
**end_time_val** | **int** | End Time Value - Formatted in unix time in ms. | [optional] 
**points** | **int** | total number of data points. | [optional] 
**data** | [**List[HistoryResultBarsDataInner]**](HistoryResultBarsDataInner.md) |  | [optional] 
**mkt_data_delay** | **int** | If 0 then data is returned in real time. Otherwise will return the number of seconds history data is delayed. | [optional] 

## Example

```python
from ibkr-web-api.models.history_result_bars import HistoryResultBars

# TODO update the JSON string below
json = "{}"
# create an instance of HistoryResultBars from a JSON string
history_result_bars_instance = HistoryResultBars.from_json(json)
# print the JSON string representation of the object
print(HistoryResultBars.to_json())

# convert the object into a dict
history_result_bars_dict = history_result_bars_instance.to_dict()
# create an instance of HistoryResultBars from a dict
history_result_bars_from_dict = HistoryResultBars.from_dict(history_result_bars_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



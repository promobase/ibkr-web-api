# HistoryData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**symbol** | **str** | Underlying symbol | [optional] 
**text** | **str** | companyName | [optional] 
**price_factor** | **int** | priceFactor is price increment obtained from display rule | [optional] 
**start_time** | **str** | start date time in the format YYYYMMDD-HH:mm:ss | [optional] 
**high** | **str** | High value during this time series with format %h/%v/%t. %h is the high price (scaled by priceFactor), %v is volume (volume factor will always be 100 (reported volume &#x3D; actual volume/100)) and %t is minutes from start time of the chart  | [optional] 
**low** | **str** | Low value during this time series with format %l/%v/%t. %l is the low price (scaled by priceFactor), %v is volume (volume factor will always be 100 (reported volume &#x3D; actual volume/100)) and %t is minutes from start time of the chart  | [optional] 
**time_period** | **str** | The duration for the historical data request | [optional] 
**bar_length** | **int** | The number of seconds in a bar | [optional] 
**md_availability** | **str** | Market Data Availability. The field may contain two chars. The first char is the primary code: S &#x3D; Streaming, R &#x3D; Realtime, D &#x3D; Delayed, Z &#x3D; Frozen, Y &#x3D; Frozen Delayed. The second char is the secondary code: P &#x3D; Snapshot Available, p &#x3D; Consolidated.  | [optional] 
**mkt_data_delay** | **int** | The time it takes, in milliseconds, to process the historical data request | [optional] 
**outside_rth** | **bool** | The historical data returned includes outside of regular trading hours  | [optional] 
**trading_day_duration** | **int** | The number of seconds in the trading day | [optional] 
**volume_factor** | **int** |  | [optional] 
**price_display_rule** | **int** |  | [optional] 
**price_display_value** | **str** |  | [optional] 
**negative_capable** | **bool** |  | [optional] 
**message_version** | **int** |  | [optional] 
**data** | [**List[HistoryDataDataInner]**](HistoryDataDataInner.md) |  | [optional] 
**points** | **int** | total number of points | [optional] 
**travel_time** | **int** |  | [optional] 

## Example

```python
from ibkr-web-api.models.history_data import HistoryData

# TODO update the JSON string below
json = "{}"
# create an instance of HistoryData from a JSON string
history_data_instance = HistoryData.from_json(json)
# print the JSON string representation of the object
print(HistoryData.to_json())

# convert the object into a dict
history_data_dict = history_data_instance.to_dict()
# create an instance of HistoryData from a dict
history_data_from_dict = HistoryData.from_dict(history_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



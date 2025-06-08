# TrsrvSecdefScheduleGet200ResponseSchedulesInnerTradingTimes

Returns tradingTime in exchange time zone.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**opening_time** | **int** |  | [optional] 
**closing_time** | **int** |  | [optional] 
**cancel_day_orders** | **str** |  | [optional] 

## Example

```python
from ibkr_web_api.models.trsrv_secdef_schedule_get200_response_schedules_inner_trading_times import TrsrvSecdefScheduleGet200ResponseSchedulesInnerTradingTimes

# TODO update the JSON string below
json = "{}"
# create an instance of TrsrvSecdefScheduleGet200ResponseSchedulesInnerTradingTimes from a JSON string
trsrv_secdef_schedule_get200_response_schedules_inner_trading_times_instance = TrsrvSecdefScheduleGet200ResponseSchedulesInnerTradingTimes.from_json(json)
# print the JSON string representation of the object
print(TrsrvSecdefScheduleGet200ResponseSchedulesInnerTradingTimes.to_json())

# convert the object into a dict
trsrv_secdef_schedule_get200_response_schedules_inner_trading_times_dict = trsrv_secdef_schedule_get200_response_schedules_inner_trading_times_instance.to_dict()
# create an instance of TrsrvSecdefScheduleGet200ResponseSchedulesInnerTradingTimes from a dict
trsrv_secdef_schedule_get200_response_schedules_inner_trading_times_from_dict = TrsrvSecdefScheduleGet200ResponseSchedulesInnerTradingTimes.from_dict(trsrv_secdef_schedule_get200_response_schedules_inner_trading_times_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



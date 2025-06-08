# TrsrvSecdefScheduleGet200ResponseSchedulesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**clearing_cycle_end_time** | **int** |  | [optional] 
**trading_schedule_date** | **int** | 20000101 stands for any Sat, 20000102 stands for any Sun, ... 20000107 stands for any Fri. Any other date stands for itself. | [optional] 
**sessions** | [**TrsrvSecdefScheduleGet200ResponseSchedulesInnerSessions**](TrsrvSecdefScheduleGet200ResponseSchedulesInnerSessions.md) |  | [optional] 
**trading_times** | [**TrsrvSecdefScheduleGet200ResponseSchedulesInnerTradingTimes**](TrsrvSecdefScheduleGet200ResponseSchedulesInnerTradingTimes.md) |  | [optional] 

## Example

```python
from openapi_client.models.trsrv_secdef_schedule_get200_response_schedules_inner import TrsrvSecdefScheduleGet200ResponseSchedulesInner

# TODO update the JSON string below
json = "{}"
# create an instance of TrsrvSecdefScheduleGet200ResponseSchedulesInner from a JSON string
trsrv_secdef_schedule_get200_response_schedules_inner_instance = TrsrvSecdefScheduleGet200ResponseSchedulesInner.from_json(json)
# print the JSON string representation of the object
print(TrsrvSecdefScheduleGet200ResponseSchedulesInner.to_json())

# convert the object into a dict
trsrv_secdef_schedule_get200_response_schedules_inner_dict = trsrv_secdef_schedule_get200_response_schedules_inner_instance.to_dict()
# create an instance of TrsrvSecdefScheduleGet200ResponseSchedulesInner from a dict
trsrv_secdef_schedule_get200_response_schedules_inner_from_dict = TrsrvSecdefScheduleGet200ResponseSchedulesInner.from_dict(trsrv_secdef_schedule_get200_response_schedules_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# TrsrvSecdefScheduleGet200ResponseSchedulesInnerSessions

If the LIQUID hours differs from the total trading day then a separate 'session' tag is returned.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**opening_time** | **int** |  | [optional] 
**closing_time** | **int** |  | [optional] 
**prop** | **str** | If the whole trading day is considered LIQUID then the value &#39;LIQUID&#39; is returned. | [optional] 

## Example

```python
from ibkr-web-api.models.trsrv_secdef_schedule_get200_response_schedules_inner_sessions import TrsrvSecdefScheduleGet200ResponseSchedulesInnerSessions

# TODO update the JSON string below
json = "{}"
# create an instance of TrsrvSecdefScheduleGet200ResponseSchedulesInnerSessions from a JSON string
trsrv_secdef_schedule_get200_response_schedules_inner_sessions_instance = TrsrvSecdefScheduleGet200ResponseSchedulesInnerSessions.from_json(json)
# print the JSON string representation of the object
print(TrsrvSecdefScheduleGet200ResponseSchedulesInnerSessions.to_json())

# convert the object into a dict
trsrv_secdef_schedule_get200_response_schedules_inner_sessions_dict = trsrv_secdef_schedule_get200_response_schedules_inner_sessions_instance.to_dict()
# create an instance of TrsrvSecdefScheduleGet200ResponseSchedulesInnerSessions from a dict
trsrv_secdef_schedule_get200_response_schedules_inner_sessions_from_dict = TrsrvSecdefScheduleGet200ResponseSchedulesInnerSessions.from_dict(trsrv_secdef_schedule_get200_response_schedules_inner_sessions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



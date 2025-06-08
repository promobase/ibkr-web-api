# TrsrvSecdefScheduleGet200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Exchange parameter id | [optional] 
**trade_venue_id** | **str** | Reference on a trade venue of given exchange parameter | [optional] 
**schedules** | [**List[TrsrvSecdefScheduleGet200ResponseSchedulesInner]**](TrsrvSecdefScheduleGet200ResponseSchedulesInner.md) | Always contains at least one &#39;tradingTime&#39;  and zero or more &#39;sessionTime&#39; tags | [optional] 

## Example

```python
from openapi_client.models.trsrv_secdef_schedule_get200_response import TrsrvSecdefScheduleGet200Response

# TODO update the JSON string below
json = "{}"
# create an instance of TrsrvSecdefScheduleGet200Response from a JSON string
trsrv_secdef_schedule_get200_response_instance = TrsrvSecdefScheduleGet200Response.from_json(json)
# print the JSON string representation of the object
print(TrsrvSecdefScheduleGet200Response.to_json())

# convert the object into a dict
trsrv_secdef_schedule_get200_response_dict = trsrv_secdef_schedule_get200_response_instance.to_dict()
# create an instance of TrsrvSecdefScheduleGet200Response from a dict
trsrv_secdef_schedule_get200_response_from_dict = TrsrvSecdefScheduleGet200Response.from_dict(trsrv_secdef_schedule_get200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



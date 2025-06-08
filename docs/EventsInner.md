# EventsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**index_date_type** | **str** |  | [optional] 
**event_type** | **str** |  | [optional] 
**data** | **object** | will be different for different event types | [optional] 
**conids** | **List[str]** |  | [optional] 
**index_date** | **str** | for exmple 20180817T040000+0000 | [optional] 
**source** | **str** | for example RSE | [optional] 
**event_key** | **str** | for example 11662135 | [optional] 
**tooltips** | **object** |  | [optional] 
**status** | **str** |  | [optional] 

## Example

```python
from ibkr-web-api.models.events_inner import EventsInner

# TODO update the JSON string below
json = "{}"
# create an instance of EventsInner from a JSON string
events_inner_instance = EventsInner.from_json(json)
# print the JSON string representation of the object
print(EventsInner.to_json())

# convert the object into a dict
events_inner_dict = events_inner_instance.to_dict()
# create an instance of EventsInner from a dict
events_inner_from_dict = EventsInner.from_dict(events_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



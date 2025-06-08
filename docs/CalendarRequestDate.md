# CalendarRequestDate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**start** | **str** | start date of a period. for example 20180808-0400 | [optional] 
**end** | **str** | end date of a period. for example 20180808-0400 | [optional] 

## Example

```python
from ibkr_web_api.models.calendar_request_date import CalendarRequestDate

# TODO update the JSON string below
json = "{}"
# create an instance of CalendarRequestDate from a JSON string
calendar_request_date_instance = CalendarRequestDate.from_json(json)
# print the JSON string representation of the object
print(CalendarRequestDate.to_json())

# convert the object into a dict
calendar_request_date_dict = calendar_request_date_instance.to_dict()
# create an instance of CalendarRequestDate from a dict
calendar_request_date_from_dict = CalendarRequestDate.from_dict(calendar_request_date_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



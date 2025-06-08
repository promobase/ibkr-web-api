# CalendarRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_date** | [**CalendarRequestDate**](CalendarRequestDate.md) |  | [optional] 
**filters** | [**CalendarRequestFilters**](CalendarRequestFilters.md) |  | [optional] 

## Example

```python
from ibkr_web_api.models.calendar_request import CalendarRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CalendarRequest from a JSON string
calendar_request_instance = CalendarRequest.from_json(json)
# print the JSON string representation of the object
print(CalendarRequest.to_json())

# convert the object into a dict
calendar_request_dict = calendar_request_instance.to_dict()
# create an instance of CalendarRequest from a dict
calendar_request_from_dict = CalendarRequest.from_dict(calendar_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



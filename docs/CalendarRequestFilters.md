# CalendarRequestFilters


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**recently_held** | **str** | value can be &#39;true&#39; or &#39;false&#39;. | [optional] 
**corporate_earnings** | **str** | value can be &#39;true&#39; or &#39;false&#39;. | [optional] 
**div_ex_dates** | **str** | value can be &#39;true&#39; or &#39;false&#39;. | [optional] 
**ipo** | **str** | value can be &#39;true&#39; or &#39;false&#39;. | [optional] 
**splits** | **str** | value can be &#39;true&#39; or &#39;false&#39;. | [optional] 
**corporate_events** | **str** | value can be &#39;true&#39; or &#39;false&#39;. | [optional] 
**economic_events** | **str** | value can be &#39;true&#39; or &#39;false&#39;. | [optional] 
**option_show_monthly** | **str** | value can be &#39;true&#39; or &#39;false&#39;. | [optional] 
**option_show_weekly** | **str** | value can be &#39;true&#39; or &#39;false&#39;. | [optional] 
**country** | **str** | default is &#39;All&#39;. | [optional] 
**limit** | **str** | default is &#39;250&#39;. | [optional] 
**limit_region** | **str** | default is &#39;50&#39;. | [optional] 

## Example

```python
from openapi_client.models.calendar_request_filters import CalendarRequestFilters

# TODO update the JSON string below
json = "{}"
# create an instance of CalendarRequestFilters from a JSON string
calendar_request_filters_instance = CalendarRequestFilters.from_json(json)
# print the JSON string representation of the object
print(CalendarRequestFilters.to_json())

# convert the object into a dict
calendar_request_filters_dict = calendar_request_filters_instance.to_dict()
# create an instance of CalendarRequestFilters from a dict
calendar_request_filters_from_dict = CalendarRequestFilters.from_dict(calendar_request_filters_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# PerformanceNav

Net asset value data for the account or consolidated accounts. NAV data is not applicable to benchmarks.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dates** | **List[str]** | array of dates, the length should be same as the length of returns inside data. | [optional] 
**freq** | **str** | D means Day | [optional] 
**data** | [**List[PerformanceCpsDataInner]**](PerformanceCpsDataInner.md) |  | [optional] 

## Example

```python
from ibkr-web-api.models.performance_nav import PerformanceNav

# TODO update the JSON string below
json = "{}"
# create an instance of PerformanceNav from a JSON string
performance_nav_instance = PerformanceNav.from_json(json)
# print the JSON string representation of the object
print(PerformanceNav.to_json())

# convert the object into a dict
performance_nav_dict = performance_nav_instance.to_dict()
# create an instance of PerformanceNav from a dict
performance_nav_from_dict = PerformanceNav.from_dict(performance_nav_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



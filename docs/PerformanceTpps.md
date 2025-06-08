# PerformanceTpps

Time period performance data

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dates** | **List[str]** | array of dates, the length should be same as the length of returns inside data. | [optional] 
**freq** | **str** | M means Month | [optional] 
**data** | [**List[PerformanceCpsDataInner]**](PerformanceCpsDataInner.md) |  | [optional] 

## Example

```python
from ibkr-web-api.models.performance_tpps import PerformanceTpps

# TODO update the JSON string below
json = "{}"
# create an instance of PerformanceTpps from a JSON string
performance_tpps_instance = PerformanceTpps.from_json(json)
# print the JSON string representation of the object
print(PerformanceTpps.to_json())

# convert the object into a dict
performance_tpps_dict = performance_tpps_instance.to_dict()
# create an instance of PerformanceTpps from a dict
performance_tpps_from_dict = PerformanceTpps.from_dict(performance_tpps_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



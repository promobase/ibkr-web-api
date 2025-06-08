# PerformanceCps

Cumulative performance data

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dates** | **List[str]** | array of dates, the length should be same as the length of returns inside data. | [optional] 
**freq** | **str** | D means Day | [optional] 
**data** | [**List[PerformanceCpsDataInner]**](PerformanceCpsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.performance_cps import PerformanceCps

# TODO update the JSON string below
json = "{}"
# create an instance of PerformanceCps from a JSON string
performance_cps_instance = PerformanceCps.from_json(json)
# print the JSON string representation of the object
print(PerformanceCps.to_json())

# convert the object into a dict
performance_cps_dict = performance_cps_instance.to_dict()
# create an instance of PerformanceCps from a dict
performance_cps_from_dict = PerformanceCps.from_dict(performance_cps_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



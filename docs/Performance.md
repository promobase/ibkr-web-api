# Performance


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**cps** | [**PerformanceCps**](PerformanceCps.md) |  | [optional] 
**tpps** | [**PerformanceTpps**](PerformanceTpps.md) |  | [optional] 
**nav** | [**PerformanceNav**](PerformanceNav.md) |  | [optional] 
**pm** | **str** |  | [optional] 
**included** | **List[str]** |  | [optional] 
**currency_type** | **str** |  | [optional] 
**rc** | **int** |  | [optional] 

## Example

```python
from ibkr-web-api.models.performance import Performance

# TODO update the JSON string below
json = "{}"
# create an instance of Performance from a JSON string
performance_instance = Performance.from_json(json)
# print the JSON string representation of the object
print(Performance.to_json())

# convert the object into a dict
performance_dict = performance_instance.to_dict()
# create an instance of Performance from a dict
performance_from_dict = Performance.from_dict(performance_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



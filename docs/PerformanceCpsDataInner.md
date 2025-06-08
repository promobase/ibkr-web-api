# PerformanceCpsDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**id_type** | **str** | for example-- acctid | [optional] 
**start** | **str** | start date-- yyyyMMdd | [optional] 
**base_currency** | **str** |  | [optional] 
**returns** | **List[float]** | each value stands for price change percent of corresponding date in dates array | [optional] 
**end** | **str** | end date-- yyyyMMdd | [optional] 

## Example

```python
from ibkr_web_api.models.performance_cps_data_inner import PerformanceCpsDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of PerformanceCpsDataInner from a JSON string
performance_cps_data_inner_instance = PerformanceCpsDataInner.from_json(json)
# print the JSON string representation of the object
print(PerformanceCpsDataInner.to_json())

# convert the object into a dict
performance_cps_data_inner_dict = performance_cps_data_inner_instance.to_dict()
# create an instance of PerformanceCpsDataInner from a dict
performance_cps_data_inner_from_dict = PerformanceCpsDataInner.from_dict(performance_cps_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



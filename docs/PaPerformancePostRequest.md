# PaPerformancePostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**acct_ids** | **List[str]** |  | [optional] 
**freq** | **str** | Frequency of cumulative performance data points: &#39;D&#39;aily, &#39;M&#39;onthly,&#39;Q&#39;uarterly.  | [optional] 

## Example

```python
from ibkr_web_api.models.pa_performance_post_request import PaPerformancePostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PaPerformancePostRequest from a JSON string
pa_performance_post_request_instance = PaPerformancePostRequest.from_json(json)
# print the JSON string representation of the object
print(PaPerformancePostRequest.to_json())

# convert the object into a dict
pa_performance_post_request_dict = pa_performance_post_request_instance.to_dict()
# create an instance of PaPerformancePostRequest from a dict
pa_performance_post_request_from_dict = PaPerformancePostRequest.from_dict(pa_performance_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



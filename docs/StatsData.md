# StatsData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**conid** | **float** |  | [optional] 
**exchange** | **str** |  | [optional] 
**v** | **float** |  | [optional] 
**t** | **float** |  | [optional] 
**tt** | **float** |  | [optional] 
**p** | **str** | Object, payload depends on event type. See confluence page for IGEvntUpd. | [optional] 

## Example

```python
from ibkr-web-api.models.stats_data import StatsData

# TODO update the JSON string below
json = "{}"
# create an instance of StatsData from a JSON string
stats_data_instance = StatsData.from_json(json)
# print the JSON string representation of the object
print(StatsData.to_json())

# convert the object into a dict
stats_data_dict = stats_data_instance.to_dict()
# create an instance of StatsData from a dict
stats_data_from_dict = StatsData.from_dict(stats_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



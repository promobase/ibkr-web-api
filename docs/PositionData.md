# PositionData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**conid** | **float** | Contract identifier from IBKR&#39;s database. | [optional] 
**position** | **float** | Number of shares or quantity of the position. | [optional] 
**avg_cost** | **float** | Average cost of the position. | [optional] 

## Example

```python
from ibkr-web-api.models.position_data import PositionData

# TODO update the JSON string below
json = "{}"
# create an instance of PositionData from a JSON string
position_data_instance = PositionData.from_json(json)
# print the JSON string representation of the object
print(PositionData.to_json())

# convert the object into a dict
position_data_dict = position_data_instance.to_dict()
# create an instance of PositionData from a dict
position_data_from_dict = PositionData.from_dict(position_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



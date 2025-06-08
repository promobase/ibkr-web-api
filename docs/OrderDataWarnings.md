# OrderDataWarnings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**pricecap** | **str** |  | [optional] 
**time** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.order_data_warnings import OrderDataWarnings

# TODO update the JSON string below
json = "{}"
# create an instance of OrderDataWarnings from a JSON string
order_data_warnings_instance = OrderDataWarnings.from_json(json)
# print the JSON string representation of the object
print(OrderDataWarnings.to_json())

# convert the object into a dict
order_data_warnings_dict = order_data_warnings_instance.to_dict()
# create an instance of OrderDataWarnings from a dict
order_data_warnings_from_dict = OrderDataWarnings.from_dict(order_data_warnings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



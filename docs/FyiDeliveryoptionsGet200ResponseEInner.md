# FyiDeliveryoptionsGet200ResponseEInner

device

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**nm** | **str** | device name | [optional] 
**i** | **str** | device id | [optional] 
**ui** | **str** | unique device id | [optional] 
**a** | **str** | device is enabled or not 0-true, 1-false. | [optional] 

## Example

```python
from openapi_client.models.fyi_deliveryoptions_get200_response_e_inner import FyiDeliveryoptionsGet200ResponseEInner

# TODO update the JSON string below
json = "{}"
# create an instance of FyiDeliveryoptionsGet200ResponseEInner from a JSON string
fyi_deliveryoptions_get200_response_e_inner_instance = FyiDeliveryoptionsGet200ResponseEInner.from_json(json)
# print the JSON string representation of the object
print(FyiDeliveryoptionsGet200ResponseEInner.to_json())

# convert the object into a dict
fyi_deliveryoptions_get200_response_e_inner_dict = fyi_deliveryoptions_get200_response_e_inner_instance.to_dict()
# create an instance of FyiDeliveryoptionsGet200ResponseEInner from a dict
fyi_deliveryoptions_get200_response_e_inner_from_dict = FyiDeliveryoptionsGet200ResponseEInner.from_dict(fyi_deliveryoptions_get200_response_e_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



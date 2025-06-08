# FyiDeliveryoptionsGet200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**m** | **int** | Email option is enabled or not 0-off, 1-on. | [optional] 
**e** | [**List[FyiDeliveryoptionsGet200ResponseEInner]**](FyiDeliveryoptionsGet200ResponseEInner.md) |  | [optional] 

## Example

```python
from ibkr_web_api.models.fyi_deliveryoptions_get200_response import FyiDeliveryoptionsGet200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FyiDeliveryoptionsGet200Response from a JSON string
fyi_deliveryoptions_get200_response_instance = FyiDeliveryoptionsGet200Response.from_json(json)
# print the JSON string representation of the object
print(FyiDeliveryoptionsGet200Response.to_json())

# convert the object into a dict
fyi_deliveryoptions_get200_response_dict = fyi_deliveryoptions_get200_response_instance.to_dict()
# create an instance of FyiDeliveryoptionsGet200Response from a dict
fyi_deliveryoptions_get200_response_from_dict = FyiDeliveryoptionsGet200Response.from_dict(fyi_deliveryoptions_get200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



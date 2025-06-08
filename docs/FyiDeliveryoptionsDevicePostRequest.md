# FyiDeliveryoptionsDevicePostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**devicename** | **str** |  | [optional] 
**device_id** | **str** |  | [optional] 
**ui_name** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 

## Example

```python
from ibkr-web-api.models.fyi_deliveryoptions_device_post_request import FyiDeliveryoptionsDevicePostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FyiDeliveryoptionsDevicePostRequest from a JSON string
fyi_deliveryoptions_device_post_request_instance = FyiDeliveryoptionsDevicePostRequest.from_json(json)
# print the JSON string representation of the object
print(FyiDeliveryoptionsDevicePostRequest.to_json())

# convert the object into a dict
fyi_deliveryoptions_device_post_request_dict = fyi_deliveryoptions_device_post_request_instance.to_dict()
# create an instance of FyiDeliveryoptionsDevicePostRequest from a dict
fyi_deliveryoptions_device_post_request_from_dict = FyiDeliveryoptionsDevicePostRequest.from_dict(fyi_deliveryoptions_device_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



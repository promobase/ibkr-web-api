# FyiSettingsGet200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**a** | **int** | optional, if A doesn&#39;t exist, it means user can&#39;t toggle this option. 0-off, 1-on. | [optional] 
**fc** | **str** | fyi code | [optional] 
**h** | **int** | disclaimer read, 1 &#x3D; yes, &#x3D; 0 no. | [optional] 
**fd** | **str** | detailed description | [optional] 
**fn** | **str** | title | [optional] 

## Example

```python
from openapi_client.models.fyi_settings_get200_response_inner import FyiSettingsGet200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of FyiSettingsGet200ResponseInner from a JSON string
fyi_settings_get200_response_inner_instance = FyiSettingsGet200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(FyiSettingsGet200ResponseInner.to_json())

# convert the object into a dict
fyi_settings_get200_response_inner_dict = fyi_settings_get200_response_inner_instance.to_dict()
# create an instance of FyiSettingsGet200ResponseInner from a dict
fyi_settings_get200_response_inner_from_dict = FyiSettingsGet200ResponseInner.from_dict(fyi_settings_get200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



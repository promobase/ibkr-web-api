# FyiSettingsTypecodePostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | [optional] 

## Example

```python
from ibkr_web_api.models.fyi_settings_typecode_post_request import FyiSettingsTypecodePostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FyiSettingsTypecodePostRequest from a JSON string
fyi_settings_typecode_post_request_instance = FyiSettingsTypecodePostRequest.from_json(json)
# print the JSON string representation of the object
print(FyiSettingsTypecodePostRequest.to_json())

# convert the object into a dict
fyi_settings_typecode_post_request_dict = fyi_settings_typecode_post_request_instance.to_dict()
# create an instance of FyiSettingsTypecodePostRequest from a dict
fyi_settings_typecode_post_request_from_dict = FyiSettingsTypecodePostRequest.from_dict(fyi_settings_typecode_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



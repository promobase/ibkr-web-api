# SsoValidateGet200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**login_type** | **float** | 1 for Live, 2 for Paper | [optional] 
**user_name** | **str** | Username | [optional] 
**user_id** | **float** | User ID | [optional] 
**expire** | **float** | Time in milliseconds until session expires. Caller needs to call the again to re-validate session | [optional] 
**result** | **bool** | true if session was validated; false if not. | [optional] 
**auth_time** | **float** | Time of session validation | [optional] 

## Example

```python
from ibkr_web_api.models.sso_validate_get200_response import SsoValidateGet200Response

# TODO update the JSON string below
json = "{}"
# create an instance of SsoValidateGet200Response from a JSON string
sso_validate_get200_response_instance = SsoValidateGet200Response.from_json(json)
# print the JSON string representation of the object
print(SsoValidateGet200Response.to_json())

# convert the object into a dict
sso_validate_get200_response_dict = sso_validate_get200_response_instance.to_dict()
# create an instance of SsoValidateGet200Response from a dict
sso_validate_get200_response_from_dict = SsoValidateGet200Response.from_dict(sso_validate_get200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



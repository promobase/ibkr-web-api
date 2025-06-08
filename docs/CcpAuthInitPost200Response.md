# CcpAuthInitPost200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**challenge** | **object** | Challenge in hex format | [optional] 

## Example

```python
from openapi_client.models.ccp_auth_init_post200_response import CcpAuthInitPost200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CcpAuthInitPost200Response from a JSON string
ccp_auth_init_post200_response_instance = CcpAuthInitPost200Response.from_json(json)
# print the JSON string representation of the object
print(CcpAuthInitPost200Response.to_json())

# convert the object into a dict
ccp_auth_init_post200_response_dict = ccp_auth_init_post200_response_instance.to_dict()
# create an instance of CcpAuthInitPost200Response from a dict
ccp_auth_init_post200_response_from_dict = CcpAuthInitPost200Response.from_dict(ccp_auth_init_post200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



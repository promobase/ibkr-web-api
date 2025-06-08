# CcpAuthResponsePost200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**passed** | **bool** | If sso authentication completed | [optional] 
**authenticated** | **bool** | If connection is authenticated | [optional] 
**connected** | **bool** | Connected to CCP session | [optional] 
**competing** | **bool** | If user already has an existing brokerage session running. | [optional] 

## Example

```python
from openapi_client.models.ccp_auth_response_post200_response import CcpAuthResponsePost200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CcpAuthResponsePost200Response from a JSON string
ccp_auth_response_post200_response_instance = CcpAuthResponsePost200Response.from_json(json)
# print the JSON string representation of the object
print(CcpAuthResponsePost200Response.to_json())

# convert the object into a dict
ccp_auth_response_post200_response_dict = ccp_auth_response_post200_response_instance.to_dict()
# create an instance of CcpAuthResponsePost200Response from a dict
ccp_auth_response_post200_response_from_dict = CcpAuthResponsePost200Response.from_dict(ccp_auth_response_post200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



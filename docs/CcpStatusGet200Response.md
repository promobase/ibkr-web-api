# CcpStatusGet200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**authenticated** | **bool** | Login session is authenticated to the CCP. | [optional] 
**connected** | **bool** | Login session is connected | [optional] 
**name** | **str** | server name | [optional] 

## Example

```python
from ibkr_web_api.models.ccp_status_get200_response import CcpStatusGet200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CcpStatusGet200Response from a JSON string
ccp_status_get200_response_instance = CcpStatusGet200Response.from_json(json)
# print the JSON string representation of the object
print(CcpStatusGet200Response.to_json())

# convert the object into a dict
ccp_status_get200_response_dict = ccp_status_get200_response_instance.to_dict()
# create an instance of CcpStatusGet200Response from a dict
ccp_status_get200_response_from_dict = CcpStatusGet200Response.from_dict(ccp_status_get200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



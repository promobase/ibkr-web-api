# CcpAuthResponsePostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**response** | **str** |  | [optional] 

## Example

```python
from ibkr-web-api.models.ccp_auth_response_post_request import CcpAuthResponsePostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CcpAuthResponsePostRequest from a JSON string
ccp_auth_response_post_request_instance = CcpAuthResponsePostRequest.from_json(json)
# print the JSON string representation of the object
print(CcpAuthResponsePostRequest.to_json())

# convert the object into a dict
ccp_auth_response_post_request_dict = ccp_auth_response_post_request_instance.to_dict()
# create an instance of CcpAuthResponsePostRequest from a dict
ccp_auth_response_post_request_from_dict = CcpAuthResponsePostRequest.from_dict(ccp_auth_response_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



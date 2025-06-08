# CcpAccountGet200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**main_acct** | **str** | The primary or parent account. | [optional] 
**acct_list** | [**List[CcpAccountGet200ResponseAcctListInner]**](CcpAccountGet200ResponseAcctListInner.md) | List of tradeable or Sub Accounts | [optional] 

## Example

```python
from openapi_client.models.ccp_account_get200_response import CcpAccountGet200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CcpAccountGet200Response from a JSON string
ccp_account_get200_response_instance = CcpAccountGet200Response.from_json(json)
# print the JSON string representation of the object
print(CcpAccountGet200Response.to_json())

# convert the object into a dict
ccp_account_get200_response_dict = ccp_account_get200_response_instance.to_dict()
# create an instance of CcpAccountGet200Response from a dict
ccp_account_get200_response_from_dict = CcpAccountGet200Response.from_dict(ccp_account_get200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CcpAccountGet200ResponseAcctListInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_0** | **str** | For multi-account structures each trading account will numbered from 0 to ... | [optional] 

## Example

```python
from ibkr_web_api.models.ccp_account_get200_response_acct_list_inner import CcpAccountGet200ResponseAcctListInner

# TODO update the JSON string below
json = "{}"
# create an instance of CcpAccountGet200ResponseAcctListInner from a JSON string
ccp_account_get200_response_acct_list_inner_instance = CcpAccountGet200ResponseAcctListInner.from_json(json)
# print the JSON string representation of the object
print(CcpAccountGet200ResponseAcctListInner.to_json())

# convert the object into a dict
ccp_account_get200_response_acct_list_inner_dict = ccp_account_get200_response_acct_list_inner_instance.to_dict()
# create an instance of CcpAccountGet200ResponseAcctListInner from a dict
ccp_account_get200_response_acct_list_inner_from_dict = CcpAccountGet200ResponseAcctListInner.from_dict(ccp_account_get200_response_acct_list_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# IserverAccountsGet200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**accounts** | **List[str]** | Unique account id | [optional] 
**aliases** | **object** | Account Id and its alias | [optional] 
**selected_account** | **str** |  | [optional] 

## Example

```python
from ibkr_web_api.models.iserver_accounts_get200_response import IserverAccountsGet200Response

# TODO update the JSON string below
json = "{}"
# create an instance of IserverAccountsGet200Response from a JSON string
iserver_accounts_get200_response_instance = IserverAccountsGet200Response.from_json(json)
# print the JSON string representation of the object
print(IserverAccountsGet200Response.to_json())

# convert the object into a dict
iserver_accounts_get200_response_dict = iserver_accounts_get200_response_instance.to_dict()
# create an instance of IserverAccountsGet200Response from a dict
iserver_accounts_get200_response_from_dict = IserverAccountsGet200Response.from_dict(iserver_accounts_get200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



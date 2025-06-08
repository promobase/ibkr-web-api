# AuthStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**authenticated** | **bool** | Brokerage session is authenticated | [optional] 
**connected** | **bool** | Connected to backend | [optional] 
**competing** | **bool** | Brokerage session is competing, e.g. user is logged in to IBKR Mobile, WebTrader, TWS or other trading platforms. | [optional] 
**fail** | **str** | Authentication failed, why. | [optional] 
**message** | **str** | System messages that may affect trading | [optional] 
**prompts** | **List[str]** | Prompt messages that may affect trading or the account | [optional] 

## Example

```python
from openapi_client.models.auth_status import AuthStatus

# TODO update the JSON string below
json = "{}"
# create an instance of AuthStatus from a JSON string
auth_status_instance = AuthStatus.from_json(json)
# print the JSON string representation of the object
print(AuthStatus.to_json())

# convert the object into a dict
auth_status_dict = auth_status_instance.to_dict()
# create an instance of AuthStatus from a dict
auth_status_from_dict = AuthStatus.from_dict(auth_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



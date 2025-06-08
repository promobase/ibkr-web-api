# IserverAccountPost200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**set** | **bool** |  | [optional] 
**acct_id** | **str** |  | [optional] 

## Example

```python
from ibkr_web_api.models.iserver_account_post200_response import IserverAccountPost200Response

# TODO update the JSON string below
json = "{}"
# create an instance of IserverAccountPost200Response from a JSON string
iserver_account_post200_response_instance = IserverAccountPost200Response.from_json(json)
# print the JSON string representation of the object
print(IserverAccountPost200Response.to_json())

# convert the object into a dict
iserver_account_post200_response_dict = iserver_account_post200_response_instance.to_dict()
# create an instance of IserverAccountPost200Response from a dict
iserver_account_post200_response_from_dict = IserverAccountPost200Response.from_dict(iserver_account_post200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



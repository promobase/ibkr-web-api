# IserverMarketdataUnsubscribeallGet200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**confirmed** | **bool** | true means market data is cancelled, false means it is not. | [optional] 

## Example

```python
from ibkr_web_api.models.iserver_marketdata_unsubscribeall_get200_response import IserverMarketdataUnsubscribeallGet200Response

# TODO update the JSON string below
json = "{}"
# create an instance of IserverMarketdataUnsubscribeallGet200Response from a JSON string
iserver_marketdata_unsubscribeall_get200_response_instance = IserverMarketdataUnsubscribeallGet200Response.from_json(json)
# print the JSON string representation of the object
print(IserverMarketdataUnsubscribeallGet200Response.to_json())

# convert the object into a dict
iserver_marketdata_unsubscribeall_get200_response_dict = iserver_marketdata_unsubscribeall_get200_response_instance.to_dict()
# create an instance of IserverMarketdataUnsubscribeallGet200Response from a dict
iserver_marketdata_unsubscribeall_get200_response_from_dict = IserverMarketdataUnsubscribeallGet200Response.from_dict(iserver_marketdata_unsubscribeall_get200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



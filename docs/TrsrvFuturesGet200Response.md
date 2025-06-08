# TrsrvFuturesGet200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**symbol** | [**List[FuturesInner]**](FuturesInner.md) |  | [optional] 

## Example

```python
from ibkr-web-api.models.trsrv_futures_get200_response import TrsrvFuturesGet200Response

# TODO update the JSON string below
json = "{}"
# create an instance of TrsrvFuturesGet200Response from a JSON string
trsrv_futures_get200_response_instance = TrsrvFuturesGet200Response.from_json(json)
# print the JSON string representation of the object
print(TrsrvFuturesGet200Response.to_json())

# convert the object into a dict
trsrv_futures_get200_response_dict = trsrv_futures_get200_response_instance.to_dict()
# create an instance of TrsrvFuturesGet200Response from a dict
trsrv_futures_get200_response_from_dict = TrsrvFuturesGet200Response.from_dict(trsrv_futures_get200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



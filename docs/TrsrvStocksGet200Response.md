# TrsrvStocksGet200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**symbol** | [**List[StocksInner]**](StocksInner.md) | This is an array of object(s), there could be multiple results under same symbol  | [optional] 

## Example

```python
from openapi_client.models.trsrv_stocks_get200_response import TrsrvStocksGet200Response

# TODO update the JSON string below
json = "{}"
# create an instance of TrsrvStocksGet200Response from a JSON string
trsrv_stocks_get200_response_instance = TrsrvStocksGet200Response.from_json(json)
# print the JSON string representation of the object
print(TrsrvStocksGet200Response.to_json())

# convert the object into a dict
trsrv_stocks_get200_response_dict = trsrv_stocks_get200_response_instance.to_dict()
# create an instance of TrsrvStocksGet200Response from a dict
trsrv_stocks_get200_response_from_dict = TrsrvStocksGet200Response.from_dict(trsrv_stocks_get200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



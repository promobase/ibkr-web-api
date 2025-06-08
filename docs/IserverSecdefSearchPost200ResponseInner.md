# IserverSecdefSearchPost200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**conid** | **int** | Contract Identifier | [optional] 
**company_header** | **str** | Company Name - Exchange | [optional] 
**company_name** | **str** |  | [optional] 
**symbol** | **str** | Underlying symbol | [optional] 
**description** | **str** | Exchange | [optional] 
**restricted** | **str** |  | [optional] 
**fop** | **str** | List of Future Option expirations in YYYMMDD format separated by semicolon | [optional] 
**opt** | **str** | List of Option expirations in YYYYMMDD format separated by semicolon | [optional] 
**war** | **str** | List of Warrant expirations in YYYYMMDD format separated by semicolon | [optional] 
**sections** | [**List[IserverSecdefSearchPost200ResponseInnerSectionsInner]**](IserverSecdefSearchPost200ResponseInnerSectionsInner.md) |  | [optional] 

## Example

```python
from ibkr-web-api.models.iserver_secdef_search_post200_response_inner import IserverSecdefSearchPost200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of IserverSecdefSearchPost200ResponseInner from a JSON string
iserver_secdef_search_post200_response_inner_instance = IserverSecdefSearchPost200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(IserverSecdefSearchPost200ResponseInner.to_json())

# convert the object into a dict
iserver_secdef_search_post200_response_inner_dict = iserver_secdef_search_post200_response_inner_instance.to_dict()
# create an instance of IserverSecdefSearchPost200ResponseInner from a dict
iserver_secdef_search_post200_response_inner_from_dict = IserverSecdefSearchPost200ResponseInner.from_dict(iserver_secdef_search_post200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



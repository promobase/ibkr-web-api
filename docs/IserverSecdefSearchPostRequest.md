# IserverSecdefSearchPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**symbol** | **str** | symbol or name to be searched | 
**name** | **bool** | should be true if the search is to be performed by name. false by default. | [optional] 
**sec_type** | **str** | If search is done by name, only the assets provided in this field will be returned. Currently, only STK is supported. | [optional] 

## Example

```python
from ibkr_web_api.models.iserver_secdef_search_post_request import IserverSecdefSearchPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IserverSecdefSearchPostRequest from a JSON string
iserver_secdef_search_post_request_instance = IserverSecdefSearchPostRequest.from_json(json)
# print the JSON string representation of the object
print(IserverSecdefSearchPostRequest.to_json())

# convert the object into a dict
iserver_secdef_search_post_request_dict = iserver_secdef_search_post_request_instance.to_dict()
# create an instance of IserverSecdefSearchPostRequest from a dict
iserver_secdef_search_post_request_from_dict = IserverSecdefSearchPostRequest.from_dict(iserver_secdef_search_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



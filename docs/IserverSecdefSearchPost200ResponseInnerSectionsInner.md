# IserverSecdefSearchPost200ResponseInnerSectionsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sec_type** | **str** | Asset Class | [optional] 
**months** | **str** | List of expiration month(s) and year(s) in MMMYY format separated by semicolon | [optional] 
**symbol** | **str** | Underlying symbol | [optional] 
**exchange** | **str** | Listing Exchange | [optional] 
**leg_sec_type** | **str** | For combo&#39;s defines the asset class for each leg | [optional] 

## Example

```python
from ibkr-web-api.models.iserver_secdef_search_post200_response_inner_sections_inner import IserverSecdefSearchPost200ResponseInnerSectionsInner

# TODO update the JSON string below
json = "{}"
# create an instance of IserverSecdefSearchPost200ResponseInnerSectionsInner from a JSON string
iserver_secdef_search_post200_response_inner_sections_inner_instance = IserverSecdefSearchPost200ResponseInnerSectionsInner.from_json(json)
# print the JSON string representation of the object
print(IserverSecdefSearchPost200ResponseInnerSectionsInner.to_json())

# convert the object into a dict
iserver_secdef_search_post200_response_inner_sections_inner_dict = iserver_secdef_search_post200_response_inner_sections_inner_instance.to_dict()
# create an instance of IserverSecdefSearchPost200ResponseInnerSectionsInner from a dict
iserver_secdef_search_post200_response_inner_sections_inner_from_dict = IserverSecdefSearchPost200ResponseInnerSectionsInner.from_dict(iserver_secdef_search_post200_response_inner_sections_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



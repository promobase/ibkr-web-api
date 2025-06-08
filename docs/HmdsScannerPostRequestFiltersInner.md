# HmdsScannerPostRequestFiltersInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | [optional] 
**value** | **object** | Value can be either an integer, double, boolean or a string depending upon the type of filter specified in the code section | [optional] 

## Example

```python
from ibkr-web-api.models.hmds_scanner_post_request_filters_inner import HmdsScannerPostRequestFiltersInner

# TODO update the JSON string below
json = "{}"
# create an instance of HmdsScannerPostRequestFiltersInner from a JSON string
hmds_scanner_post_request_filters_inner_instance = HmdsScannerPostRequestFiltersInner.from_json(json)
# print the JSON string representation of the object
print(HmdsScannerPostRequestFiltersInner.to_json())

# convert the object into a dict
hmds_scanner_post_request_filters_inner_dict = hmds_scanner_post_request_filters_inner_instance.to_dict()
# create an instance of HmdsScannerPostRequestFiltersInner from a dict
hmds_scanner_post_request_filters_inner_from_dict = HmdsScannerPostRequestFiltersInner.from_dict(hmds_scanner_post_request_filters_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



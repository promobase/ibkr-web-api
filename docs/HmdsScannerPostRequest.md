# HmdsScannerPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**instrument** | **str** |  | [optional] 
**locations** | **str** |  | [optional] 
**scan_code** | **str** |  | [optional] 
**sec_type** | **str** |  | [optional] 
**filters** | [**List[HmdsScannerPostRequestFiltersInner]**](HmdsScannerPostRequestFiltersInner.md) |  | [optional] 

## Example

```python
from ibkr-web-api.models.hmds_scanner_post_request import HmdsScannerPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of HmdsScannerPostRequest from a JSON string
hmds_scanner_post_request_instance = HmdsScannerPostRequest.from_json(json)
# print the JSON string representation of the object
print(HmdsScannerPostRequest.to_json())

# convert the object into a dict
hmds_scanner_post_request_dict = hmds_scanner_post_request_instance.to_dict()
# create an instance of HmdsScannerPostRequest from a dict
hmds_scanner_post_request_from_dict = HmdsScannerPostRequest.from_dict(hmds_scanner_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# PaSummaryPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**acct_ids** | **List[str]** |  | [optional] 

## Example

```python
from openapi_client.models.pa_summary_post_request import PaSummaryPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PaSummaryPostRequest from a JSON string
pa_summary_post_request_instance = PaSummaryPostRequest.from_json(json)
# print the JSON string representation of the object
print(PaSummaryPostRequest.to_json())

# convert the object into a dict
pa_summary_post_request_dict = pa_summary_post_request_instance.to_dict()
# create an instance of PaSummaryPostRequest from a dict
pa_summary_post_request_from_dict = PaSummaryPostRequest.from_dict(pa_summary_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



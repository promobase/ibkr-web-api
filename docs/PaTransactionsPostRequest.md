# PaTransactionsPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**acct_ids** | **List[str]** |  | [optional] 
**conids** | **List[float]** |  | [optional] 
**currency** | **str** | optional defaults to USD. | [optional] 
**days** | **float** | optional, default value is 90 | [optional] 

## Example

```python
from ibkr_web_api.models.pa_transactions_post_request import PaTransactionsPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PaTransactionsPostRequest from a JSON string
pa_transactions_post_request_instance = PaTransactionsPostRequest.from_json(json)
# print the JSON string representation of the object
print(PaTransactionsPostRequest.to_json())

# convert the object into a dict
pa_transactions_post_request_dict = pa_transactions_post_request_instance.to_dict()
# create an instance of PaTransactionsPostRequest from a dict
pa_transactions_post_request_from_dict = PaTransactionsPostRequest.from_dict(pa_transactions_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



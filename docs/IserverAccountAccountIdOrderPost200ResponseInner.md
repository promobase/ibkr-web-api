# IserverAccountAccountIdOrderPost200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**message** | **List[str]** | Please note here, if the message is a question, you have to reply to question in order to submit the order successfully. See more in the \&quot;/iserver/reply/{replyid}\&quot; endpoint.  | [optional] 

## Example

```python
from openapi_client.models.iserver_account_account_id_order_post200_response_inner import IserverAccountAccountIdOrderPost200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of IserverAccountAccountIdOrderPost200ResponseInner from a JSON string
iserver_account_account_id_order_post200_response_inner_instance = IserverAccountAccountIdOrderPost200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(IserverAccountAccountIdOrderPost200ResponseInner.to_json())

# convert the object into a dict
iserver_account_account_id_order_post200_response_inner_dict = iserver_account_account_id_order_post200_response_inner_instance.to_dict()
# create an instance of IserverAccountAccountIdOrderPost200ResponseInner from a dict
iserver_account_account_id_order_post200_response_inner_from_dict = IserverAccountAccountIdOrderPost200ResponseInner.from_dict(iserver_account_account_id_order_post200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



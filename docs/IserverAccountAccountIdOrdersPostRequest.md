# IserverAccountAccountIdOrdersPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**orders** | [**List[OrderRequest]**](OrderRequest.md) | Notes for bracket orders: 1. Children orders will not have its own \&quot;cOID\&quot;, so please donot pass \&quot;cOID\&quot; parameter in child order.Instead, they will have a \&quot;parentId\&quot; which must be equal to \&quot;cOID\&quot; of parent. 2. When you cancel a parent order, it will cancel all bracket orders, when you cancel one child order, it will also cancel its sibling order.  | [optional] 

## Example

```python
from ibkr_web_api.models.iserver_account_account_id_orders_post_request import IserverAccountAccountIdOrdersPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IserverAccountAccountIdOrdersPostRequest from a JSON string
iserver_account_account_id_orders_post_request_instance = IserverAccountAccountIdOrdersPostRequest.from_json(json)
# print the JSON string representation of the object
print(IserverAccountAccountIdOrdersPostRequest.to_json())

# convert the object into a dict
iserver_account_account_id_orders_post_request_dict = iserver_account_account_id_orders_post_request_instance.to_dict()
# create an instance of IserverAccountAccountIdOrdersPostRequest from a dict
iserver_account_account_id_orders_post_request_from_dict = IserverAccountAccountIdOrdersPostRequest.from_dict(iserver_account_account_id_orders_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



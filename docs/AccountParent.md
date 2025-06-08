# AccountParent


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**mmc** | **List[str]** |  | [optional] 
**account_id** | **str** | Account Number for Money Manager Client | [optional] 
**is_m_parent** | **bool** | Is MM a Parent Account | [optional] 
**is_m_child** | **bool** | Is MM a Child Account | [optional] 
**is_multiplex** | **bool** | Is a Multiplex Account. These are account models with individual account being parent and managed account being child. | [optional] 

## Example

```python
from ibkr-web-api.models.account_parent import AccountParent

# TODO update the JSON string below
json = "{}"
# create an instance of AccountParent from a JSON string
account_parent_instance = AccountParent.from_json(json)
# print the JSON string representation of the object
print(AccountParent.to_json())

# convert the object into a dict
account_parent_dict = account_parent_instance.to_dict()
# create an instance of AccountParent from a dict
account_parent_from_dict = AccountParent.from_dict(account_parent_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



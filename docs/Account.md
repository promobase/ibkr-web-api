# Account

account information

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | The account identification value | [optional] 
**account_id** | **str** | The account number | [optional] 
**account_van** | **str** | The accountAlias | [optional] 
**account_title** | **str** | Title of the account | [optional] 
**display_name** | **str** | Whichever value is not null in this priority | [optional] 
**account_alias** | **str** | User customizable account alias. Refer to [Configure Account Alias](https://guides.interactivebrokers.com/cp/cp.htm#am/settings/accountalias.htm) for details. | [optional] 
**account_status** | **float** | When the account was opened in unix time. | [optional] 
**currency** | **str** | Base currency of the account. | [optional] 
**type** | **str** | Account Type | [optional] 
**trading_type** | **str** | UNI - Deprecated property | [optional] 
**faclient** | **bool** | If an account is a sub-account to a Financial Advisor. | [optional] 
**clearing_status** | **str** | Status of the Account   * O &#x3D; Open   * P or N &#x3D; Pending   * A &#x3D; Abandoned   * R &#x3D; Rejected   * C &#x3D; Closed  | [optional] 
**covestor** | **bool** | Is a Covestor Account | [optional] 
**parent** | [**AccountParent**](AccountParent.md) |  | [optional] 
**desc** | **str** | Formatted \&quot;accountId - accountAlias\&quot; | [optional] 

## Example

```python
from ibkr-web-api.models.account import Account

# TODO update the JSON string below
json = "{}"
# create an instance of Account from a JSON string
account_instance = Account.from_json(json)
# print the JSON string representation of the object
print(Account.to_json())

# convert the object into a dict
account_dict = account_instance.to_dict()
# create an instance of Account from a dict
account_from_dict = Account.from_dict(account_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



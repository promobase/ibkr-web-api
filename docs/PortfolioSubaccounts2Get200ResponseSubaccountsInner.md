# PortfolioSubaccounts2Get200ResponseSubaccountsInner

Account information

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
**clearing_status** | **str** | Status of the Account   * O &#x3D; Open   * P or N &#x3D; Pending   * A &#x3D; Abandoned   * R &#x3D; Rejected   * C &#x3D; Closed   covestor:     type: boolean     description: Is a Covestor Account   parent:     type: object     properties:       mmc:         type: array         items:           type: string           description: Money Manager Client (MMC) Account       accountId:         type: string         description: Account Number for Money Manager Client       isMParent:         type: boolean         description: Is MM a Parent Account       isMChild:         type: boolean         description: Is MM a Child Account       isMultiplex:         type: boolean         description: Is a Multiplex Account. These are account models with individual account being parent and managed account being child.   desc:     type: string     description: Formatted \&quot;accountId - accountAlias\&quot;  | [optional] 

## Example

```python
from ibkr-web-api.models.portfolio_subaccounts2_get200_response_subaccounts_inner import PortfolioSubaccounts2Get200ResponseSubaccountsInner

# TODO update the JSON string below
json = "{}"
# create an instance of PortfolioSubaccounts2Get200ResponseSubaccountsInner from a JSON string
portfolio_subaccounts2_get200_response_subaccounts_inner_instance = PortfolioSubaccounts2Get200ResponseSubaccountsInner.from_json(json)
# print the JSON string representation of the object
print(PortfolioSubaccounts2Get200ResponseSubaccountsInner.to_json())

# convert the object into a dict
portfolio_subaccounts2_get200_response_subaccounts_inner_dict = portfolio_subaccounts2_get200_response_subaccounts_inner_instance.to_dict()
# create an instance of PortfolioSubaccounts2Get200ResponseSubaccountsInner from a dict
portfolio_subaccounts2_get200_response_subaccounts_inner_from_dict = PortfolioSubaccounts2Get200ResponseSubaccountsInner.from_dict(portfolio_subaccounts2_get200_response_subaccounts_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



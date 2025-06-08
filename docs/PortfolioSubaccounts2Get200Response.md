# PortfolioSubaccounts2Get200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | [**PortfolioSubaccounts2Get200ResponseMetadata**](PortfolioSubaccounts2Get200ResponseMetadata.md) |  | [optional] 
**subaccounts** | [**List[PortfolioSubaccounts2Get200ResponseSubaccountsInner]**](PortfolioSubaccounts2Get200ResponseSubaccountsInner.md) |  | [optional] 

## Example

```python
from ibkr_web_api.models.portfolio_subaccounts2_get200_response import PortfolioSubaccounts2Get200Response

# TODO update the JSON string below
json = "{}"
# create an instance of PortfolioSubaccounts2Get200Response from a JSON string
portfolio_subaccounts2_get200_response_instance = PortfolioSubaccounts2Get200Response.from_json(json)
# print the JSON string representation of the object
print(PortfolioSubaccounts2Get200Response.to_json())

# convert the object into a dict
portfolio_subaccounts2_get200_response_dict = portfolio_subaccounts2_get200_response_instance.to_dict()
# create an instance of PortfolioSubaccounts2Get200Response from a dict
portfolio_subaccounts2_get200_response_from_dict = PortfolioSubaccounts2Get200Response.from_dict(portfolio_subaccounts2_get200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



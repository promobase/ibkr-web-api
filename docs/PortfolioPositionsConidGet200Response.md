# PortfolioPositionsConidGet200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**acctid** | [**List[PositionInner]**](PositionInner.md) |  | [optional] 

## Example

```python
from ibkr-web-api.models.portfolio_positions_conid_get200_response import PortfolioPositionsConidGet200Response

# TODO update the JSON string below
json = "{}"
# create an instance of PortfolioPositionsConidGet200Response from a JSON string
portfolio_positions_conid_get200_response_instance = PortfolioPositionsConidGet200Response.from_json(json)
# print the JSON string representation of the object
print(PortfolioPositionsConidGet200Response.to_json())

# convert the object into a dict
portfolio_positions_conid_get200_response_dict = portfolio_positions_conid_get200_response_instance.to_dict()
# create an instance of PortfolioPositionsConidGet200Response from a dict
portfolio_positions_conid_get200_response_from_dict = PortfolioPositionsConidGet200Response.from_dict(portfolio_positions_conid_get200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



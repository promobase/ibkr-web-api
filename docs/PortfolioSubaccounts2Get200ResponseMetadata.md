# PortfolioSubaccounts2Get200ResponseMetadata


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total** | **float** | Number of sub-accounts | [optional] 
**page_size** | **float** | How many sub-accounts are returned for the page requested. A max of 20 per page. | [optional] 
**page_nume** | **float** | Current page number. | [optional] 

## Example

```python
from ibkr_web_api.models.portfolio_subaccounts2_get200_response_metadata import PortfolioSubaccounts2Get200ResponseMetadata

# TODO update the JSON string below
json = "{}"
# create an instance of PortfolioSubaccounts2Get200ResponseMetadata from a JSON string
portfolio_subaccounts2_get200_response_metadata_instance = PortfolioSubaccounts2Get200ResponseMetadata.from_json(json)
# print the JSON string representation of the object
print(PortfolioSubaccounts2Get200ResponseMetadata.to_json())

# convert the object into a dict
portfolio_subaccounts2_get200_response_metadata_dict = portfolio_subaccounts2_get200_response_metadata_instance.to_dict()
# create an instance of PortfolioSubaccounts2Get200ResponseMetadata from a dict
portfolio_subaccounts2_get200_response_metadata_from_dict = PortfolioSubaccounts2Get200ResponseMetadata.from_dict(portfolio_subaccounts2_get200_response_metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# Ledger


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**commoditymarketvalue** | **float** |  | [optional] 
**futuremarketvalue** | **float** |  | [optional] 
**settledcash** | **float** |  | [optional] 
**exchangerate** | **float** |  | [optional] 
**sessionid** | **int** |  | [optional] 
**cashbalance** | **float** |  | [optional] 
**corporatebondsmarketvalue** | **float** |  | [optional] 
**warrantsmarketvalue** | **float** |  | [optional] 
**netliquidationvalue** | **float** |  | [optional] 
**interest** | **float** |  | [optional] 
**unrealizedpnl** | **float** |  | [optional] 
**stockmarketvalue** | **float** |  | [optional] 
**moneyfunds** | **float** |  | [optional] 
**currency** | **str** |  | [optional] 
**realizedpnl** | **float** |  | [optional] 
**funds** | **float** |  | [optional] 
**acctcode** | **str** |  | [optional] 
**issueroptionsmarketvalue** | **float** |  | [optional] 
**key** | **str** |  | [optional] 
**timestamp** | **int** |  | [optional] 
**severity** | **int** |  | [optional] 

## Example

```python
from openapi_client.models.ledger import Ledger

# TODO update the JSON string below
json = "{}"
# create an instance of Ledger from a JSON string
ledger_instance = Ledger.from_json(json)
# print the JSON string representation of the object
print(Ledger.to_json())

# convert the object into a dict
ledger_dict = ledger_instance.to_dict()
# create an instance of Ledger from a dict
ledger_from_dict = Ledger.from_dict(ledger_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



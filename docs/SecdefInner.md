# SecdefInner

security definition information.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**conid** | **int** | IBKR contract identifier. | [optional] 
**currency** | **str** | Currency contract trades in. | [optional] 
**cross_currency** | **bool** | Defines if a derivative contract has a different currency. | [optional] 
**time** | **int** |  | [optional] 
**chinese_name** | **str** | HTML encoded company description in Chinese. | [optional] 
**all_exchanges** | **str** | List of exchanges and venues contract trades. | [optional] 
**listing_exchange** | **str** | Main trading venue. | [optional] 
**name** | **str** | Company Name. | [optional] 
**asset_class** | **str** | Group of financial instruments which have similar financial characteristics and behave similar in the marketplace. | [optional] 
**expiry** | **str** | Specific data contract expires. | [optional] 
**last_trading_day** | **str** | Final day derivative contract can be traded before delivery of the underlying asset or cash settlement. | [optional] 
**group** | **str** | Potential characteristic of each product. | [optional] 
**put_or_call** | **str** | Defines the right to buy or sell of the underlying security. | [optional] 
**sector** | **str** | The category of the economy. | [optional] 
**sector_group** | **str** | Stock Group contract belongs too. | [optional] 
**strike** | **float** | Set price at which a derivative contract can be bought or sold. | [optional] 
**ticker** | **str** | Contract symbol. | [optional] 
**und_conid** | **int** | Underlying contract identifier. | [optional] 
**multiplier** | **int** | Multiplier for total premium paid or received for derivative contract. | [optional] 
**type** | **str** | Stock type. | [optional] 
**und_comp** | **str** | Company name for underlying contract. | [optional] 
**und_sym** | **str** | IBKR Symbol for underlying contract. | [optional] 
**has_options** | **bool** | If contract has an option. | [optional] 
**full_name** | **str** | Formatted company name with underlying symbol, expiration, strike, right. | [optional] 
**is_us** | **bool** | If contract is a US contract. Currently supported for stocks, options and warrants. | [optional] 
**increment_rules** | [**SecdefInnerIncrementRules**](SecdefInnerIncrementRules.md) |  | [optional] 

## Example

```python
from openapi_client.models.secdef_inner import SecdefInner

# TODO update the JSON string below
json = "{}"
# create an instance of SecdefInner from a JSON string
secdef_inner_instance = SecdefInner.from_json(json)
# print the JSON string representation of the object
print(SecdefInner.to_json())

# convert the object into a dict
secdef_inner_dict = secdef_inner_instance.to_dict()
# create an instance of SecdefInner from a dict
secdef_inner_from_dict = SecdefInner.from_dict(secdef_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# IserverContractConidInfoAndRulesGet200ResponseRulesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**algo_eligible** | **bool** | Contract supports algo orders | [optional] 
**can_trade_acct_ids** | [**List[IserverContractRulesPost200ResponseRulesInnerCanTradeAcctIdsInner]**](IserverContractRulesPost200ResponseRulesInnerCanTradeAcctIdsInner.md) |  | [optional] 
**error** | **str** | Returns a description on any errors with order presets | [optional] 
**order_types** | [**List[IserverContractRulesPost200ResponseRulesInnerOrderTypesInner]**](IserverContractRulesPost200ResponseRulesInnerOrderTypesInner.md) |  | [optional] 
**ibalgo_types** | [**List[IserverContractRulesPost200ResponseRulesInnerIbalgoTypesInner]**](IserverContractRulesPost200ResponseRulesInnerIbalgoTypesInner.md) |  | [optional] 
**fraq_types** | [**List[IserverContractRulesPost200ResponseRulesInnerFraqTypesInner]**](IserverContractRulesPost200ResponseRulesInnerFraqTypesInner.md) |  | [optional] 
**cqt_types** | [**List[IserverContractRulesPost200ResponseRulesInnerCqtTypesInner]**](IserverContractRulesPost200ResponseRulesInnerCqtTypesInner.md) |  | [optional] 
**order_defaults** | [**List[IserverContractRulesPost200ResponseRulesInnerOrderDefaultsInner]**](IserverContractRulesPost200ResponseRulesInnerOrderDefaultsInner.md) | If object returned will provide the defaults based on user settings | [optional] 
**order_types_outside** | [**List[IserverContractRulesPost200ResponseRulesInnerOrderTypesOutsideInner]**](IserverContractRulesPost200ResponseRulesInnerOrderTypesOutsideInner.md) |  | [optional] 
**default_size** | **int** | Default quantity | [optional] 
**cash_size** | **int** | cash value | [optional] 
**size_increment** | **int** | increment quantity value | [optional] 
**tif_types** | [**List[IserverContractRulesPost200ResponseRulesInnerTifTypesInner]**](IserverContractRulesPost200ResponseRulesInnerTifTypesInner.md) |  | [optional] 
**default_tif** | **str** | Default time in force value | [optional] 
**limit_price** | **float** | Limit price | [optional] 
**stopprice** | **float** | Stop price | [optional] 
**order_origination** | **float** | Order origin designation for US securities options and Options Clearing Corporation | [optional] 
**preview** | **bool** | order preview required | [optional] 
**display_size** | **float** |  | [optional] 
**fraq_int** | **float** | decimal places for fractional order size | [optional] 
**cash_ccy** | **str** | Cash currency for the contract | [optional] 
**cash_qty_incr** | **float** | Increment value for cash quantity | [optional] 
**price_magnifier** | **float** | Price Magnifier | [optional] 
**negative_capable** | **bool** | trading negative price support | [optional] 
**increment** | **float** | Price increment value | [optional] 
**increment_digits** | **int** | Number of digits for price increment | [optional] 

## Example

```python
from ibkr_web_api.models.iserver_contract_conid_info_and_rules_get200_response_rules_inner import IserverContractConidInfoAndRulesGet200ResponseRulesInner

# TODO update the JSON string below
json = "{}"
# create an instance of IserverContractConidInfoAndRulesGet200ResponseRulesInner from a JSON string
iserver_contract_conid_info_and_rules_get200_response_rules_inner_instance = IserverContractConidInfoAndRulesGet200ResponseRulesInner.from_json(json)
# print the JSON string representation of the object
print(IserverContractConidInfoAndRulesGet200ResponseRulesInner.to_json())

# convert the object into a dict
iserver_contract_conid_info_and_rules_get200_response_rules_inner_dict = iserver_contract_conid_info_and_rules_get200_response_rules_inner_instance.to_dict()
# create an instance of IserverContractConidInfoAndRulesGet200ResponseRulesInner from a dict
iserver_contract_conid_info_and_rules_get200_response_rules_inner_from_dict = IserverContractConidInfoAndRulesGet200ResponseRulesInner.from_dict(iserver_contract_conid_info_and_rules_get200_response_rules_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



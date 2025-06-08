# IserverContractConidInfoAndRulesGet200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cfi_code** | **str** | Classification of Financial Instrument codes | [optional] 
**symbol** | **str** | Underlying symbol | [optional] 
**cusip** | **str** |  | [optional] 
**expiry_full** | **float** | Expiration Date in the format YYYYMMDD | [optional] 
**con_id** | **float** | IBKRs contract identifier | [optional] 
**maturity_date** | **float** | Date on which the underlying transaction settles if the option is exercised | [optional] 
**industry** | **str** | Specific group of companies or businesses. | [optional] 
**instrument_type** | **str** | Asset Class of the contract | [optional] 
**trading_class** | **str** | Designation of the contract | [optional] 
**valid_exchanges** | **str** | Comma separated list of exchanges or trading venues | [optional] 
**allow_sell_long** | **bool** | Allowed to sell shares that you own | [optional] 
**is_zero_commission_security** | **bool** | Supports zero commission trades | [optional] 
**local_symbol** | **str** | Contracts symbol from primary exchange. For options it is the OCC symbol. | [optional] 
**classifier** | **str** |  | [optional] 
**currency** | **str** | Currency contract trades in | [optional] 
**text** | **str** | Formatted contract parameters | [optional] 
**underlying_con_id** | **float** | IBKRs contract identifier for the underlying instrument | [optional] 
**r_t_h** | **bool** | Provides trading outside of Regular Trading Hours | [optional] 
**multiplier** | **str** | numerical value of each point of price movement | [optional] 
**strike** | **str** | fixed price at which the owner of the option buys or sells the underlying | [optional] 
**right** | **str** | Put or Call of the option | [optional] 
**underlying_issuer** | **str** | Legal entity for underlying contract | [optional] 
**contract_month** | **str** | Month the contract must be satisfied by making or accepting delivery | [optional] 
**company_name** | **str** | Contracts company name | [optional] 
**smart_available** | **bool** | Support IBKRs SMART routing | [optional] 
**exchange** | **str** | Primary Exchange, Routing or Trading Venue | [optional] 
**rules** | [**List[IserverContractConidInfoAndRulesGet200ResponseRulesInner]**](IserverContractConidInfoAndRulesGet200ResponseRulesInner.md) |  | [optional] 

## Example

```python
from ibkr-web-api.models.iserver_contract_conid_info_and_rules_get200_response import IserverContractConidInfoAndRulesGet200Response

# TODO update the JSON string below
json = "{}"
# create an instance of IserverContractConidInfoAndRulesGet200Response from a JSON string
iserver_contract_conid_info_and_rules_get200_response_instance = IserverContractConidInfoAndRulesGet200Response.from_json(json)
# print the JSON string representation of the object
print(IserverContractConidInfoAndRulesGet200Response.to_json())

# convert the object into a dict
iserver_contract_conid_info_and_rules_get200_response_dict = iserver_contract_conid_info_and_rules_get200_response_instance.to_dict()
# create an instance of IserverContractConidInfoAndRulesGet200Response from a dict
iserver_contract_conid_info_and_rules_get200_response_from_dict = IserverContractConidInfoAndRulesGet200Response.from_dict(iserver_contract_conid_info_and_rules_get200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



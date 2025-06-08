# IserverAccountOrdersGet200ResponseOrdersInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**acct** | **str** | Account number | [optional] 
**conidex** | **str** | conid and exchange. Format supports conid or conid@exchange | [optional] 
**conid** | **float** | Contract identifier | [optional] 
**order_id** | **str** | Order identifier | [optional] 
**cash_ccy** | **str** | Cash currency | [optional] 
**size_and_fills** | **str** | Quantity outstanding and total quantity concatenated with forward slash separator | [optional] 
**order_desc** | **str** | Order description | [optional] 
**description1** | **str** | Formatted ticker description | [optional] 
**ticker** | **str** | Underlying symbol | [optional] 
**sec_type** | **str** | Asset class | [optional] 
**listing_exchange** | **str** | Listing Exchange | [optional] 
**remaining_quantity** | **float** | Quantity remaining | [optional] 
**filled_quantity** | **float** | Quantity filled | [optional] 
**company_name** | **str** | Company Name | [optional] 
**status** | **str** | Status of the order | [optional] 
**orig_order_type** | **str** | Original order type | [optional] 
**supports_tax_opt** | **float** | Supports Tax Optimization with 0 for no and 1 for yes | [optional] 
**last_execution_time** | **float** | Last status update in format YYMMDDhhmms based in GMT | [optional] 
**last_execution_time_r** | **float** | Last status update unix time in ms | [optional] 
**order_type** | **str** | Order type | [optional] 
**order_ref** | **str** | Order reference | [optional] 
**side** | **str** | The side of the market of the order.  * BUY: Buy contract near posted ask price  * SELL: Sell contract near posted bid price  * ASSN: Option Assignment, if BUYSELL&#x3D;BUY and OptionType&#x3D;PUT or BUYSELL&#x3D;SELL and OptionType&#x3D;CALL  * EXER: Option Exercise, if BUYSELL&#x3D;SELL and OptionType&#x3D;PUT or BUYSELL&#x3D;BUY and OptionType&#x3D;CALL  | [optional] 
**time_in_force** | **str** | Time in force | [optional] 
**price** | **float** | Price of order | [optional] 
**bg_color** | **str** | Background color in hex format | [optional] 
**fg_color** | **str** | Foreground color in hex format | [optional] 

## Example

```python
from ibkr-web-api.models.iserver_account_orders_get200_response_orders_inner import IserverAccountOrdersGet200ResponseOrdersInner

# TODO update the JSON string below
json = "{}"
# create an instance of IserverAccountOrdersGet200ResponseOrdersInner from a JSON string
iserver_account_orders_get200_response_orders_inner_instance = IserverAccountOrdersGet200ResponseOrdersInner.from_json(json)
# print the JSON string representation of the object
print(IserverAccountOrdersGet200ResponseOrdersInner.to_json())

# convert the object into a dict
iserver_account_orders_get200_response_orders_inner_dict = iserver_account_orders_get200_response_orders_inner_instance.to_dict()
# create an instance of IserverAccountOrdersGet200ResponseOrdersInner from a dict
iserver_account_orders_get200_response_orders_inner_from_dict = IserverAccountOrdersGet200ResponseOrdersInner.from_dict(iserver_account_orders_get200_response_orders_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



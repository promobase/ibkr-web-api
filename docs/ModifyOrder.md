# ModifyOrder


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**acct_id** | **str** |  | [optional] 
**conid** | **int** |  | [optional] 
**order_type** | **str** | for example LMT | [optional] 
**outside_rth** | **bool** |  | [optional] 
**price** | **float** |  | [optional] 
**aux_price** | **float** |  | [optional] 
**side** | **str** | SELL or BUY | [optional] 
**listing_exchange** | **str** | optional, not required | [optional] 
**ticker** | **str** | The ticker symbol of the original place order | [optional] 
**tif** | **str** | Specify a time in force to change how long your order will continue to work in the market | [optional] 
**quantity** | **float** | usually integer, for some special cases can be float numbers | [optional] 
**deactivated** | **bool** | Set to true if you want to pause a working order. For details refer to the [TWS Users&#39; Guide:](https://guides.interactivebrokers.com/tws/twsguide.html#usersguidebook/getstarted/pause_execution.htm)  | [optional] 

## Example

```python
from ibkr-web-api.models.modify_order import ModifyOrder

# TODO update the JSON string below
json = "{}"
# create an instance of ModifyOrder from a JSON string
modify_order_instance = ModifyOrder.from_json(json)
# print the JSON string representation of the object
print(ModifyOrder.to_json())

# convert the object into a dict
modify_order_dict = modify_order_instance.to_dict()
# create an instance of ModifyOrder from a dict
modify_order_from_dict = ModifyOrder.from_dict(modify_order_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



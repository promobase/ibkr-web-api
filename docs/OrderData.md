# OrderData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**client_order_id** | **str** |  | [optional] 
**exec_id** | **str** |  | [optional] 
**exec_type** | **str** |  | [optional] 
**order_type** | **str** |  | [optional] 
**order_status** | **str** |  | [optional] 
**symbol** | **str** | Underlying symbol for contract | [optional] 
**order_qty** | **str** | Quantity of active order | [optional] 
**price** | **str** | Price of active order | [optional] 
**last_shares** | **str** | Quantity of the last partial fill | [optional] 
**last_price** | **str** | Price of the last partial fill | [optional] 
**cum_qty** | **str** | Cumulative fill quantity | [optional] 
**leaves_qty** | **str** | Remaining quantity to be filled | [optional] 
**avg_price** | **str** | Average fill price | [optional] 
**side** | **str** |  | [optional] 
**order_id** | **str** | Order identifier | [optional] 
**account** | **str** | Account number | [optional] 
**sec_type** | **str** | Contracts asset class | [optional] 
**tx_time** | **str** | Time of transaction in GMT, format YYYYMMDD-hh:m:ss | [optional] 
**rcpt_time** | **str** | Time of receipt in GMT, format YYYYMMDD-hh:mm:ss | [optional] 
**tif** | **str** | Time in Force | [optional] 
**conid** | **str** | Contract identifier from IBKR&#39;s database. | [optional] 
**currency** | **str** | Trading currency | [optional] 
**exchange** | **str** | Exchange or venue | [optional] 
**listing_exchange** | **str** | Listing Exchange | [optional] 
**text** | **float** | error message | [optional] 
**warnings** | [**OrderDataWarnings**](OrderDataWarnings.md) |  | [optional] 
**comm_curr** | **str** | Commission currency | [optional] 
**comms** | **str** | Commissions | [optional] 
**realized_pnl** | **str** | Realized PnL | [optional] 

## Example

```python
from openapi_client.models.order_data import OrderData

# TODO update the JSON string below
json = "{}"
# create an instance of OrderData from a JSON string
order_data_instance = OrderData.from_json(json)
# print the JSON string representation of the object
print(OrderData.to_json())

# convert the object into a dict
order_data_dict = order_data_instance.to_dict()
# create an instance of OrderData from a dict
order_data_from_dict = OrderData.from_dict(order_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



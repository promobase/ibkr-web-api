# OrderStatus

contains all the details of an order

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sub_type** | **str** | order sub-type | [optional] 
**request_id** | **str** | order request id | [optional] 
**order_id** | **int** | system generated order id, unique per account | [optional] 
**conidex** | **str** | conid and exchange. Format supports conid or conid@exchange | [optional] 
**symbol** | **str** | Underlying symbol | [optional] 
**side** | **str** | The side of the market of the order.   * B - Buy contract near posted ask price   * S - Sell contract near posted bid price   * X - Option expired  | [optional] 
**contract_description_1** | **str** | Format contract name | [optional] 
**listing_exchange** | **str** | Trading Exchange or Venue | [optional] 
**option_acct** | **str** |  | [optional] 
**company_name** | **str** | Contracts company name | [optional] 
**size** | **str** | Quantity updated | [optional] 
**total_size** | **str** | Total quantity | [optional] 
**currency** | **str** | Contract traded currency | [optional] 
**account** | **str** | account id | [optional] 
**order_type** | **str** | Types of orders | [optional] 
**limit_price** | **str** | Limit price | [optional] 
**stop_price** | **str** | Stop price | [optional] 
**cum_fill** | **str** | Cumulative fill | [optional] 
**order_status** | **str** | *  PendingSubmit - Indicates the order was sent, but confirmation has not been received that it has been received by the destination.                    Occurs most commonly if an exchange is closed. *  PendingCancel - Indicates that a request has been sent to cancel an order but confirmation has not been received of its cancellation. *  PreSubmitted - Indicates that a simulated order type has been accepted by the IBKR system and that this order has yet to be elected.                   The order is held in the IBKR system until the election criteria are met. At that time the order is transmitted to the order destination as specified. *  Submitted - Indicates that the order has been accepted at the order destination and is working. *  Cancelled - Indicates that the balance of the order has been confirmed cancelled by the IB system.                This could occur unexpectedly when IB or the destination has rejected the order. *  Filled - Indicates that the order has been completely filled. *  Inactive - Indicates the order is not working, for instance if the order was invalid and triggered an error message,               or if the order was to short a security and shares have not yet been located.  | [optional] 
**order_status_description** | **str** | Description of the order status | [optional] 
**tif** | **str** | Time-in-Force - length of time order will continue working before it is canceled. | [optional] 
**fg_color** | **str** | Foreground color in hex format | [optional] 
**bg_color** | **str** | Background color in hex format | [optional] 
**order_not_editable** | **bool** | If true not allowed to modify order | [optional] 
**editable_fields** | **str** | Fields that can be edited in escaped unicode characters | [optional] 
**cannot_cancel_order** | **bool** | If true not allowed to cancel order | [optional] 
**outside_rth** | **bool** | If true order trades outside regular trading hours | [optional] 
**deactivate_order** | **bool** | If true order is de-activated | [optional] 
**use_price_mgmt_algo** | **bool** | If true price management algo is enabled, refer to https://www.interactivebrokers.com/en/index.php?f&#x3D;43423 | [optional] 
**sec_type** | **str** | Asset class | [optional] 
**available_chart_periods** | **str** | List of available chart periods | [optional] 
**order_description** | **str** | Format description of order | [optional] 
**order_description_with_contract** | **str** | order_description with the symbol | [optional] 
**alert_active** | **int** |  | [optional] 
**child_order_type** | **str** | type of the child order | [optional] 
**size_and_fills** | **str** | Format fillQuantity\\totalQuantity | [optional] 
**exit_strategy_display_price** | **str** | Position display price | [optional] 
**exit_strategy_chart_description** | **str** | Position description to display on chart | [optional] 
**exit_strategy_tool_availability** | **str** | * 1: If your account has position or order for contract * 0: If your account has no position or order for contract  | [optional] 
**allowed_duplicate_opposite** | **bool** | Returns true if contract supports duplicate/opposite side order. | [optional] 
**order_time** | **str** | Time of status update in unix time | [optional] 
**oca_group_id** | **str** | only exists for oca orders, oca orders in same group will have same id | [optional] 

## Example

```python
from ibkr_web_api.models.order_status import OrderStatus

# TODO update the JSON string below
json = "{}"
# create an instance of OrderStatus from a JSON string
order_status_instance = OrderStatus.from_json(json)
# print the JSON string representation of the object
print(OrderStatus.to_json())

# convert the object into a dict
order_status_dict = order_status_instance.to_dict()
# create an instance of OrderStatus from a dict
order_status_from_dict = OrderStatus.from_dict(order_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



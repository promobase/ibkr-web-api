# Trade


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**execution_id** | **str** | execution identifier for the order | [optional] 
**symbol** | **str** | Underlying Symbol | [optional] 
**side** | **str** | The side of the market of the order.   * B - Buy contract near posted ask price   * S - Sell contract near posted bid price   * X - Option expired  | [optional] 
**order_description** | **str** | Formatted description of the order \&quot;%side% %size% @ %price% on %exchange%\&quot;. | [optional] 
**trade_time** | **str** | Time of Status update in format \&quot;YYYYMMDD-hh:mm:ss\&quot;. | [optional] 
**trade_time_r** | **float** | Time of status update in format unix time. | [optional] 
**size** | **str** | Quantity of the order | [optional] 
**price** | **str** | Average Price | [optional] 
**order_ref** | **str** | User defined string used to identify the order. Value is set using \&quot;cOID\&quot; field while placing an order. | [optional] 
**submitter** | **str** | User that submitted order | [optional] 
**exchange** | **str** | Exchange or venue of order | [optional] 
**commission** | **float** | Commission of the order | [optional] 
**net_amount** | **float** | Net cost of the order, including contract multiplier and quantity. | [optional] 
**account** | **str** | accountCode | [optional] 
**acount_code** | **str** | Account Number | [optional] 
**company_name** | **str** | Contracts company name | [optional] 
**contract_description_1** | **str** | Format contract name | [optional] 
**sec_type** | **str** | Asset class | [optional] 
**conid** | **str** | IBKR&#39;s contract identifier | [optional] 
**conidex** | **str** | conid and exchange. Format supports conid or conid@exchange | [optional] 
**position** | **str** | Total quantity owned for this contract | [optional] 
**clearing_id** | **str** | Firm which will settle the trade. For IBExecution customers only. | [optional] 
**clearing_name** | **str** | Specifies the true beneficiary of the order. For IBExecution customers only. | [optional] 
**liquidation_trade** | **float** | If order adds liquidity to the market. | [optional] 

## Example

```python
from ibkr_web_api.models.trade import Trade

# TODO update the JSON string below
json = "{}"
# create an instance of Trade from a JSON string
trade_instance = Trade.from_json(json)
# print the JSON string representation of the object
print(Trade.to_json())

# convert the object into a dict
trade_dict = trade_instance.to_dict()
# create an instance of Trade from a dict
trade_from_dict = Trade.from_dict(trade_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



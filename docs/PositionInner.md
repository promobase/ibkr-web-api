# PositionInner

Account Information

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**acct_id** | **str** |  | [optional] 
**conid** | **int** |  | [optional] 
**contract_desc** | **str** |  | [optional] 
**asset_class** | **str** |  | [optional] 
**position** | **float** |  | [optional] 
**mkt_price** | **float** |  | [optional] 
**mkt_value** | **float** |  | [optional] 
**currency** | **str** |  | [optional] 
**avg_cost** | **float** |  | [optional] 
**avg_price** | **float** |  | [optional] 
**realized_pnl** | **float** |  | [optional] 
**unrealized_pnl** | **float** |  | [optional] 
**exchs** | **str** |  | [optional] 
**expiry** | **str** |  | [optional] 
**put_or_call** | **str** |  | [optional] 
**multiplier** | **float** |  | [optional] 
**strike** | **float** |  | [optional] 
**exercise_style** | **str** |  | [optional] 
**und_conid** | **int** |  | [optional] 
**con_exch_map** | **List[str]** |  | [optional] 
**base_mkt_value** | **float** |  | [optional] 
**base_mkt_price** | **float** |  | [optional] 
**base_avg_cost** | **float** |  | [optional] 
**base_avg_price** | **float** |  | [optional] 
**base_realized_pnl** | **float** |  | [optional] 
**base_unrealized_pnl** | **float** |  | [optional] 
**name** | **str** |  | [optional] 
**last_trading_day** | **str** |  | [optional] 
**group** | **str** |  | [optional] 
**sector** | **str** |  | [optional] 
**sector_group** | **str** |  | [optional] 
**ticker** | **str** |  | [optional] 
**und_comp** | **str** |  | [optional] 
**und_sym** | **str** |  | [optional] 
**full_name** | **str** |  | [optional] 
**page_size** | **int** |  | [optional] 
**model** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.position_inner import PositionInner

# TODO update the JSON string below
json = "{}"
# create an instance of PositionInner from a JSON string
position_inner_instance = PositionInner.from_json(json)
# print the JSON string representation of the object
print(PositionInner.to_json())

# convert the object into a dict
position_inner_dict = position_inner_instance.to_dict()
# create an instance of PositionInner from a dict
position_inner_from_dict = PositionInner.from_dict(position_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



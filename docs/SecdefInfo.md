# SecdefInfo

Contains some basic info of contract

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**conid** | **float** | IBKR contract identifier | [optional] 
**symbol** | **str** | Underlying symbol | [optional] 
**sec_type** | **str** | Security type | [optional] 
**exchange** | **str** | Primary Exchange, Routing or Trading Venue | [optional] 
**listing_exchange** | **str** | Main Trading Venue | [optional] 
**right** | **str** | Put or Call of the option. C &#x3D; Call Option, P &#x3D; Put Option | [optional] 
**strike** | **float** | Set price at which a derivative contract can be bought or sold. The strike price also known as exercise price. | [optional] 
**currency** | **str** | Currency the contract trades in | [optional] 
**cusip** | **str** | Committee on Uniform Securities Identification Procedures number | [optional] 
**coupon** | **str** | Annual interest rate paid on a bond | [optional] 
**desc1** | **str** | Currency pairs for Forex e.g. EUR.AUD, EUR.CAD, EUR.CHF etc. | [optional] 
**desc2** | **str** | Formatted expiration, strike and right | [optional] 
**maturity_date** | **float** | Format YYYYMMDD, the date on which the underlying transaction settles if the option is exercised | [optional] 
**multiplier** | **str** | Multiplier for total premium paid or received for derivative contract. | [optional] 
**trading_class** | **str** | Designation of the contract. | [optional] 
**valid_exchanges** | **str** | Comma separated list of exchanges or trading venues. | [optional] 

## Example

```python
from ibkr-web-api.models.secdef_info import SecdefInfo

# TODO update the JSON string below
json = "{}"
# create an instance of SecdefInfo from a JSON string
secdef_info_instance = SecdefInfo.from_json(json)
# print the JSON string representation of the object
print(SecdefInfo.to_json())

# convert the object into a dict
secdef_info_dict = secdef_info_instance.to_dict()
# create an instance of SecdefInfo from a dict
secdef_info_from_dict = SecdefInfo.from_dict(secdef_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



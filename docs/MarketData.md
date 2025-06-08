# MarketData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_31** | **str** | Last Price - The last price at which the contract traded. May contain one of the following prefixes:   * C - Previous day&#39;s closing price.   * H - Trading has halted.  | [optional] 
**var_70** | **float** | High - Current day high price | [optional] 
**var_71** | **float** | Low - Current day low price | [optional] 
**var_82** | **str** | Change - The difference between the last price and the close on the previous trading day | [optional] 
**var_83** | **float** | Change % - The difference between the last price and the close on the previous trading day in percentage. | [optional] 
**var_84** | **str** | Bid Price - The highest-priced bid on the contract. | [optional] 
**var_85** | **str** | Ask Size - The number of contracts or shares offered at the ask price. For US stocks, the number displayed is divided by 100. | [optional] 
**var_86** | **str** | Ask Price - The lowest-priced offer on the contract. | [optional] 
**var_87** | **str** | Volume - Volume for the day, formatted with &#39;K&#39; for thousands or &#39;M&#39; for millions. For higher precision volume refer to field 7762. | [optional] 
**var_88** | **str** | Bid Size - The number of contracts or shares bid for at the bid price. For US stocks, the number displayed is divided by 100. | [optional] 
**var_6509** | **str** | Market Data Availability. The field may contain three chars. First char defines: R &#x3D; RealTime, D &#x3D; Delayed, Z &#x3D; Frozen, Y &#x3D; Frozen Delayed, N &#x3D; Not Subscribed. Second char defines: P &#x3D; Snapshot, p &#x3D; Consolidated. Third char defines: B &#x3D; Book   * RealTime - Data is relayed back in real time without delay, market data subscription(s) are required.   * Delayed - Data is relayed back 15-20 min delayed.   * Frozen - Last recorded data at market close, relayed back in real time.   * Frozen Delayed - Last recorded data at market close, relayed back delayed.   * Not Subscribed - User does not have the required market data subscription(s) to relay back either real time or delayed data.   * Snapshot - Snapshot request is available for contract.   * Consolidated - Market data is aggregated across multiple exchanges or venues.   * Book - Top of the book data is available for contract.  | [optional] 
**var_7057** | **str** | Ask Exch - Displays the exchange(s) offering the SMART price. A&#x3D;AMEX, C&#x3D;CBOE, I&#x3D;ISE, X&#x3D;PHLX, N&#x3D;PSE, B&#x3D;BOX, Q&#x3D;NASDAQOM, Z&#x3D;BATS, W&#x3D;CBOE2, T&#x3D;NASDAQBX, M&#x3D;MIAX, H&#x3D;GEMINI, E&#x3D;EDGX, J&#x3D;MERCURY | [optional] 
**var_7058** | **str** | Last Exch - Displays the exchange(s) offering the SMART price. A&#x3D;AMEX, C&#x3D;CBOE, I&#x3D;ISE, X&#x3D;PHLX, N&#x3D;PSE, B&#x3D;BOX, Q&#x3D;NASDAQOM, Z&#x3D;BATS, W&#x3D;CBOE2, T&#x3D;NASDAQBX, M&#x3D;MIAX, H&#x3D;GEMINI, E&#x3D;EDGX, J&#x3D;MERCURY | [optional] 
**var_7059** | **float** | Last Size - The number of unites traded at the last price | [optional] 
**var_7068** | **str** | Bid Exch - Displays the exchange(s) offering the SMART price. A&#x3D;AMEX, C&#x3D;CBOE, I&#x3D;ISE, X&#x3D;PHLX, N&#x3D;PSE, B&#x3D;BOX, Q&#x3D;NASDAQOM, Z&#x3D;BATS, W&#x3D;CBOE2, T&#x3D;NASDAQBX, M&#x3D;MIAX, H&#x3D;GEMINI, E&#x3D;EDGX, J&#x3D;MERCURY | [optional] 
**var_7195** | **str** | IV Rank | [optional] 
**var_7196** | **str** | IV Rank | [optional] 
**var_7197** | **str** | IV Rank | [optional] 
**var_7198** | **str** | IV Percentile | [optional] 
**var_7199** | **str** | IV Percentile | [optional] 
**var_7200** | **str** | IV Percentile | [optional] 
**var_7201** | **str** | IV High Low | [optional] 
**var_7202** | **str** | IV High Low | [optional] 
**var_7203** | **str** | IV High Low | [optional] 
**var_7204** | **str** | IV High Low | [optional] 
**var_7205** | **str** | IV High Low | [optional] 
**var_7206** | **str** | IV High Low | [optional] 
**var_7207** | **str** | HV Rank | [optional] 
**var_7208** | **str** | HV Rank | [optional] 
**var_7209** | **str** | HV Rank | [optional] 
**var_7210** | **str** | HV Percentile | [optional] 
**var_7211** | **str** | HV Percentile | [optional] 
**var_7212** | **str** | HV Percentile | [optional] 
**var_7245** | **str** | HV High Low | [optional] 
**var_7246** | **str** | HV High Low | [optional] 
**var_7247** | **str** | HV High Low | [optional] 
**var_7248** | **str** | HV High Low | [optional] 
**var_7249** | **str** | HV High Low | [optional] 
**var_7263** | **str** | HV High Low | [optional] 
**var_7264** | **str** | ESG | [optional] 
**var_7265** | **str** | ESG | [optional] 
**var_7266** | **str** | ESG | [optional] 
**var_7267** | **str** | ESG | [optional] 
**var_7268** | **str** | ESG | [optional] 
**var_7269** | **str** | ESG | [optional] 
**var_7271** | **str** | ESG | [optional] 
**var_7272** | **str** | ESG | [optional] 
**var_7273** | **str** | ESG | [optional] 
**var_7274** | **str** | ESG | [optional] 
**var_7275** | **str** | ESG | [optional] 
**var_7276** | **str** | ESG | [optional] 
**var_7277** | **str** | ESG | [optional] 
**var_7282** | **str** | Average Volume - The average daily trading volume over 90 days. | [optional] 
**var_7283** | **str** | Option Implied Vol. % - A prediction of how volatile an underlying will be in the future. At the market volatility estimated for a maturity thirty calendar days forward of the current trading day, and based on option prices from two consecutive expiration months.       | [optional] 
**var_7284** | **str** | Historic Volume (30d) | [optional] 
**var_7286** | **float** | Dividend Amount - Displays the amount of the next dividend. | [optional] 
**var_7287** | **str** | Dividend Yield % - This value is the toal of the expected dividend payments over the next twelve months per share divided by the Current Price and is expressed as a percentage. For derivatives, this displays the total of the expected dividend payments over the expiry date.  | [optional] 
**var_7288** | **str** | Ex-date of the dividend | [optional] 
**var_7289** | **str** | Market Cap | [optional] 
**var_7290** | **str** | P/E | [optional] 
**var_7293** | **str** | 52 Week High - The highest price for the past 52 weeks. | [optional] 
**var_7294** | **str** | 52 Week Low - The lowest price for the past 52 weeks. | [optional] 
**var_7295** | **float** | Open - Today&#39;s opening price. | [optional] 
**var_7296** | **float** | Close - Today&#39;s closing price. | [optional] 
**var_7331** | **str** | Reuters Fundamentals | [optional] 
**var_7370** | **str** | ESG | [optional] 
**var_7371** | **str** | ESG | [optional] 
**var_7372** | **str** | ESG | [optional] 
**var_7635** | **str** | Mark - The mark price is, the ask price if ask is less than last price, the bid price if bid is more than the last price, otherwise it&#39;s equal to last price | [optional] 
**var_7636** | **float** | shortable invetory | [optional] 
**var_7637** | **str** | Fee rebate rate | [optional] 
**var_7644** | **str** | Shortable - Describes the level of difficulty with which the security can be sold short. | [optional] 
**var_7674** | **str** | EMA(200) - Exponential moving average (N&#x3D;200). | [optional] 
**var_7675** | **str** | EMA(100) - Exponential moving average (N&#x3D;100). | [optional] 
**var_7676** | **str** | EMA(50) - Exponential moving average (N&#x3D;50). | [optional] 
**var_7677** | **str** | EMA(20) - Exponential moving average (N&#x3D;20). | [optional] 
**var_7681** | **str** | Price/EMA(20) - Price to Exponential moving average (N&#x3D;20) ratio -1, displayed in percents. | [optional] 
**var_7698** | **str** | Last Yield - Implied yield of the bond if it is purchased at the current last price. Last yield is calculated using the Last price on all possible call dates. It is assumed that prepayment occurs if the bond has call or put provisions and the issuer can offer a lower coupon rate based on current market rates. The yield to worst will be the lowest of the yield to maturity or yield to call (if the bond has prepayment provisions). Yield to worse may be the same as yield to maturity but never higher.  | [optional] 
**var_7699** | **str** | Bid Yield - Implied yield of the bond if it is purchased at the current bid price. Bid yield is calculated using the Ask on all possible call dates. It is assumed that prepayment occurs if the bond has call or put provisions and the issuer can offer a lower coupon rate based on current market rates. The yield to worst will be the lowest of the yield to maturity or yield to call (if the bond has prepayment provisions). Yield to worse may be the same as yield to maturity but never higher.  | [optional] 
**var_7718** | **str** | Beta - Beta is against standard index. | [optional] 
**var_7720** | **str** | Ask Yield - Implied yield of the bond if it is purchased at the current offer. Ask yield is calculated using the Bid on all possible call dates. It is assumed that prepayment occurs if the bond has call or put provisions and the issuer can offer a lower coupon rate based on current market rates. The yield to worst will be the lowest of the yield to maturity or yield to call (if the bond has prepayment provisions). Yield to worse may be the same as yield to maturity but never higher.  | [optional] 
**var_7743** | **str** | Reuters Fundamentals | [optional] 
**var_7761** | **str** | ESG | [optional] 
**var_7992** | **str** | 26 Week High - The highest price for the past 26 weeks. | [optional] 
**var_7993** | **str** | 26 Week Low - The lowest price for the past 26 weeks. | [optional] 
**var_7994** | **str** | 13 Week High - The highest price for the past 13 weeks. | [optional] 
**var_7995** | **str** | 13 Week Low - The lowest price for the past 13 weeks. | [optional] 
**conid** | **int** | IBKR Contract identifier | [optional] 
**min_tick** | **float** | minimum price increment | [optional] 
**bbo_exchange** | **str** | Color for Best Bid/Offer Exchange in hex code | [optional] 
**has_delayed** | **bool** | If market data field values return delayed | [optional] 
**size_min_tick** | **int** | minimum size increment | [optional] 
**best_eligible** | **int** |  | [optional] 
**best_bid_exch** | **int** |  | [optional] 
**best_ask_exch** | **int** |  | [optional] 
**pre_open_bid** | **int** |  | [optional] 
**last_attribs** | **int** |  | [optional] 
**timestamp_base** | **int** | Base time stamp for last update in format YYYYMMDD | [optional] 
**timestamp_delta** | **int** |  | [optional] 
**last_exch** | **int** |  | [optional] 
**close_attribs** | **int** |  | [optional] 

## Example

```python
from ibkr_web_api.models.market_data import MarketData

# TODO update the JSON string below
json = "{}"
# create an instance of MarketData from a JSON string
market_data_instance = MarketData.from_json(json)
# print the JSON string representation of the object
print(MarketData.to_json())

# convert the object into a dict
market_data_dict = market_data_instance.to_dict()
# create an instance of MarketData from a dict
market_data_from_dict = MarketData.from_dict(market_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



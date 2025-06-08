# ibkr_web_api.MarketDataApi

All URIs are relative to *http://localhost:5000/v1/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**hmds_history_get**](MarketDataApi.md#hmds_history_get) | **GET** /hmds/history | Market Data History (Beta)
[**iserver_marketdata_conid_unsubscribe_get**](MarketDataApi.md#iserver_marketdata_conid_unsubscribe_get) | **GET** /iserver/marketdata/{conid}/unsubscribe | Market Data Cancel (Single)
[**iserver_marketdata_history_get**](MarketDataApi.md#iserver_marketdata_history_get) | **GET** /iserver/marketdata/history | Market Data History
[**iserver_marketdata_snapshot_get**](MarketDataApi.md#iserver_marketdata_snapshot_get) | **GET** /iserver/marketdata/snapshot | Market Data
[**iserver_marketdata_unsubscribeall_get**](MarketDataApi.md#iserver_marketdata_unsubscribeall_get) | **GET** /iserver/marketdata/unsubscribeall | Market Data Cancel (All)
[**md_snapshot_get**](MarketDataApi.md#md_snapshot_get) | **GET** /md/snapshot | Market Data Snapshot (Beta)


# **hmds_history_get**
> HistoryResult hmds_history_get(conid, period, bar=bar, outside_rth=outside_rth)

Market Data History (Beta)

Using a direct connection to the market data farm, will provide a list of historical market data for given conid.

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.history_result import HistoryResult
from ibkr_web_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = ibkr_web_api.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with ibkr_web_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ibkr_web_api.MarketDataApi(api_client)
    conid = 56 # int | contract id
    period = 'period_example' # str | Time period for history request.    * min: Minutes   * h: Hours   * d: Days   * w: Weeks   * m: Months   * y: Years 
    bar = 'bar_example' # str | Duration of time for each candlestick bar.   * min: Minutes   * h: Hours   * d: Days   * w: Weeks   * m: Months  (optional)
    outside_rth = True # bool | For contracts that support it, will determine if history data includes outside of regular trading hours. (optional)

    try:
        # Market Data History (Beta)
        api_response = api_instance.hmds_history_get(conid, period, bar=bar, outside_rth=outside_rth)
        print("The response of MarketDataApi->hmds_history_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketDataApi->hmds_history_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conid** | **int**| contract id | 
 **period** | **str**| Time period for history request.    * min: Minutes   * h: Hours   * d: Days   * w: Weeks   * m: Months   * y: Years  | 
 **bar** | **str**| Duration of time for each candlestick bar.   * min: Minutes   * h: Hours   * d: Days   * w: Weeks   * m: Months  | [optional] 
 **outside_rth** | **bool**| For contracts that support it, will determine if history data includes outside of regular trading hours. | [optional] 

### Return type

[**HistoryResult**](HistoryResult.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Bad request |  -  |
**200** | Valid result |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **iserver_marketdata_conid_unsubscribe_get**
> IserverMarketdataConidUnsubscribeGet200Response iserver_marketdata_conid_unsubscribe_get(conid)

Market Data Cancel (Single)

Cancel market data for given conid. To cancel all market data request(s), see /iserver/marketdata/unsubscribeall.


### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_marketdata_conid_unsubscribe_get200_response import IserverMarketdataConidUnsubscribeGet200Response
from ibkr_web_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = ibkr_web_api.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with ibkr_web_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ibkr_web_api.MarketDataApi(api_client)
    conid = 'conid_example' # str | contract id

    try:
        # Market Data Cancel (Single)
        api_response = api_instance.iserver_marketdata_conid_unsubscribe_get(conid)
        print("The response of MarketDataApi->iserver_marketdata_conid_unsubscribe_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketDataApi->iserver_marketdata_conid_unsubscribe_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conid** | **str**| contract id | 

### Return type

[**IserverMarketdataConidUnsubscribeGet200Response**](IserverMarketdataConidUnsubscribeGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**500** | cancel failed |  -  |
**200** | confirms market data for conid is cancelled |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **iserver_marketdata_history_get**
> HistoryData iserver_marketdata_history_get(conid, period, exchange=exchange, bar=bar, outside_rth=outside_rth)

Market Data History

Get historical market Data for given conid, length of data is controlled by 'period' and 'bar'.
Formatted as: min=minute, h=hour, d=day, w=week, m=month, y=year
e.g. period =1y with bar =1w returns 52 data points (Max of 1000 data points supported).
**Note**: There's a limit of 5 concurrent requests. Excessive requests will return a 'Too many requests' status 429 response.


### Example


```python
import ibkr_web_api
from ibkr_web_api.models.history_data import HistoryData
from ibkr_web_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = ibkr_web_api.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with ibkr_web_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ibkr_web_api.MarketDataApi(api_client)
    conid = 'conid_example' # str | contract id
    period = 'period_example' # str | available time period-- {1-30}min, {1-8}h, {1-1000}d, {1-792}w, {1-182}m, {1-15}y
    exchange = 'exchange_example' # str | Exchange of the conid (e.g. ISLAND, NYSE, etc.). Default value is empty which corresponds to primary exchange of the conid. (optional)
    bar = 'bar_example' # str | possible value-- 1min, 2min, 3min, 5min, 10min, 15min, 30min, 1h, 2h, 3h, 4h, 8h, 1d, 1w, 1m (optional)
    outside_rth = True # bool | For contracts that support it, will determine if historical data includes outside of regular trading hours. (optional)

    try:
        # Market Data History
        api_response = api_instance.iserver_marketdata_history_get(conid, period, exchange=exchange, bar=bar, outside_rth=outside_rth)
        print("The response of MarketDataApi->iserver_marketdata_history_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketDataApi->iserver_marketdata_history_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conid** | **str**| contract id | 
 **period** | **str**| available time period-- {1-30}min, {1-8}h, {1-1000}d, {1-792}w, {1-182}m, {1-15}y | 
 **exchange** | **str**| Exchange of the conid (e.g. ISLAND, NYSE, etc.). Default value is empty which corresponds to primary exchange of the conid. | [optional] 
 **bar** | **str**| possible value-- 1min, 2min, 3min, 5min, 10min, 15min, 30min, 1h, 2h, 3h, 4h, 8h, 1d, 1w, 1m | [optional] 
 **outside_rth** | **bool**| For contracts that support it, will determine if historical data includes outside of regular trading hours. | [optional] 

### Return type

[**HistoryData**](HistoryData.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Returns an object |  -  |
**429** | Too many requests |  -  |
**500** | System Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **iserver_marketdata_snapshot_get**
> List[IserverMarketdataSnapshotGet200ResponseInner] iserver_marketdata_snapshot_get(conids, since=since, fields=fields)

Market Data

Get Market Data for the given conid(s). The endpoint will return by default bid, ask, last, change, change pct, close, listing exchange.
See response fields for a list of available fields that can be request via fields argument.
The endpoint /iserver/accounts must be called prior to /iserver/marketdata/snapshot.
For derivative contracts the endpoint /iserver/secdef/search must be called first.
First /snapshot endpoint call for given conid will initiate the market data request. 
To receive all available fields the /snapshot endpoint will need to be called several times.
To receive streaming market data the endpoint /ws can be used. Refer to [Streaming WebSocket Data](https://interactivebrokers.github.io/cpwebapi/RealtimeSubscription.html) for details.


### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_marketdata_snapshot_get200_response_inner import IserverMarketdataSnapshotGet200ResponseInner
from ibkr_web_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = ibkr_web_api.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with ibkr_web_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ibkr_web_api.MarketDataApi(api_client)
    conids = 'conids_example' # str | list of conids separated by comma
    since = 56 # int | time period since which updates are required. uses epoch time with milliseconds. (optional)
    fields = 'fields_example' # str | list of fields separated by comma (optional)

    try:
        # Market Data
        api_response = api_instance.iserver_marketdata_snapshot_get(conids, since=since, fields=fields)
        print("The response of MarketDataApi->iserver_marketdata_snapshot_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketDataApi->iserver_marketdata_snapshot_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conids** | **str**| list of conids separated by comma | 
 **since** | **int**| time period since which updates are required. uses epoch time with milliseconds. | [optional] 
 **fields** | **str**| list of fields separated by comma | [optional] 

### Return type

[**List[IserverMarketdataSnapshotGet200ResponseInner]**](IserverMarketdataSnapshotGet200ResponseInner.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Returns an array of objects |  -  |
**400** | sent when accounts are not queried before sending this request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **iserver_marketdata_unsubscribeall_get**
> IserverMarketdataUnsubscribeallGet200Response iserver_marketdata_unsubscribeall_get()

Market Data Cancel (All)

Cancel all market data request(s). To cancel market data for given conid, see /iserver/marketdata/{conid}/unsubscribe.


### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_marketdata_unsubscribeall_get200_response import IserverMarketdataUnsubscribeallGet200Response
from ibkr_web_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = ibkr_web_api.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with ibkr_web_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ibkr_web_api.MarketDataApi(api_client)

    try:
        # Market Data Cancel (All)
        api_response = api_instance.iserver_marketdata_unsubscribeall_get()
        print("The response of MarketDataApi->iserver_marketdata_unsubscribeall_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketDataApi->iserver_marketdata_unsubscribeall_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**IserverMarketdataUnsubscribeallGet200Response**](IserverMarketdataUnsubscribeallGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | confirms market data is cancelled |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **md_snapshot_get**
> MarketData md_snapshot_get(conids, fields=fields)

Market Data Snapshot (Beta)

Get a snapshot of Market Data for the given conid(s).See response for a list of available fields that can be requested from the fields argument.
Must be connected to a brokerage session before can query snapshot data.
First /snapshot endpoint call for given conid(s) will initiate the market data request, make an additional request to receive field values back.
To receive all available fields the /snapshot endpoint will need to be called several times.
To receive streaming market data the endpoint /ws can be used. Refer to [Streaming WebSocket Data](https://interactivebrokers.github.io/cpwebapi/RealtimeSubscription.html) for details.


### Example


```python
import ibkr_web_api
from ibkr_web_api.models.market_data import MarketData
from ibkr_web_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = ibkr_web_api.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with ibkr_web_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ibkr_web_api.MarketDataApi(api_client)
    conids = 'conids_example' # str | List of conids comma separated. Optional exchange and instrument type can be specified.   * conid: IBKR Contract Identifier   * exchange: Exchange or venue   * instrType: Instrument Type supported values: CS (Stocks), OPT (Options), FUT (Futures), FOP (Future Options), WAR (Warrants), BOND (Bonds), FUND (Mutual Funds), CASH (Forex), CFD (Contract for difference), IND (Index) 
    fields = 'fields_example' # str | list of fields separated by comma (optional)

    try:
        # Market Data Snapshot (Beta)
        api_response = api_instance.md_snapshot_get(conids, fields=fields)
        print("The response of MarketDataApi->md_snapshot_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketDataApi->md_snapshot_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conids** | **str**| List of conids comma separated. Optional exchange and instrument type can be specified.   * conid: IBKR Contract Identifier   * exchange: Exchange or venue   * instrType: Instrument Type supported values: CS (Stocks), OPT (Options), FUT (Futures), FOP (Future Options), WAR (Warrants), BOND (Bonds), FUND (Mutual Funds), CASH (Forex), CFD (Contract for difference), IND (Index)  | 
 **fields** | **str**| list of fields separated by comma | [optional] 

### Return type

[**MarketData**](MarketData.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**500** | System failed |  -  |
**401** | Authentication failed |  -  |
**200** | An Object |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


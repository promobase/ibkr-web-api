# ibkr_web_api.ContractApi

All URIs are relative to *http://localhost:5000/v1/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**iserver_contract_conid_algos_get**](ContractApi.md#iserver_contract_conid_algos_get) | **GET** /iserver/contract/{conid}/algos | IB Algo Params
[**iserver_contract_conid_info_and_rules_get**](ContractApi.md#iserver_contract_conid_info_and_rules_get) | **GET** /iserver/contract/{conid}/info-and-rules | Info and Rules
[**iserver_contract_conid_info_get**](ContractApi.md#iserver_contract_conid_info_get) | **GET** /iserver/contract/{conid}/info | Contract Details
[**iserver_contract_rules_post**](ContractApi.md#iserver_contract_rules_post) | **POST** /iserver/contract/rules | Contract Rules
[**iserver_secdef_info_get**](ContractApi.md#iserver_secdef_info_get) | **GET** /iserver/secdef/info | Secdef Info
[**iserver_secdef_search_post**](ContractApi.md#iserver_secdef_search_post) | **POST** /iserver/secdef/search | Search by Symbol or Name
[**iserver_secdef_strikes_get**](ContractApi.md#iserver_secdef_strikes_get) | **GET** /iserver/secdef/strikes | Search Strikes
[**trsrv_futures_get**](ContractApi.md#trsrv_futures_get) | **GET** /trsrv/futures | Security Futures by Symbol
[**trsrv_secdef_post**](ContractApi.md#trsrv_secdef_post) | **POST** /trsrv/secdef | Secdef by Conid
[**trsrv_secdef_schedule_get**](ContractApi.md#trsrv_secdef_schedule_get) | **GET** /trsrv/secdef/schedule | Get trading schedule for symbol
[**trsrv_stocks_get**](ContractApi.md#trsrv_stocks_get) | **GET** /trsrv/stocks | Security Stocks by Symbol


# **iserver_contract_conid_algos_get**
> List[IserverContractConidAlgosGet200ResponseInner] iserver_contract_conid_algos_get(conid, algos=algos, add_description=add_description, add_params=add_params)

IB Algo Params

Returns supported IB Algos for contract. Must be called a second time to query the list of available parameters.

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_contract_conid_algos_get200_response_inner import IserverContractConidAlgosGet200ResponseInner
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
    api_instance = ibkr_web_api.ContractApi(api_client)
    conid = 'conid_example' # str | IBKR contract identifier
    algos = 'algos_example' # str | List of algo ids delimited by \";\" to filter by. Max of 8 algos ids can be specified. (optional)
    add_description = 'add_description_example' # str | Whether or not to add algo descriptions to response. Set to 1 for yes, 0 for no. (optional)
    add_params = 'add_params_example' # str | Whether or not to show algo parameters.  Set to 1 for yes, 0 for no. (optional)

    try:
        # IB Algo Params
        api_response = api_instance.iserver_contract_conid_algos_get(conid, algos=algos, add_description=add_description, add_params=add_params)
        print("The response of ContractApi->iserver_contract_conid_algos_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContractApi->iserver_contract_conid_algos_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conid** | **str**| IBKR contract identifier | 
 **algos** | **str**| List of algo ids delimited by \&quot;;\&quot; to filter by. Max of 8 algos ids can be specified. | [optional] 
 **add_description** | **str**| Whether or not to add algo descriptions to response. Set to 1 for yes, 0 for no. | [optional] 
 **add_params** | **str**| Whether or not to show algo parameters.  Set to 1 for yes, 0 for no. | [optional] 

### Return type

[**List[IserverContractConidAlgosGet200ResponseInner]**](IserverContractConidAlgosGet200ResponseInner.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns an array of algos |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **iserver_contract_conid_info_and_rules_get**
> IserverContractConidInfoAndRulesGet200Response iserver_contract_conid_info_and_rules_get(conid, is_buy)

Info and Rules

Returns both contract info and rules from a single endpoint.
For only contract rules, use the endpoint /iserver/contract/rules.
For only contract info, use the endpoint /iserver/contract/{conid}/info. 


### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_contract_conid_info_and_rules_get200_response import IserverContractConidInfoAndRulesGet200Response
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
    api_instance = ibkr_web_api.ContractApi(api_client)
    conid = 'conid_example' # str | IBKR contract identifier
    is_buy = True # bool | Side of the market rules apply too. Set to **true** for Buy Orders, set to **false** for Sell Orders

    try:
        # Info and Rules
        api_response = api_instance.iserver_contract_conid_info_and_rules_get(conid, is_buy)
        print("The response of ContractApi->iserver_contract_conid_info_and_rules_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContractApi->iserver_contract_conid_info_and_rules_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conid** | **str**| IBKR contract identifier | 
 **is_buy** | **bool**| Side of the market rules apply too. Set to **true** for Buy Orders, set to **false** for Sell Orders | 

### Return type

[**IserverContractConidInfoAndRulesGet200Response**](IserverContractConidInfoAndRulesGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns an array |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **iserver_contract_conid_info_get**
> Contract iserver_contract_conid_info_get(conid)

Contract Details

Using the Contract Identifier get contract info. You can use this to prefill your order before you submit an order

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.contract import Contract
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
    api_instance = ibkr_web_api.ContractApi(api_client)
    conid = 'conid_example' # str | contract id

    try:
        # Contract Details
        api_response = api_instance.iserver_contract_conid_info_get(conid)
        print("The response of ContractApi->iserver_contract_conid_info_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContractApi->iserver_contract_conid_info_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conid** | **str**| contract id | 

### Return type

[**Contract**](Contract.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns an object |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **iserver_contract_rules_post**
> IserverContractRulesPost200Response iserver_contract_rules_post(conid)

Contract Rules

Returns trading related rules for a specific contract and side. For both contract info and rules use the endpoint /iserver/contract/{conid}/info-and-rules.

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_contract_rules_post200_response import IserverContractRulesPost200Response
from ibkr_web_api.models.iserver_contract_rules_post_request import IserverContractRulesPostRequest
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
    api_instance = ibkr_web_api.ContractApi(api_client)
    conid = ibkr_web_api.IserverContractRulesPostRequest() # IserverContractRulesPostRequest | 

    try:
        # Contract Rules
        api_response = api_instance.iserver_contract_rules_post(conid)
        print("The response of ContractApi->iserver_contract_rules_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContractApi->iserver_contract_rules_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conid** | [**IserverContractRulesPostRequest**](IserverContractRulesPostRequest.md)|  | 

### Return type

[**IserverContractRulesPost200Response**](IserverContractRulesPost200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns an array |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **iserver_secdef_info_get**
> List[SecdefInfo] iserver_secdef_info_get(conid, sectype, month=month, exchange=exchange, strike=strike, right=right)

Secdef Info

Provides Contract Details of Futures, Options, Warrants, Cash and CFDs based on conid. To get the strike price for Options/Warrants use "/iserver/secdef/strikes" endpoint. Must call /secdef/search for the underlying contract first.

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.secdef_info import SecdefInfo
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
    api_instance = ibkr_web_api.ContractApi(api_client)
    conid = 'conid_example' # str | underlying contract id
    sectype = 'sectype_example' # str | FUT/OPT/WAR/CASH/CFD
    month = 'month_example' # str | contract month, only required for FUT/OPT/WAR in the format MMMYY, example JAN00 (optional)
    exchange = 'exchange_example' # str | optional, default is SMART (optional)
    strike = 3.4 # float | optional, only required for OPT/WAR (optional)
    right = 'right_example' # str | C for call, P for put (optional)

    try:
        # Secdef Info
        api_response = api_instance.iserver_secdef_info_get(conid, sectype, month=month, exchange=exchange, strike=strike, right=right)
        print("The response of ContractApi->iserver_secdef_info_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContractApi->iserver_secdef_info_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conid** | **str**| underlying contract id | 
 **sectype** | **str**| FUT/OPT/WAR/CASH/CFD | 
 **month** | **str**| contract month, only required for FUT/OPT/WAR in the format MMMYY, example JAN00 | [optional] 
 **exchange** | **str**| optional, default is SMART | [optional] 
 **strike** | **float**| optional, only required for OPT/WAR | [optional] 
 **right** | **str**| C for call, P for put | [optional] 

### Return type

[**List[SecdefInfo]**](SecdefInfo.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns an array of objects |  -  |
**500** | error while processing the request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **iserver_secdef_search_post**
> List[IserverSecdefSearchPost200ResponseInner] iserver_secdef_search_post(symbol)

Search by Symbol or Name

Search by underlying symbol or company name. Relays back what derivative contract(s) it has. This endpoint must be called before using /secdef/info.
If company name is specified will only receive limited response: conid, companyName, companyHeader and symbol.


### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_secdef_search_post200_response_inner import IserverSecdefSearchPost200ResponseInner
from ibkr_web_api.models.iserver_secdef_search_post_request import IserverSecdefSearchPostRequest
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
    api_instance = ibkr_web_api.ContractApi(api_client)
    symbol = ibkr_web_api.IserverSecdefSearchPostRequest() # IserverSecdefSearchPostRequest | Symbol or Company Name to be searched

    try:
        # Search by Symbol or Name
        api_response = api_instance.iserver_secdef_search_post(symbol)
        print("The response of ContractApi->iserver_secdef_search_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContractApi->iserver_secdef_search_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **symbol** | [**IserverSecdefSearchPostRequest**](IserverSecdefSearchPostRequest.md)| Symbol or Company Name to be searched | 

### Return type

[**List[IserverSecdefSearchPost200ResponseInner]**](IserverSecdefSearchPost200ResponseInner.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns an array of results |  -  |
**500** | error while processing the request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **iserver_secdef_strikes_get**
> IserverSecdefStrikesGet200Response iserver_secdef_strikes_get(conid, sectype, month, exchange=exchange)

Search Strikes

Query strikes for Options/Warrants. For the conid of the underlying contract, available contract months and exchanges use "/iserver/secdef/search"

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_secdef_strikes_get200_response import IserverSecdefStrikesGet200Response
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
    api_instance = ibkr_web_api.ContractApi(api_client)
    conid = 'conid_example' # str | contract id of the underlying contract
    sectype = 'sectype_example' # str | OPT/WAR
    month = 'month_example' # str | contract month
    exchange = 'exchange_example' # str | optional, default is SMART (optional)

    try:
        # Search Strikes
        api_response = api_instance.iserver_secdef_strikes_get(conid, sectype, month, exchange=exchange)
        print("The response of ContractApi->iserver_secdef_strikes_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContractApi->iserver_secdef_strikes_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conid** | **str**| contract id of the underlying contract | 
 **sectype** | **str**| OPT/WAR | 
 **month** | **str**| contract month | 
 **exchange** | **str**| optional, default is SMART | [optional] 

### Return type

[**IserverSecdefStrikesGet200Response**](IserverSecdefStrikesGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns an object contains call/put strike prices |  -  |
**500** | error while processing the request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **trsrv_futures_get**
> TrsrvFuturesGet200Response trsrv_futures_get(symbols)

Security Futures by Symbol

Returns a list of non-expired future contracts for given symbol(s)

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.trsrv_futures_get200_response import TrsrvFuturesGet200Response
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
    api_instance = ibkr_web_api.ContractApi(api_client)
    symbols = 'symbols_example' # str | list of case-sensitive symbols separated by comma

    try:
        # Security Futures by Symbol
        api_response = api_instance.trsrv_futures_get(symbols)
        print("The response of ContractApi->trsrv_futures_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContractApi->trsrv_futures_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **symbols** | **str**| list of case-sensitive symbols separated by comma | 

### Return type

[**TrsrvFuturesGet200Response**](TrsrvFuturesGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns an object with symbol and and array of its future contracts |  -  |
**500** | error while processing the request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **trsrv_secdef_post**
> List[SecdefInner] trsrv_secdef_post(body)

Secdef by Conid

Returns a list of security definitions for the given conids

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.secdef_inner import SecdefInner
from ibkr_web_api.models.trsrv_secdef_post_request import TrsrvSecdefPostRequest
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
    api_instance = ibkr_web_api.ContractApi(api_client)
    body = ibkr_web_api.TrsrvSecdefPostRequest() # TrsrvSecdefPostRequest | request body

    try:
        # Secdef by Conid
        api_response = api_instance.trsrv_secdef_post(body)
        print("The response of ContractApi->trsrv_secdef_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContractApi->trsrv_secdef_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**TrsrvSecdefPostRequest**](TrsrvSecdefPostRequest.md)| request body | 

### Return type

[**List[SecdefInner]**](SecdefInner.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns an array of secdef info |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **trsrv_secdef_schedule_get**
> TrsrvSecdefScheduleGet200Response trsrv_secdef_schedule_get(asset_class, symbol, exchange=exchange, exchange_filter=exchange_filter)

Get trading schedule for symbol

Returns the trading schedule up to a month for the requested contract

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.trsrv_secdef_schedule_get200_response import TrsrvSecdefScheduleGet200Response
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
    api_instance = ibkr_web_api.ContractApi(api_client)
    asset_class = 'asset_class_example' # str | specify the asset class of the contract. Available values-- Stock: STK, Option: OPT, Future: FUT, Contract For Difference: CFD, Warrant: WAR, Forex: SWP, Mutual Fund: FND, Bond: BND, Inter-Commodity Spreads: ICS 
    symbol = 'symbol_example' # str | Underlying Symbol for specified contract, for example 'AAPL' for US Stock - Apple Inc.
    exchange = 'exchange_example' # str | Native exchange for contract, for example 'NASDAQ' for US Stock - Apple Inc. (optional)
    exchange_filter = 'exchange_filter_example' # str | Response only returns trading schedule for specified exchange (optional)

    try:
        # Get trading schedule for symbol
        api_response = api_instance.trsrv_secdef_schedule_get(asset_class, symbol, exchange=exchange, exchange_filter=exchange_filter)
        print("The response of ContractApi->trsrv_secdef_schedule_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContractApi->trsrv_secdef_schedule_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **asset_class** | **str**| specify the asset class of the contract. Available values-- Stock: STK, Option: OPT, Future: FUT, Contract For Difference: CFD, Warrant: WAR, Forex: SWP, Mutual Fund: FND, Bond: BND, Inter-Commodity Spreads: ICS  | 
 **symbol** | **str**| Underlying Symbol for specified contract, for example &#39;AAPL&#39; for US Stock - Apple Inc. | 
 **exchange** | **str**| Native exchange for contract, for example &#39;NASDAQ&#39; for US Stock - Apple Inc. | [optional] 
 **exchange_filter** | **str**| Response only returns trading schedule for specified exchange | [optional] 

### Return type

[**TrsrvSecdefScheduleGet200Response**](TrsrvSecdefScheduleGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Returns an object |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **trsrv_stocks_get**
> TrsrvStocksGet200Response trsrv_stocks_get(symbols)

Security Stocks by Symbol

Returns an object contains all stock contracts for given symbol(s)

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.trsrv_stocks_get200_response import TrsrvStocksGet200Response
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
    api_instance = ibkr_web_api.ContractApi(api_client)
    symbols = 'symbols_example' # str | list of upper-sensitive symbols separated by comma

    try:
        # Security Stocks by Symbol
        api_response = api_instance.trsrv_stocks_get(symbols)
        print("The response of ContractApi->trsrv_stocks_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContractApi->trsrv_stocks_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **symbols** | **str**| list of upper-sensitive symbols separated by comma | 

### Return type

[**TrsrvStocksGet200Response**](TrsrvStocksGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns an object with symbols |  -  |
**500** | error while processing the request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


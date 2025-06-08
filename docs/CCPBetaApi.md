# ibkr-web-api.CCPBetaApi

All URIs are relative to *http://localhost:5000/v1/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ccp_account_get**](CCPBetaApi.md#ccp_account_get) | **GET** /ccp/account | Brokerage Accounts
[**ccp_auth_init_post**](CCPBetaApi.md#ccp_auth_init_post) | **POST** /ccp/auth/init | Start CCP Session
[**ccp_auth_response_post**](CCPBetaApi.md#ccp_auth_response_post) | **POST** /ccp/auth/response | Complete CCP Session
[**ccp_order_delete**](CCPBetaApi.md#ccp_order_delete) | **DELETE** /ccp/order | Delete Order
[**ccp_order_post**](CCPBetaApi.md#ccp_order_post) | **POST** /ccp/order | Submit Order
[**ccp_order_put**](CCPBetaApi.md#ccp_order_put) | **PUT** /ccp/order | Update Order
[**ccp_orders_get**](CCPBetaApi.md#ccp_orders_get) | **GET** /ccp/orders | Order Status
[**ccp_positions_get**](CCPBetaApi.md#ccp_positions_get) | **GET** /ccp/positions | Positions
[**ccp_status_get**](CCPBetaApi.md#ccp_status_get) | **GET** /ccp/status | CCP Status
[**ccp_trades_get**](CCPBetaApi.md#ccp_trades_get) | **GET** /ccp/trades | Trades


# **ccp_account_get**
> CcpAccountGet200Response ccp_account_get()

Brokerage Accounts

Provides the list of tradeable accounts

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.ccp_account_get200_response import CcpAccountGet200Response
from ibkr-web-api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = ibkr-web-api.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with ibkr-web-api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ibkr-web-api.CCPBetaApi(api_client)

    try:
        # Brokerage Accounts
        api_response = api_instance.ccp_account_get()
        print("The response of CCPBetaApi->ccp_account_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CCPBetaApi->ccp_account_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**CcpAccountGet200Response**](CcpAccountGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | An array of accounts |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ccp_auth_init_post**
> CcpAuthInitPost200Response ccp_auth_init_post(compete=compete, locale=locale, mac=mac, machine_id=machine_id, username=username)

Start CCP Session

Initiate a brokerage session to CCP. Only one brokerage session type can run at a time. If an existing brokerage session to iServer is running then call the endpoint /logout first. Note at this time only order management is possible from CCP session, market data and scanner endpoints can't be used since they are only available from iServer session. Work is in progress to provide new CCP endpoints for market data and scanners.

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.ccp_auth_init_post200_response import CcpAuthInitPost200Response
from ibkr-web-api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = ibkr-web-api.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with ibkr-web-api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ibkr-web-api.CCPBetaApi(api_client)
    compete = True # bool | Allow competing CCP session to run (optional)
    locale = 'locale_example' # str | Concatenate value for language and region, set to \\\"en_US\\\" (optional)
    mac = 'mac_example' # str | Local MAC Address (optional)
    machine_id = 'machine_id_example' # str | Local machine ID (optional)
    username = 'username_example' # str | Login user, set to dash \\\"-\\\" (optional)

    try:
        # Start CCP Session
        api_response = api_instance.ccp_auth_init_post(compete=compete, locale=locale, mac=mac, machine_id=machine_id, username=username)
        print("The response of CCPBetaApi->ccp_auth_init_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CCPBetaApi->ccp_auth_init_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **compete** | **bool**| Allow competing CCP session to run | [optional] 
 **locale** | **str**| Concatenate value for language and region, set to \\\&quot;en_US\\\&quot; | [optional] 
 **mac** | **str**| Local MAC Address | [optional] 
 **machine_id** | **str**| Local machine ID | [optional] 
 **username** | **str**| Login user, set to dash \\\&quot;-\\\&quot; | [optional] 

### Return type

[**CcpAuthInitPost200Response**](CcpAuthInitPost200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**500** | System error |  -  |
**401** | Access denied |  -  |
**200** | Returns challenge for connection |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ccp_auth_response_post**
> CcpAuthResponsePost200Response ccp_auth_response_post(auth=auth)

Complete CCP Session

Session Token Authentication

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.ccp_auth_response_post200_response import CcpAuthResponsePost200Response
from ibkr-web-api.models.ccp_auth_response_post_request import CcpAuthResponsePostRequest
from ibkr-web-api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = ibkr-web-api.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with ibkr-web-api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ibkr-web-api.CCPBetaApi(api_client)
    auth = ibkr-web-api.CcpAuthResponsePostRequest() # CcpAuthResponsePostRequest |  (optional)

    try:
        # Complete CCP Session
        api_response = api_instance.ccp_auth_response_post(auth=auth)
        print("The response of CCPBetaApi->ccp_auth_response_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CCPBetaApi->ccp_auth_response_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **auth** | [**CcpAuthResponsePostRequest**](CcpAuthResponsePostRequest.md)|  | [optional] 

### Return type

[**CcpAuthResponsePost200Response**](CcpAuthResponsePost200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**500** | System error |  -  |
**401** | Access denied |  -  |
**200** | Valid result |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ccp_order_delete**
> OrderData ccp_order_delete(acct, id)

Delete Order

Sends an Order cancellation request. The status of the order can be queried through /ccp/order. Passing arguments as GET is also supported (requires passing action=delete) (GET is meant for development only)


### Example


```python
import ibkr-web-api
from ibkr-web-api.models.order_data import OrderData
from ibkr-web-api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = ibkr-web-api.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with ibkr-web-api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ibkr-web-api.CCPBetaApi(api_client)
    acct = 'acct_example' # str | Account Number
    id = 3.4 # float | Order Identifier of original submit order

    try:
        # Delete Order
        api_response = api_instance.ccp_order_delete(acct, id)
        print("The response of CCPBetaApi->ccp_order_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CCPBetaApi->ccp_order_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **acct** | **str**| Account Number | 
 **id** | **float**| Order Identifier of original submit order | 

### Return type

[**OrderData**](OrderData.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**500** | System error, for example when connection to CCP failed |  -  |
**401** | Access denied |  -  |
**200** | An Object |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ccp_order_post**
> OrderData ccp_order_post(acct, conid, ccy, exchange, qty, type=type, side=side, price=price, tif=tif)

Submit Order

Submits an Order.


### Example


```python
import ibkr-web-api
from ibkr-web-api.models.order_data import OrderData
from ibkr-web-api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = ibkr-web-api.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with ibkr-web-api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ibkr-web-api.CCPBetaApi(api_client)
    acct = 'acct_example' # str | User Account
    conid = 3.4 # float | Contract identifier from IBKR's database.
    ccy = 'ccy_example' # str | Contract Currency
    exchange = 'exchange_example' # str | Exchange
    qty = 3.4 # float | Order Quantity
    type = 'type_example' # str | Order Price; required if order type is limit (optional)
    side = 'side_example' # str | Side (optional)
    price = 3.4 # float | Order Price; required if order type is limit (optional)
    tif = 'tif_example' # str | Time in Force (optional)

    try:
        # Submit Order
        api_response = api_instance.ccp_order_post(acct, conid, ccy, exchange, qty, type=type, side=side, price=price, tif=tif)
        print("The response of CCPBetaApi->ccp_order_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CCPBetaApi->ccp_order_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **acct** | **str**| User Account | 
 **conid** | **float**| Contract identifier from IBKR&#39;s database. | 
 **ccy** | **str**| Contract Currency | 
 **exchange** | **str**| Exchange | 
 **qty** | **float**| Order Quantity | 
 **type** | **str**| Order Price; required if order type is limit | [optional] 
 **side** | **str**| Side | [optional] 
 **price** | **float**| Order Price; required if order type is limit | [optional] 
 **tif** | **str**| Time in Force | [optional] 

### Return type

[**OrderData**](OrderData.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**500** | System error, for example when connection to CCP failed |  -  |
**400** | Bad Request |  -  |
**401** | Access denied |  -  |
**200** | An Object |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ccp_order_put**
> OrderData ccp_order_put(acct, id)

Update Order

Updates an Order. Updating an order requires the same arguments as placing an order besides the conid. Note: The status of the order can be queried through GET /ccp/order.


### Example


```python
import ibkr-web-api
from ibkr-web-api.models.order_data import OrderData
from ibkr-web-api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = ibkr-web-api.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with ibkr-web-api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ibkr-web-api.CCPBetaApi(api_client)
    acct = 'acct_example' # str | User Account
    id = 3.4 # float | Order ID to be modified

    try:
        # Update Order
        api_response = api_instance.ccp_order_put(acct, id)
        print("The response of CCPBetaApi->ccp_order_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CCPBetaApi->ccp_order_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **acct** | **str**| User Account | 
 **id** | **float**| Order ID to be modified | 

### Return type

[**OrderData**](OrderData.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**500** | System error, for example when connection to CCP failed |  -  |
**401** | Access denied |  -  |
**200** | An Object |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ccp_orders_get**
> CcpOrdersGet200Response ccp_orders_get(acct, cancelled=cancelled)

Order Status

Get status for all orders

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.ccp_orders_get200_response import CcpOrdersGet200Response
from ibkr-web-api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = ibkr-web-api.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with ibkr-web-api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ibkr-web-api.CCPBetaApi(api_client)
    acct = 'acct_example' # str | User Account
    cancelled = True # bool | Return only Rejected or Cancelled orders since today midnight (optional)

    try:
        # Order Status
        api_response = api_instance.ccp_orders_get(acct, cancelled=cancelled)
        print("The response of CCPBetaApi->ccp_orders_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CCPBetaApi->ccp_orders_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **acct** | **str**| User Account | 
 **cancelled** | **bool**| Return only Rejected or Cancelled orders since today midnight | [optional] 

### Return type

[**CcpOrdersGet200Response**](CcpOrdersGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**500** | System error |  -  |
**400** | Bad request |  -  |
**401** | Access denied |  -  |
**200** | An Object |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ccp_positions_get**
> PositionData ccp_positions_get()

Positions

List of positions

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.position_data import PositionData
from ibkr-web-api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = ibkr-web-api.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with ibkr-web-api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ibkr-web-api.CCPBetaApi(api_client)

    try:
        # Positions
        api_response = api_instance.ccp_positions_get()
        print("The response of CCPBetaApi->ccp_positions_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CCPBetaApi->ccp_positions_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**PositionData**](PositionData.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**500** | System error |  -  |
**401** | Access denied |  -  |
**200** | Valid result |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ccp_status_get**
> CcpStatusGet200Response ccp_status_get()

CCP Status

Provide the current CCP session status. When using the Gateway this endpoint will also initiate a brokerage session to CCP by sending /auth/init and response.

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.ccp_status_get200_response import CcpStatusGet200Response
from ibkr-web-api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = ibkr-web-api.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with ibkr-web-api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ibkr-web-api.CCPBetaApi(api_client)

    try:
        # CCP Status
        api_response = api_instance.ccp_status_get()
        print("The response of CCPBetaApi->ccp_status_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CCPBetaApi->ccp_status_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**CcpStatusGet200Response**](CcpStatusGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**500** | System error |  -  |
**401** | Access denied |  -  |
**200** | Valid result |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ccp_trades_get**
> CcpOrdersGet200Response ccp_trades_get(var_from=var_from, to=to)

Trades

Get a list of Trades, by default, the list is from today midnight to Date.now().


### Example


```python
import ibkr-web-api
from ibkr-web-api.models.ccp_orders_get200_response import CcpOrdersGet200Response
from ibkr-web-api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = ibkr-web-api.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with ibkr-web-api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ibkr-web-api.CCPBetaApi(api_client)
    var_from = 'var_from_example' # str | From Date (YYYYMMDD-HH:mm:ss) or offset (-1,-2,-3..) (optional)
    to = 'to_example' # str | To Date (YYYYMMDD-HH:mm:ss) or offset (-1,-2,-3..). To value should be bigger than from value.  (optional)

    try:
        # Trades
        api_response = api_instance.ccp_trades_get(var_from=var_from, to=to)
        print("The response of CCPBetaApi->ccp_trades_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CCPBetaApi->ccp_trades_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **var_from** | **str**| From Date (YYYYMMDD-HH:mm:ss) or offset (-1,-2,-3..) | [optional] 
 **to** | **str**| To Date (YYYYMMDD-HH:mm:ss) or offset (-1,-2,-3..). To value should be bigger than from value.  | [optional] 

### Return type

[**CcpOrdersGet200Response**](CcpOrdersGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**500** | System error |  -  |
**400** | Bad request |  -  |
**401** | Access denied |  -  |
**200** | An Object |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


# ibkr_web_api.OrderApi

All URIs are relative to *http://localhost:5000/v1/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**iserver_account_account_id_order_order_id_delete**](OrderApi.md#iserver_account_account_id_order_order_id_delete) | **DELETE** /iserver/account/{accountId}/order/{orderId} | Cancel Order
[**iserver_account_account_id_order_order_id_post**](OrderApi.md#iserver_account_account_id_order_order_id_post) | **POST** /iserver/account/{accountId}/order/{orderId} | Modify Order
[**iserver_account_account_id_order_post**](OrderApi.md#iserver_account_account_id_order_post) | **POST** /iserver/account/{accountId}/order | Place Order (Deprecated)
[**iserver_account_account_id_order_whatif_post**](OrderApi.md#iserver_account_account_id_order_whatif_post) | **POST** /iserver/account/{accountId}/order/whatif | Preview Order (Deprecated)
[**iserver_account_account_id_orders_post**](OrderApi.md#iserver_account_account_id_orders_post) | **POST** /iserver/account/{accountId}/orders | Place Orders
[**iserver_account_account_id_orders_whatif_post**](OrderApi.md#iserver_account_account_id_orders_whatif_post) | **POST** /iserver/account/{accountId}/orders/whatif | Preview Orders
[**iserver_account_order_status_order_id_get**](OrderApi.md#iserver_account_order_status_order_id_get) | **GET** /iserver/account/order/status/{orderId} | Order Status
[**iserver_account_orders_fa_group_post**](OrderApi.md#iserver_account_orders_fa_group_post) | **POST** /iserver/account/orders/{faGroup} | Place Orders for FA
[**iserver_account_orders_get**](OrderApi.md#iserver_account_orders_get) | **GET** /iserver/account/orders | Live Orders
[**iserver_reply_replyid_post**](OrderApi.md#iserver_reply_replyid_post) | **POST** /iserver/reply/{replyid} | Place Order Reply


# **iserver_account_account_id_order_order_id_delete**
> IserverAccountAccountIdOrderOrderIdDelete200Response iserver_account_account_id_order_order_id_delete(account_id, order_id)

Cancel Order

Cancels an open order. Must call /iserver/accounts endpoint prior to cancelling an order. Use /iservers/account/orders endpoint to review open-order(s) and get latest order status.

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_account_account_id_order_order_id_delete200_response import IserverAccountAccountIdOrderOrderIdDelete200Response
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
    api_instance = ibkr_web_api.OrderApi(api_client)
    account_id = 'account_id_example' # str | account id, or fa group if deleting a group order
    order_id = 'order_id_example' # str | Customer order id, use /iservers/account/orders endpoint to query orderId.

    try:
        # Cancel Order
        api_response = api_instance.iserver_account_account_id_order_order_id_delete(account_id, order_id)
        print("The response of OrderApi->iserver_account_account_id_order_order_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderApi->iserver_account_account_id_order_order_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**| account id, or fa group if deleting a group order | 
 **order_id** | **str**| Customer order id, use /iservers/account/orders endpoint to query orderId. | 

### Return type

[**IserverAccountAccountIdOrderOrderIdDelete200Response**](IserverAccountAccountIdOrderOrderIdDelete200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns an object with order id, message, conid and account id |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **iserver_account_account_id_order_order_id_post**
> List[IserverAccountAccountIdOrderOrderIdPost200ResponseInner] iserver_account_account_id_order_order_id_post(account_id, order_id, body)

Modify Order

Modifies an open order. Must call /iserver/accounts endpoint prior to modifying an order. Use /iservers/account/orders endpoint to review open-order(s).

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_account_account_id_order_order_id_post200_response_inner import IserverAccountAccountIdOrderOrderIdPost200ResponseInner
from ibkr_web_api.models.modify_order import ModifyOrder
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
    api_instance = ibkr_web_api.OrderApi(api_client)
    account_id = 'account_id_example' # str | account id, or fa group if modifying a group order
    order_id = 'order_id_example' # str | Customer order id, use /iservers/account/orders endpoint to query orderId.
    body = ibkr_web_api.ModifyOrder() # ModifyOrder | modify-order request

    try:
        # Modify Order
        api_response = api_instance.iserver_account_account_id_order_order_id_post(account_id, order_id, body)
        print("The response of OrderApi->iserver_account_account_id_order_order_id_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderApi->iserver_account_account_id_order_order_id_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**| account id, or fa group if modifying a group order | 
 **order_id** | **str**| Customer order id, use /iservers/account/orders endpoint to query orderId. | 
 **body** | [**ModifyOrder**](ModifyOrder.md)| modify-order request | 

### Return type

[**List[IserverAccountAccountIdOrderOrderIdPost200ResponseInner]**](IserverAccountAccountIdOrderOrderIdPost200ResponseInner.md)

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

# **iserver_account_account_id_order_post**
> List[IserverAccountAccountIdOrderPost200ResponseInner] iserver_account_account_id_order_post(account_id, body)

Place Order (Deprecated)

This endpoint is going to be deprecated, you can use /iserver/account/{accountId}/orders, just pass one order
in the array, the order structure will be same.
Please note here, sometimes this endpoint alone can't make sure you submit the order successfully,
you could receive some questions in the response, you have to to answer them in order to submit the order
successfully. You can use "/iserver/reply/{replyid}" endpoint to answer questions


### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_account_account_id_order_post200_response_inner import IserverAccountAccountIdOrderPost200ResponseInner
from ibkr_web_api.models.order_request import OrderRequest
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
    api_instance = ibkr_web_api.OrderApi(api_client)
    account_id = 'account_id_example' # str | account id
    body = ibkr_web_api.OrderRequest() # OrderRequest | order request info

    try:
        # Place Order (Deprecated)
        api_response = api_instance.iserver_account_account_id_order_post(account_id, body)
        print("The response of OrderApi->iserver_account_account_id_order_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderApi->iserver_account_account_id_order_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**| account id | 
 **body** | [**OrderRequest**](OrderRequest.md)| order request info | 

### Return type

[**List[IserverAccountAccountIdOrderPost200ResponseInner]**](IserverAccountAccountIdOrderPost200ResponseInner.md)

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

# **iserver_account_account_id_order_whatif_post**
> IserverAccountAccountIdOrderWhatifPost200Response iserver_account_account_id_order_whatif_post(account_id, body)

Preview Order (Deprecated)

This end-point is going to be deprecated, you can use /iserver/account/{accountId}/orders/whatif,
just pass one order in the array, the order structure will be same.
This endpoint allows you to preview order without actually submitting the order and you can get
commission information in the response.


### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_account_account_id_order_whatif_post200_response import IserverAccountAccountIdOrderWhatifPost200Response
from ibkr_web_api.models.order_request import OrderRequest
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
    api_instance = ibkr_web_api.OrderApi(api_client)
    account_id = 'account_id_example' # str | account id
    body = ibkr_web_api.OrderRequest() # OrderRequest | order info

    try:
        # Preview Order (Deprecated)
        api_response = api_instance.iserver_account_account_id_order_whatif_post(account_id, body)
        print("The response of OrderApi->iserver_account_account_id_order_whatif_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderApi->iserver_account_account_id_order_whatif_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**| account id | 
 **body** | [**OrderRequest**](OrderRequest.md)| order info | 

### Return type

[**IserverAccountAccountIdOrderWhatifPost200Response**](IserverAccountAccountIdOrderWhatifPost200Response.md)

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

# **iserver_account_account_id_orders_post**
> List[IserverAccountAccountIdOrderPost200ResponseInner] iserver_account_account_id_orders_post(account_id, body)

Place Orders

When connected to an IServer Brokerage Session, this endpoint will allow you to submit orders. 
CP WEB API supports various advanced orderTypes, for additional details and examples refer to [IBKR Quant Blog](https://www.tradersinsight.news/category/ibkr-quant-news/programming_languages/rest-development/).
  * Bracket - Attach additional opposite-side order(s) by using a single **cOID** sent with the parent and set the same value for **parentId** in each child order(s).
  * Cash Quantity -  Send orders using monetary value by specifying **cashQty** instead of quantity, e.g. cashQty: 200. The endpoint /iserver/contract/rules returns list of valid orderTypes in cqtTypes.
  * Currency Conversion - Convert cash from one currency to another by including **isCcyConv** = **true**. To specify the cash quantity use **fxQTY** instead of quantity, e.g. fxQTY: 100.
  * Fractional - Contracts that support fractional shares can be traded by specifying **quantity** as a float, e.g. quantity: 0.001. The endpoint /iserver/contract/rules returns a list of valid orderTypes in fraqTypes.
  * IB Algos - Attached user-defined settings to your trades by using any of IBKR's Algo Orders. Use the endpoint /iserver/contract/{conid}/algos to identify the available strategies for a contract.
  * One-Cancels-All (OCA) - Group multiple unrelated orders by passing order request info in an array and including **isSingleGroup = true** for each order. All orders will be assigned the same oca_group_id.


### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_account_account_id_order_post200_response_inner import IserverAccountAccountIdOrderPost200ResponseInner
from ibkr_web_api.models.iserver_account_account_id_orders_post_request import IserverAccountAccountIdOrdersPostRequest
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
    api_instance = ibkr_web_api.OrderApi(api_client)
    account_id = 'account_id_example' # str | account id
    body = ibkr_web_api.IserverAccountAccountIdOrdersPostRequest() # IserverAccountAccountIdOrdersPostRequest | order request info

    try:
        # Place Orders
        api_response = api_instance.iserver_account_account_id_orders_post(account_id, body)
        print("The response of OrderApi->iserver_account_account_id_orders_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderApi->iserver_account_account_id_orders_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**| account id | 
 **body** | [**IserverAccountAccountIdOrdersPostRequest**](IserverAccountAccountIdOrdersPostRequest.md)| order request info | 

### Return type

[**List[IserverAccountAccountIdOrderPost200ResponseInner]**](IserverAccountAccountIdOrderPost200ResponseInner.md)

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

# **iserver_account_account_id_orders_whatif_post**
> IserverAccountAccountIdOrderWhatifPost200Response iserver_account_account_id_orders_whatif_post(account_id, body)

Preview Orders

This endpoint allows you to preview order without actually submitting the order and you can get
commission information in the response. Also supports bracket orders.


### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_account_account_id_order_whatif_post200_response import IserverAccountAccountIdOrderWhatifPost200Response
from ibkr_web_api.models.iserver_account_account_id_orders_post_request import IserverAccountAccountIdOrdersPostRequest
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
    api_instance = ibkr_web_api.OrderApi(api_client)
    account_id = 'account_id_example' # str | account id
    body = ibkr_web_api.IserverAccountAccountIdOrdersPostRequest() # IserverAccountAccountIdOrdersPostRequest | order info

    try:
        # Preview Orders
        api_response = api_instance.iserver_account_account_id_orders_whatif_post(account_id, body)
        print("The response of OrderApi->iserver_account_account_id_orders_whatif_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderApi->iserver_account_account_id_orders_whatif_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**| account id | 
 **body** | [**IserverAccountAccountIdOrdersPostRequest**](IserverAccountAccountIdOrdersPostRequest.md)| order info | 

### Return type

[**IserverAccountAccountIdOrderWhatifPost200Response**](IserverAccountAccountIdOrderWhatifPost200Response.md)

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

# **iserver_account_order_status_order_id_get**
> OrderStatus iserver_account_order_status_order_id_get(order_id)

Order Status

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.order_status import OrderStatus
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
    api_instance = ibkr_web_api.OrderApi(api_client)
    order_id = 'order_id_example' # str | Customer order id, use /iservers/account/orders endpoint to query orderId.

    try:
        # Order Status
        api_response = api_instance.iserver_account_order_status_order_id_get(order_id)
        print("The response of OrderApi->iserver_account_order_status_order_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderApi->iserver_account_order_status_order_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_id** | **str**| Customer order id, use /iservers/account/orders endpoint to query orderId. | 

### Return type

[**OrderStatus**](OrderStatus.md)

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

# **iserver_account_orders_fa_group_post**
> List[IserverAccountAccountIdOrderPost200ResponseInner] iserver_account_orders_fa_group_post(fa_group, body)

Place Orders for FA

Financial Advisors can use this endpoint to place an order for a specified group. To place an order for a specified account use the endpoint /iserver/account/{accountId}/order.
More information about groups can be found in the [TWS Users' Guide:](https://guides.interactivebrokers.com/twsguide/twsguide.htm#usersguidebook/financialadvisors/create_an_account_group_for_share_allocation.htm).


### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_account_account_id_order_post200_response_inner import IserverAccountAccountIdOrderPost200ResponseInner
from ibkr_web_api.models.order_request import OrderRequest
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
    api_instance = ibkr_web_api.OrderApi(api_client)
    fa_group = 'fa_group_example' # str | financial advisor group
    body = ibkr_web_api.OrderRequest() # OrderRequest | order request info

    try:
        # Place Orders for FA
        api_response = api_instance.iserver_account_orders_fa_group_post(fa_group, body)
        print("The response of OrderApi->iserver_account_orders_fa_group_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderApi->iserver_account_orders_fa_group_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fa_group** | **str**| financial advisor group | 
 **body** | [**OrderRequest**](OrderRequest.md)| order request info | 

### Return type

[**List[IserverAccountAccountIdOrderPost200ResponseInner]**](IserverAccountAccountIdOrderPost200ResponseInner.md)

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

# **iserver_account_orders_get**
> IserverAccountOrdersGet200Response iserver_account_orders_get(filters=filters)

Live Orders

The endpoint is meant to be used in polling mode, e.g. requesting every x seconds.
The response will contain two objects, one is notification, the other is orders.
Orders is the list of live orders (cancelled, filled, submitted).
Notifications contains information about execute orders as they happen, see status field.
To receive streaming live orders the endpoint /ws can be used. Refer to [Streaming WebSocket Data](https://interactivebrokers.github.io/cpwebapi/RealtimeSubscription.html) for details.


### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_account_orders_get200_response import IserverAccountOrdersGet200Response
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
    api_instance = ibkr_web_api.OrderApi(api_client)
    filters = 'filters_example' # str | list of filters separated by comma (optional)

    try:
        # Live Orders
        api_response = api_instance.iserver_account_orders_get(filters=filters)
        print("The response of OrderApi->iserver_account_orders_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderApi->iserver_account_orders_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filters** | **str**| list of filters separated by comma | [optional] 

### Return type

[**IserverAccountOrdersGet200Response**](IserverAccountOrdersGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | An object contains two arrays |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **iserver_reply_replyid_post**
> List[IserverReplyReplyidPost200ResponseInner] iserver_reply_replyid_post(replyid, body)

Place Order Reply

Reply to questions when placing orders and submit orders

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_reply_replyid_post200_response_inner import IserverReplyReplyidPost200ResponseInner
from ibkr_web_api.models.iserver_reply_replyid_post_request import IserverReplyReplyidPostRequest
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
    api_instance = ibkr_web_api.OrderApi(api_client)
    replyid = 'replyid_example' # str | Please use the \"id\" from the response of \"Place Order\" endpoint
    body = ibkr_web_api.IserverReplyReplyidPostRequest() # IserverReplyReplyidPostRequest | Answer to question

    try:
        # Place Order Reply
        api_response = api_instance.iserver_reply_replyid_post(replyid, body)
        print("The response of OrderApi->iserver_reply_replyid_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderApi->iserver_reply_replyid_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **replyid** | **str**| Please use the \&quot;id\&quot; from the response of \&quot;Place Order\&quot; endpoint | 
 **body** | [**IserverReplyReplyidPostRequest**](IserverReplyReplyidPostRequest.md)| Answer to question | 

### Return type

[**List[IserverReplyReplyidPost200ResponseInner]**](IserverReplyReplyidPost200ResponseInner.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Order is submitted successfully, returns an array contains one object |  -  |
**400** | When you send \&quot;confirmed-false\&quot; in the request, you will receive this |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


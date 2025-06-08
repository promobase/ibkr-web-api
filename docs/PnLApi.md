# ibkr-web-api.PnLApi

All URIs are relative to *http://localhost:5000/v1/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**iserver_account_pnl_partitioned_get**](PnLApi.md#iserver_account_pnl_partitioned_get) | **GET** /iserver/account/pnl/partitioned | PnL for the selected account


# **iserver_account_pnl_partitioned_get**
> IserverAccountPnlPartitionedGet200Response iserver_account_pnl_partitioned_get()

PnL for the selected account

Returns an object containing PnL for the selected account and its models (if any).
To receive streaming PnL the endpoint /ws can be used. Refer to [Streaming WebSocket Data](https://interactivebrokers.github.io/cpwebapi/RealtimeSubscription.html) for details.


### Example


```python
import ibkr-web-api
from ibkr-web-api.models.iserver_account_pnl_partitioned_get200_response import IserverAccountPnlPartitionedGet200Response
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
    api_instance = ibkr-web-api.PnLApi(api_client)

    try:
        # PnL for the selected account
        api_response = api_instance.iserver_account_pnl_partitioned_get()
        print("The response of PnLApi->iserver_account_pnl_partitioned_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PnLApi->iserver_account_pnl_partitioned_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**IserverAccountPnlPartitionedGet200Response**](IserverAccountPnlPartitionedGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | An object containing account and model(s) pnl |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


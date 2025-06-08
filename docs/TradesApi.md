# ibkr_web_api.TradesApi

All URIs are relative to *http://localhost:5000/v1/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**iserver_account_trades_get**](TradesApi.md#iserver_account_trades_get) | **GET** /iserver/account/trades | List of Trades for the selected account


# **iserver_account_trades_get**
> List[Trade] iserver_account_trades_get()

List of Trades for the selected account

Returns a list of trades for the currently selected account for current day and six previous days. It is advised to call this endpoint once per session.


### Example


```python
import ibkr_web_api
from ibkr_web_api.models.trade import Trade
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
    api_instance = ibkr_web_api.TradesApi(api_client)

    try:
        # List of Trades for the selected account
        api_response = api_instance.iserver_account_trades_get()
        print("The response of TradesApi->iserver_account_trades_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TradesApi->iserver_account_trades_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[Trade]**](Trade.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | An array of trades |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


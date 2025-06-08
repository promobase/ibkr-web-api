# ibkr_web_api.StreamingApi

All URIs are relative to *http://localhost:5000/v1/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ws_post**](StreamingApi.md#ws_post) | **POST** /ws | Websocket Endpoint


# **ws_post**
> ws_post()

Websocket Endpoint

The streaming API is documented under [Streaming WebSocket Data](https://interactivebrokers.github.io/cpwebapi/RealtimeSubscription.html) for details.

### Example


```python
import ibkr_web_api
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
    api_instance = ibkr_web_api.StreamingApi(api_client)

    try:
        # Websocket Endpoint
        api_instance.ws_post()
    except Exception as e:
        print("Exception when calling StreamingApi->ws_post: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | confirms session is open |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


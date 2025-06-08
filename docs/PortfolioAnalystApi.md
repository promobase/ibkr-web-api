# ibkr-web-api.PortfolioAnalystApi

All URIs are relative to *http://localhost:5000/v1/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**pa_performance_post**](PortfolioAnalystApi.md#pa_performance_post) | **POST** /pa/performance | Account Performance
[**pa_summary_post**](PortfolioAnalystApi.md#pa_summary_post) | **POST** /pa/summary | Account Balance&#39;s Summary (Deprecated)
[**pa_transactions_post**](PortfolioAnalystApi.md#pa_transactions_post) | **POST** /pa/transactions | Position&#39;s Transaction History


# **pa_performance_post**
> Performance pa_performance_post(body)

Account Performance

Returns the performance (MTM) for the given accounts, if more than one account is passed, the result is consolidated.

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.pa_performance_post_request import PaPerformancePostRequest
from ibkr-web-api.models.performance import Performance
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
    api_instance = ibkr-web-api.PortfolioAnalystApi(api_client)
    body = ibkr-web-api.PaPerformancePostRequest() # PaPerformancePostRequest | an array of account ids

    try:
        # Account Performance
        api_response = api_instance.pa_performance_post(body)
        print("The response of PortfolioAnalystApi->pa_performance_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PortfolioAnalystApi->pa_performance_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**PaPerformancePostRequest**](PaPerformancePostRequest.md)| an array of account ids | 

### Return type

[**Performance**](Performance.md)

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

# **pa_summary_post**
> Summary pa_summary_post(body)

Account Balance's Summary (Deprecated)

This endpoint is going to be deprecated. Please use /pa/performance instead.
Returns a summary of all account balances for the given accounts, if more than one account is passe, the result is consolidated.

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.pa_summary_post_request import PaSummaryPostRequest
from ibkr-web-api.models.summary import Summary
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
    api_instance = ibkr-web-api.PortfolioAnalystApi(api_client)
    body = ibkr-web-api.PaSummaryPostRequest() # PaSummaryPostRequest | an array of account ids

    try:
        # Account Balance's Summary (Deprecated)
        api_response = api_instance.pa_summary_post(body)
        print("The response of PortfolioAnalystApi->pa_summary_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PortfolioAnalystApi->pa_summary_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**PaSummaryPostRequest**](PaSummaryPostRequest.md)| an array of account ids | 

### Return type

[**Summary**](Summary.md)

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

# **pa_transactions_post**
> Transactions pa_transactions_post(body)

Position's Transaction History

transaction history for a given number of conids and accounts.
Types of transactions include dividend payments, buy and sell transactions, transfers.


### Example


```python
import ibkr-web-api
from ibkr-web-api.models.pa_transactions_post_request import PaTransactionsPostRequest
from ibkr-web-api.models.transactions import Transactions
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
    api_instance = ibkr-web-api.PortfolioAnalystApi(api_client)
    body = ibkr-web-api.PaTransactionsPostRequest() # PaTransactionsPostRequest | 

    try:
        # Position's Transaction History
        api_response = api_instance.pa_transactions_post(body)
        print("The response of PortfolioAnalystApi->pa_transactions_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PortfolioAnalystApi->pa_transactions_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**PaTransactionsPostRequest**](PaTransactionsPostRequest.md)|  | 

### Return type

[**Transactions**](Transactions.md)

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


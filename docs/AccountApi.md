# ibkr-web-api.AccountApi

All URIs are relative to *http://localhost:5000/v1/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**iserver_account_pnl_partitioned_get**](AccountApi.md#iserver_account_pnl_partitioned_get) | **GET** /iserver/account/pnl/partitioned | PnL for the selected account
[**iserver_account_post**](AccountApi.md#iserver_account_post) | **POST** /iserver/account | Switch Account
[**iserver_accounts_get**](AccountApi.md#iserver_accounts_get) | **GET** /iserver/accounts | Brokerage Accounts
[**portfolio_account_id_ledger_get**](AccountApi.md#portfolio_account_id_ledger_get) | **GET** /portfolio/{accountId}/ledger | Account Ledger
[**portfolio_account_id_meta_get**](AccountApi.md#portfolio_account_id_meta_get) | **GET** /portfolio/{accountId}/meta | Account Information
[**portfolio_account_id_summary_get**](AccountApi.md#portfolio_account_id_summary_get) | **GET** /portfolio/{accountId}/summary | Account Summary
[**portfolio_accounts_get**](AccountApi.md#portfolio_accounts_get) | **GET** /portfolio/accounts | Portfolio Accounts
[**portfolio_subaccounts2_get**](AccountApi.md#portfolio_subaccounts2_get) | **GET** /portfolio/subaccounts2 | List of Sub-Accounts (Large Accounts)
[**portfolio_subaccounts_get**](AccountApi.md#portfolio_subaccounts_get) | **GET** /portfolio/subaccounts | List of Sub-Accounts


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
    api_instance = ibkr-web-api.AccountApi(api_client)

    try:
        # PnL for the selected account
        api_response = api_instance.iserver_account_pnl_partitioned_get()
        print("The response of AccountApi->iserver_account_pnl_partitioned_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountApi->iserver_account_pnl_partitioned_get: %s\n" % e)
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

# **iserver_account_post**
> IserverAccountPost200Response iserver_account_post(body)

Switch Account

If an user has multiple accounts, and user wants to get orders, trades, etc. of an account other than currently selected account, then user can update the currently selected account using this API and then can fetch required information for the newly updated account.

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.iserver_account_post200_response import IserverAccountPost200Response
from ibkr-web-api.models.set_account import SetAccount
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
    api_instance = ibkr-web-api.AccountApi(api_client)
    body = ibkr-web-api.SetAccount() # SetAccount | account id

    try:
        # Switch Account
        api_response = api_instance.iserver_account_post(body)
        print("The response of AccountApi->iserver_account_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountApi->iserver_account_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**SetAccount**](SetAccount.md)| account id | 

### Return type

[**IserverAccountPost200Response**](IserverAccountPost200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | an object containing updated account ID |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **iserver_accounts_get**
> IserverAccountsGet200Response iserver_accounts_get()

Brokerage Accounts

Returns a list of accounts the user has trading access to, their respective aliases and the currently selected account. Note this endpoint must be called before modifying an order or querying open orders.

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.iserver_accounts_get200_response import IserverAccountsGet200Response
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
    api_instance = ibkr-web-api.AccountApi(api_client)

    try:
        # Brokerage Accounts
        api_response = api_instance.iserver_accounts_get()
        print("The response of AccountApi->iserver_accounts_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountApi->iserver_accounts_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**IserverAccountsGet200Response**](IserverAccountsGet200Response.md)

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

# **portfolio_account_id_ledger_get**
> PortfolioAccountIdLedgerGet200Response portfolio_account_id_ledger_get(account_id)

Account Ledger

Information regarding settled cash, cash balances, etc. in the account's base currency and any other cash balances hold in other currencies.  /portfolio/accounts or /portfolio/subaccounts must be called prior to this endpoint. The list of supported currencies is available at https://www.interactivebrokers.com/en/index.php?f=3185.

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.portfolio_account_id_ledger_get200_response import PortfolioAccountIdLedgerGet200Response
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
    api_instance = ibkr-web-api.AccountApi(api_client)
    account_id = 'account_id_example' # str | account id

    try:
        # Account Ledger
        api_response = api_instance.portfolio_account_id_ledger_get(account_id)
        print("The response of AccountApi->portfolio_account_id_ledger_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountApi->portfolio_account_id_ledger_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**| account id | 

### Return type

[**PortfolioAccountIdLedgerGet200Response**](PortfolioAccountIdLedgerGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 200 means successful |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **portfolio_account_id_meta_get**
> List[Account] portfolio_account_id_meta_get(account_id)

Account Information

Account information related to account Id /portfolio/accounts or /portfolio/subaccounts must be called prior to this endpoint.

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.account import Account
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
    api_instance = ibkr-web-api.AccountApi(api_client)
    account_id = 'account_id_example' # str | account id

    try:
        # Account Information
        api_response = api_instance.portfolio_account_id_meta_get(account_id)
        print("The response of AccountApi->portfolio_account_id_meta_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountApi->portfolio_account_id_meta_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**| account id | 

### Return type

[**List[Account]**](Account.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | An object |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **portfolio_account_id_summary_get**
> PortfolioAccountIdSummaryGet200Response portfolio_account_id_summary_get(account_id)

Account Summary

Returns information about margin, cash balances and other information related to specified account. See also /portfolio/{accountId}/ledger. /portfolio/accounts or /portfolio/subaccounts must be called prior to this endpoint.

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.portfolio_account_id_summary_get200_response import PortfolioAccountIdSummaryGet200Response
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
    api_instance = ibkr-web-api.AccountApi(api_client)
    account_id = 'account_id_example' # str | account id

    try:
        # Account Summary
        api_response = api_instance.portfolio_account_id_summary_get(account_id)
        print("The response of AccountApi->portfolio_account_id_summary_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountApi->portfolio_account_id_summary_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**| account id | 

### Return type

[**PortfolioAccountIdSummaryGet200Response**](PortfolioAccountIdSummaryGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns an object containing account summary. The object contains multiple properties. A property is sufficed with -c if its provides commodity value, -s if it provides security value and -c if its UKL segment value |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **portfolio_accounts_get**
> List[Account] portfolio_accounts_get()

Portfolio Accounts

In non-tiered account structures, returns a list of accounts for which the user can view position and account information. This endpoint must be called prior to calling other /portfolio endpoints for those accounts. For querying a list of accounts which the user can trade, see /iserver/accounts. For a list of subaccounts in tiered account structures (e.g. financial advisor or ibroker accounts) see /portfolio/subaccounts.

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.account import Account
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
    api_instance = ibkr-web-api.AccountApi(api_client)

    try:
        # Portfolio Accounts
        api_response = api_instance.portfolio_accounts_get()
        print("The response of AccountApi->portfolio_accounts_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountApi->portfolio_accounts_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[Account]**](Account.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | An array |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **portfolio_subaccounts2_get**
> PortfolioSubaccounts2Get200Response portfolio_subaccounts2_get(page)

List of Sub-Accounts (Large Accounts)

Used in tiered account structures (such as Financial Advisor and IBroker Accounts) to return a list of sub-accounts, paginated up to 20 accounts per page, for which the user can view position and account-related information. This endpoint must be called prior to calling other /portfolio endpoints for those sub-accounts. If you have less than 100 sub-accounts use /portfolio/subaccounts. To query a list of accounts the user can trade, see /iserver/accounts.

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.portfolio_subaccounts2_get200_response import PortfolioSubaccounts2Get200Response
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
    api_instance = ibkr-web-api.AccountApi(api_client)
    page = '0' # str |  (default to '0')

    try:
        # List of Sub-Accounts (Large Accounts)
        api_response = api_instance.portfolio_subaccounts2_get(page)
        print("The response of AccountApi->portfolio_subaccounts2_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountApi->portfolio_subaccounts2_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **str**|  | [default to &#39;0&#39;]

### Return type

[**PortfolioSubaccounts2Get200Response**](PortfolioSubaccounts2Get200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | An object containing an array |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **portfolio_subaccounts_get**
> Account portfolio_subaccounts_get()

List of Sub-Accounts

Used in tiered account structures (such as Financial Advisor and IBroker Accounts) to return a list of up to 100 sub-accounts for which the user can view position and account-related information. This endpoint must be called prior to calling other /portfolio endpoints for those sub-accounts. If you have more than 100 sub-accounts use /portfolio/subaccounts2. To query a list of accounts the user can trade, see /iserver/accounts.

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.account import Account
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
    api_instance = ibkr-web-api.AccountApi(api_client)

    try:
        # List of Sub-Accounts
        api_response = api_instance.portfolio_subaccounts_get()
        print("The response of AccountApi->portfolio_subaccounts_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountApi->portfolio_subaccounts_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**Account**](Account.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | An array |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


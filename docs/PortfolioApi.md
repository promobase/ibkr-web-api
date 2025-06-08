# ibkr_web_api.PortfolioApi

All URIs are relative to *http://localhost:5000/v1/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**portfolio_account_id_allocation_get**](PortfolioApi.md#portfolio_account_id_allocation_get) | **GET** /portfolio/{accountId}/allocation | Account Allocation
[**portfolio_account_id_ledger_get**](PortfolioApi.md#portfolio_account_id_ledger_get) | **GET** /portfolio/{accountId}/ledger | Account Ledger
[**portfolio_account_id_meta_get**](PortfolioApi.md#portfolio_account_id_meta_get) | **GET** /portfolio/{accountId}/meta | Account Information
[**portfolio_account_id_position_conid_get**](PortfolioApi.md#portfolio_account_id_position_conid_get) | **GET** /portfolio/{accountId}/position/{conid} | Position by Conid
[**portfolio_account_id_positions_invalidate_post**](PortfolioApi.md#portfolio_account_id_positions_invalidate_post) | **POST** /portfolio/{accountId}/positions/invalidate | Invalidates the backend cache of the Portfolio
[**portfolio_account_id_positions_page_id_get**](PortfolioApi.md#portfolio_account_id_positions_page_id_get) | **GET** /portfolio/{accountId}/positions/{pageId} | Portfolio Positions
[**portfolio_account_id_summary_get**](PortfolioApi.md#portfolio_account_id_summary_get) | **GET** /portfolio/{accountId}/summary | Account Summary
[**portfolio_accounts_get**](PortfolioApi.md#portfolio_accounts_get) | **GET** /portfolio/accounts | Portfolio Accounts
[**portfolio_allocation_post**](PortfolioApi.md#portfolio_allocation_post) | **POST** /portfolio/allocation | Account Alloction (All Accounts)
[**portfolio_positions_conid_get**](PortfolioApi.md#portfolio_positions_conid_get) | **GET** /portfolio/positions/{conid} | Positions by Conid
[**portfolio_subaccounts2_get**](PortfolioApi.md#portfolio_subaccounts2_get) | **GET** /portfolio/subaccounts2 | List of Sub-Accounts (Large Accounts)
[**portfolio_subaccounts_get**](PortfolioApi.md#portfolio_subaccounts_get) | **GET** /portfolio/subaccounts | List of Sub-Accounts


# **portfolio_account_id_allocation_get**
> List[AllocationInner] portfolio_account_id_allocation_get(account_id)

Account Allocation

Information about the account's portfolio allocation by Asset Class, Industry and Category.  /portfolio/accounts or /portfolio/subaccounts must be called prior to this endpoint.

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.allocation_inner import AllocationInner
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
    api_instance = ibkr_web_api.PortfolioApi(api_client)
    account_id = 'account_id_example' # str | account id

    try:
        # Account Allocation
        api_response = api_instance.portfolio_account_id_allocation_get(account_id)
        print("The response of PortfolioApi->portfolio_account_id_allocation_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PortfolioApi->portfolio_account_id_allocation_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**| account id | 

### Return type

[**List[AllocationInner]**](AllocationInner.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns an object of three different allocations |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **portfolio_account_id_ledger_get**
> PortfolioAccountIdLedgerGet200Response portfolio_account_id_ledger_get(account_id)

Account Ledger

Information regarding settled cash, cash balances, etc. in the account's base currency and any other cash balances hold in other currencies.  /portfolio/accounts or /portfolio/subaccounts must be called prior to this endpoint. The list of supported currencies is available at https://www.interactivebrokers.com/en/index.php?f=3185.

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.portfolio_account_id_ledger_get200_response import PortfolioAccountIdLedgerGet200Response
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
    api_instance = ibkr_web_api.PortfolioApi(api_client)
    account_id = 'account_id_example' # str | account id

    try:
        # Account Ledger
        api_response = api_instance.portfolio_account_id_ledger_get(account_id)
        print("The response of PortfolioApi->portfolio_account_id_ledger_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PortfolioApi->portfolio_account_id_ledger_get: %s\n" % e)
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
import ibkr_web_api
from ibkr_web_api.models.account import Account
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
    api_instance = ibkr_web_api.PortfolioApi(api_client)
    account_id = 'account_id_example' # str | account id

    try:
        # Account Information
        api_response = api_instance.portfolio_account_id_meta_get(account_id)
        print("The response of PortfolioApi->portfolio_account_id_meta_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PortfolioApi->portfolio_account_id_meta_get: %s\n" % e)
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

# **portfolio_account_id_position_conid_get**
> List[PositionInner] portfolio_account_id_position_conid_get(account_id, conid)

Position by Conid

Returns a list of all positions matching the conid. For portfolio models the conid could be in more than one model, returning an array with the name of the model it belongs to.  /portfolio/accounts or /portfolio/subaccounts must be called prior to this endpoint.

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.position_inner import PositionInner
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
    api_instance = ibkr_web_api.PortfolioApi(api_client)
    account_id = 'account_id_example' # str | account id
    conid = 56 # int | contract id

    try:
        # Position by Conid
        api_response = api_instance.portfolio_account_id_position_conid_get(account_id, conid)
        print("The response of PortfolioApi->portfolio_account_id_position_conid_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PortfolioApi->portfolio_account_id_position_conid_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**| account id | 
 **conid** | **int**| contract id | 

### Return type

[**List[PositionInner]**](PositionInner.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns a list containing only one position for the conid |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **portfolio_account_id_positions_invalidate_post**
> object portfolio_account_id_positions_invalidate_post(account_id)

Invalidates the backend cache of the Portfolio

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
    api_instance = ibkr_web_api.PortfolioApi(api_client)
    account_id = 'account_id_example' # str | account id

    try:
        # Invalidates the backend cache of the Portfolio
        api_response = api_instance.portfolio_account_id_positions_invalidate_post(account_id)
        print("The response of PortfolioApi->portfolio_account_id_positions_invalidate_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PortfolioApi->portfolio_account_id_positions_invalidate_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**| account id | 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Means successful |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **portfolio_account_id_positions_page_id_get**
> List[PositionInner] portfolio_account_id_positions_page_id_get(account_id, page_id, model=model, sort=sort, direction=direction, period=period)

Portfolio Positions

Returns a list of positions for the given account. The endpoint supports paging, page's default size is 30 positions. /portfolio/accounts or /portfolio/subaccounts must be called prior to this endpoint.

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.position_inner import PositionInner
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
    api_instance = ibkr_web_api.PortfolioApi(api_client)
    account_id = 'account_id_example' # str | account id
    page_id = '0' # str | page id (default to '0')
    model = 'model_example' # str | optional (optional)
    sort = 'sort_example' # str | declare the table to be sorted by which column (optional)
    direction = 'direction_example' # str | in which order, a means ascending - d means descending (optional)
    period = 'period_example' # str | period for pnl column, can be 1D, 7D, 1M... (optional)

    try:
        # Portfolio Positions
        api_response = api_instance.portfolio_account_id_positions_page_id_get(account_id, page_id, model=model, sort=sort, direction=direction, period=period)
        print("The response of PortfolioApi->portfolio_account_id_positions_page_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PortfolioApi->portfolio_account_id_positions_page_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**| account id | 
 **page_id** | **str**| page id | [default to &#39;0&#39;]
 **model** | **str**| optional | [optional] 
 **sort** | **str**| declare the table to be sorted by which column | [optional] 
 **direction** | **str**| in which order, a means ascending - d means descending | [optional] 
 **period** | **str**| period for pnl column, can be 1D, 7D, 1M... | [optional] 

### Return type

[**List[PositionInner]**](PositionInner.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns a list of positions in the portfolio |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **portfolio_account_id_summary_get**
> PortfolioAccountIdSummaryGet200Response portfolio_account_id_summary_get(account_id)

Account Summary

Returns information about margin, cash balances and other information related to specified account. See also /portfolio/{accountId}/ledger. /portfolio/accounts or /portfolio/subaccounts must be called prior to this endpoint.

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.portfolio_account_id_summary_get200_response import PortfolioAccountIdSummaryGet200Response
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
    api_instance = ibkr_web_api.PortfolioApi(api_client)
    account_id = 'account_id_example' # str | account id

    try:
        # Account Summary
        api_response = api_instance.portfolio_account_id_summary_get(account_id)
        print("The response of PortfolioApi->portfolio_account_id_summary_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PortfolioApi->portfolio_account_id_summary_get: %s\n" % e)
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
import ibkr_web_api
from ibkr_web_api.models.account import Account
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
    api_instance = ibkr_web_api.PortfolioApi(api_client)

    try:
        # Portfolio Accounts
        api_response = api_instance.portfolio_accounts_get()
        print("The response of PortfolioApi->portfolio_accounts_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PortfolioApi->portfolio_accounts_get: %s\n" % e)
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

# **portfolio_allocation_post**
> List[AllocationInner] portfolio_allocation_post(body)

Account Alloction (All Accounts)

Similar to /portfolio/{accountId}/allocation but returns a consolidated view of of all the accounts returned by /portfolio/accounts. /portfolio/accounts or /portfolio/subaccounts must be called prior to this endpoint.

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.allocation_inner import AllocationInner
from ibkr_web_api.models.pa_summary_post_request import PaSummaryPostRequest
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
    api_instance = ibkr_web_api.PortfolioApi(api_client)
    body = ibkr_web_api.PaSummaryPostRequest() # PaSummaryPostRequest | accounts info

    try:
        # Account Alloction (All Accounts)
        api_response = api_instance.portfolio_allocation_post(body)
        print("The response of PortfolioApi->portfolio_allocation_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PortfolioApi->portfolio_allocation_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**PaSummaryPostRequest**](PaSummaryPostRequest.md)| accounts info | 

### Return type

[**List[AllocationInner]**](AllocationInner.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns an object of three different allocations |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **portfolio_positions_conid_get**
> PortfolioPositionsConidGet200Response portfolio_positions_conid_get(conid)

Positions by Conid

Returns an object of all positions matching the conid for all the selected accounts. For portfolio models the conid could be in more than one model, returning an array with the name of the model it belongs to. /portfolio/accounts or /portfolio/subaccounts must be called prior to this endpoint.

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.portfolio_positions_conid_get200_response import PortfolioPositionsConidGet200Response
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
    api_instance = ibkr_web_api.PortfolioApi(api_client)
    conid = 56 # int | contract id

    try:
        # Positions by Conid
        api_response = api_instance.portfolio_positions_conid_get(conid)
        print("The response of PortfolioApi->portfolio_positions_conid_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PortfolioApi->portfolio_positions_conid_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conid** | **int**| contract id | 

### Return type

[**PortfolioPositionsConidGet200Response**](PortfolioPositionsConidGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns an object containing account and its position information |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **portfolio_subaccounts2_get**
> PortfolioSubaccounts2Get200Response portfolio_subaccounts2_get(page)

List of Sub-Accounts (Large Accounts)

Used in tiered account structures (such as Financial Advisor and IBroker Accounts) to return a list of sub-accounts, paginated up to 20 accounts per page, for which the user can view position and account-related information. This endpoint must be called prior to calling other /portfolio endpoints for those sub-accounts. If you have less than 100 sub-accounts use /portfolio/subaccounts. To query a list of accounts the user can trade, see /iserver/accounts.

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.portfolio_subaccounts2_get200_response import PortfolioSubaccounts2Get200Response
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
    api_instance = ibkr_web_api.PortfolioApi(api_client)
    page = '0' # str |  (default to '0')

    try:
        # List of Sub-Accounts (Large Accounts)
        api_response = api_instance.portfolio_subaccounts2_get(page)
        print("The response of PortfolioApi->portfolio_subaccounts2_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PortfolioApi->portfolio_subaccounts2_get: %s\n" % e)
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
import ibkr_web_api
from ibkr_web_api.models.account import Account
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
    api_instance = ibkr_web_api.PortfolioApi(api_client)

    try:
        # List of Sub-Accounts
        api_response = api_instance.portfolio_subaccounts_get()
        print("The response of PortfolioApi->portfolio_subaccounts_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PortfolioApi->portfolio_subaccounts_get: %s\n" % e)
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


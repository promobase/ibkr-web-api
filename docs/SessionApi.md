# ibkr-web-api.SessionApi

All URIs are relative to *http://localhost:5000/v1/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**iserver_auth_status_post**](SessionApi.md#iserver_auth_status_post) | **POST** /iserver/auth/status | Authentication Status
[**iserver_reauthenticate_post**](SessionApi.md#iserver_reauthenticate_post) | **POST** /iserver/reauthenticate | Tries to re-authenticate to Brokerage
[**logout_post**](SessionApi.md#logout_post) | **POST** /logout | Ends the current session
[**sso_validate_get**](SessionApi.md#sso_validate_get) | **GET** /sso/validate | Validate SSO
[**tickle_post**](SessionApi.md#tickle_post) | **POST** /tickle | Ping the server to keep the session open


# **iserver_auth_status_post**
> AuthStatus iserver_auth_status_post()

Authentication Status

Current Authentication status to the Brokerage system. Market Data and Trading is not possible if not authenticated, e.g. authenticated shows false

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.auth_status import AuthStatus
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
    api_instance = ibkr-web-api.SessionApi(api_client)

    try:
        # Authentication Status
        api_response = api_instance.iserver_auth_status_post()
        print("The response of SessionApi->iserver_auth_status_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SessionApi->iserver_auth_status_post: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**AuthStatus**](AuthStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Authentication Status |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **iserver_reauthenticate_post**
> AuthStatus iserver_reauthenticate_post()

Tries to re-authenticate to Brokerage

When using the CP Gateway, this endpoint provides a way to reauthenticate to the Brokerage system as long as there is a valid SSO session, see /sso/validate.


### Example


```python
import ibkr-web-api
from ibkr-web-api.models.auth_status import AuthStatus
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
    api_instance = ibkr-web-api.SessionApi(api_client)

    try:
        # Tries to re-authenticate to Brokerage
        api_response = api_instance.iserver_reauthenticate_post()
        print("The response of SessionApi->iserver_reauthenticate_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SessionApi->iserver_reauthenticate_post: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**AuthStatus**](AuthStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Authentication Status |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **logout_post**
> LogoutPost200Response logout_post()

Ends the current session

Logs the user out of the gateway session. Any further activity requires re-authentication.

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.logout_post200_response import LogoutPost200Response
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
    api_instance = ibkr-web-api.SessionApi(api_client)

    try:
        # Ends the current session
        api_response = api_instance.logout_post()
        print("The response of SessionApi->logout_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SessionApi->logout_post: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**LogoutPost200Response**](LogoutPost200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returned status indicates if user is logged in |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sso_validate_get**
> SsoValidateGet200Response sso_validate_get()

Validate SSO

Validates the current session for the SSO user

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.sso_validate_get200_response import SsoValidateGet200Response
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
    api_instance = ibkr-web-api.SessionApi(api_client)

    try:
        # Validate SSO
        api_response = api_instance.sso_validate_get()
        print("The response of SessionApi->sso_validate_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SessionApi->sso_validate_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**SsoValidateGet200Response**](SsoValidateGet200Response.md)

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

# **tickle_post**
> tickle_post()

Ping the server to keep the session open

If the gateway has not received any requests for several minutes an open session will automatically timeout. The tickle endpoint pings the server to prevent the session from ending.

### Example


```python
import ibkr-web-api
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
    api_instance = ibkr-web-api.SessionApi(api_client)

    try:
        # Ping the server to keep the session open
        api_instance.tickle_post()
    except Exception as e:
        print("Exception when calling SessionApi->tickle_post: %s\n" % e)
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


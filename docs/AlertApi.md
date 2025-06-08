# ibkr_web_api.AlertApi

All URIs are relative to *http://localhost:5000/v1/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**iserver_account_account_id_alert_activate_post**](AlertApi.md#iserver_account_account_id_alert_activate_post) | **POST** /iserver/account/:accountId/alert/activate | Activate or deactivate an alert
[**iserver_account_account_id_alert_alert_id_delete**](AlertApi.md#iserver_account_account_id_alert_alert_id_delete) | **DELETE** /iserver/account/:accountId/alert/:alertId | Delete an alert
[**iserver_account_account_id_alert_post**](AlertApi.md#iserver_account_account_id_alert_post) | **POST** /iserver/account/{accountId}/alert | Create or modify alert
[**iserver_account_account_id_alerts_get**](AlertApi.md#iserver_account_account_id_alerts_get) | **GET** /iserver/account/:accountId/alerts | Get a list of available alerts
[**iserver_account_alert_id_get**](AlertApi.md#iserver_account_alert_id_get) | **GET** /iserver/account/alert/:id | Get details of an alert
[**iserver_account_mta_get**](AlertApi.md#iserver_account_mta_get) | **GET** /iserver/account/mta | Get MTA alert


# **iserver_account_account_id_alert_activate_post**
> IserverAccountAccountIdAlertActivatePost200Response iserver_account_account_id_alert_activate_post(account_id, body)

Activate or deactivate an alert

Please note, if alertId is 0, it will activate/deactivate all alerts

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_account_account_id_alert_activate_post200_response import IserverAccountAccountIdAlertActivatePost200Response
from ibkr_web_api.models.iserver_account_account_id_alert_activate_post_request import IserverAccountAccountIdAlertActivatePostRequest
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
    api_instance = ibkr_web_api.AlertApi(api_client)
    account_id = 'account_id_example' # str | account id
    body = ibkr_web_api.IserverAccountAccountIdAlertActivatePostRequest() # IserverAccountAccountIdAlertActivatePostRequest | order request info

    try:
        # Activate or deactivate an alert
        api_response = api_instance.iserver_account_account_id_alert_activate_post(account_id, body)
        print("The response of AlertApi->iserver_account_account_id_alert_activate_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlertApi->iserver_account_account_id_alert_activate_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**| account id | 
 **body** | [**IserverAccountAccountIdAlertActivatePostRequest**](IserverAccountAccountIdAlertActivatePostRequest.md)| order request info | 

### Return type

[**IserverAccountAccountIdAlertActivatePost200Response**](IserverAccountAccountIdAlertActivatePost200Response.md)

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

# **iserver_account_account_id_alert_alert_id_delete**
> IserverAccountAccountIdAlertActivatePost200Response iserver_account_account_id_alert_alert_id_delete(account_id, alert_id)

Delete an alert

Please be careful, if alertId is 0, it will delete all alerts

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_account_account_id_alert_activate_post200_response import IserverAccountAccountIdAlertActivatePost200Response
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
    api_instance = ibkr_web_api.AlertApi(api_client)
    account_id = 'account_id_example' # str | account id
    alert_id = 'alert_id_example' # str | alert id

    try:
        # Delete an alert
        api_response = api_instance.iserver_account_account_id_alert_alert_id_delete(account_id, alert_id)
        print("The response of AlertApi->iserver_account_account_id_alert_alert_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlertApi->iserver_account_account_id_alert_alert_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**| account id | 
 **alert_id** | **str**| alert id | 

### Return type

[**IserverAccountAccountIdAlertActivatePost200Response**](IserverAccountAccountIdAlertActivatePost200Response.md)

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

# **iserver_account_account_id_alert_post**
> IserverAccountAccountIdAlertPost200Response iserver_account_account_id_alert_post(account_id, body)

Create or modify alert

Please note here, DO NOT pass orderId when creating a new alert, toolId is only required for MTA alert


### Example


```python
import ibkr_web_api
from ibkr_web_api.models.alert_request import AlertRequest
from ibkr_web_api.models.iserver_account_account_id_alert_post200_response import IserverAccountAccountIdAlertPost200Response
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
    api_instance = ibkr_web_api.AlertApi(api_client)
    account_id = 'account_id_example' # str | account id
    body = ibkr_web_api.AlertRequest() # AlertRequest | alert info

    try:
        # Create or modify alert
        api_response = api_instance.iserver_account_account_id_alert_post(account_id, body)
        print("The response of AlertApi->iserver_account_account_id_alert_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlertApi->iserver_account_account_id_alert_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**| account id | 
 **body** | [**AlertRequest**](AlertRequest.md)| alert info | 

### Return type

[**IserverAccountAccountIdAlertPost200Response**](IserverAccountAccountIdAlertPost200Response.md)

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

# **iserver_account_account_id_alerts_get**
> List[IserverAccountAccountIdAlertsGet200ResponseInner] iserver_account_account_id_alerts_get(account_id)

Get a list of available alerts

The response will contain both active and inactive alerts, but it won't have MTA alert

### Example


```python
import ibkr_web_api
from ibkr_web_api.models.iserver_account_account_id_alerts_get200_response_inner import IserverAccountAccountIdAlertsGet200ResponseInner
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
    api_instance = ibkr_web_api.AlertApi(api_client)
    account_id = 'account_id_example' # str | account id

    try:
        # Get a list of available alerts
        api_response = api_instance.iserver_account_account_id_alerts_get(account_id)
        print("The response of AlertApi->iserver_account_account_id_alerts_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlertApi->iserver_account_account_id_alerts_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**| account id | 

### Return type

[**List[IserverAccountAccountIdAlertsGet200ResponseInner]**](IserverAccountAccountIdAlertsGet200ResponseInner.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | returns an array of objects |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **iserver_account_alert_id_get**
> AlertResponse iserver_account_alert_id_get(id)

Get details of an alert

Use the endpoint /iserver/account/:accountId/alerts to receive the alert id.
The order_id in the response is the alert id.


### Example


```python
import ibkr_web_api
from ibkr_web_api.models.alert_response import AlertResponse
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
    api_instance = ibkr_web_api.AlertApi(api_client)
    id = 'id_example' # str | alert id

    try:
        # Get details of an alert
        api_response = api_instance.iserver_account_alert_id_get(id)
        print("The response of AlertApi->iserver_account_alert_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlertApi->iserver_account_alert_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| alert id | 

### Return type

[**AlertResponse**](AlertResponse.md)

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

# **iserver_account_mta_get**
> AlertResponse iserver_account_mta_get()

Get MTA alert

Each login user only has one mobile trading assistant (MTA) alert with it's own unique tool id.
The tool id cannot be changed. When modified a new order Id is generated. MTA alerts can not
be created or deleted. If you call delete /iserver/account/:accountId/alert/:alertId,
it will reset MTA to default. See [here](https://www.interactivebrokers.com/en/software/mobileiphonemobile/mobileiphone.htm#monitor/trading-assistant.htm) for more information on MTA alerts.


### Example


```python
import ibkr_web_api
from ibkr_web_api.models.alert_response import AlertResponse
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
    api_instance = ibkr_web_api.AlertApi(api_client)

    try:
        # Get MTA alert
        api_response = api_instance.iserver_account_mta_get()
        print("The response of AlertApi->iserver_account_mta_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlertApi->iserver_account_mta_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**AlertResponse**](AlertResponse.md)

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


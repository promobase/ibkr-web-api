# openapi_client.FYIApi

All URIs are relative to *http://localhost:5000/v1/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fyi_deliveryoptions_device_id_delete**](FYIApi.md#fyi_deliveryoptions_device_id_delete) | **DELETE** /fyi/deliveryoptions/{deviceId} | Delete a device
[**fyi_deliveryoptions_device_post**](FYIApi.md#fyi_deliveryoptions_device_post) | **POST** /fyi/deliveryoptions/device | Enable/Disable device option
[**fyi_deliveryoptions_email_put**](FYIApi.md#fyi_deliveryoptions_email_put) | **PUT** /fyi/deliveryoptions/email | Enable/Disable email option
[**fyi_deliveryoptions_get**](FYIApi.md#fyi_deliveryoptions_get) | **GET** /fyi/deliveryoptions | Get delivery options
[**fyi_disclaimer_typecode_get**](FYIApi.md#fyi_disclaimer_typecode_get) | **GET** /fyi/disclaimer/{typecode} | Get disclaimer for a certain kind of fyi
[**fyi_disclaimer_typecode_put**](FYIApi.md#fyi_disclaimer_typecode_put) | **PUT** /fyi/disclaimer/{typecode} | Mark disclaimer read
[**fyi_notifications_get**](FYIApi.md#fyi_notifications_get) | **GET** /fyi/notifications | Get a list of notifications
[**fyi_notifications_more_get**](FYIApi.md#fyi_notifications_more_get) | **GET** /fyi/notifications/more | Get more notifications based on a certain one
[**fyi_notifications_notification_id_put**](FYIApi.md#fyi_notifications_notification_id_put) | **PUT** /fyi/notifications/{notificationId} | Get a list of notifications
[**fyi_settings_get**](FYIApi.md#fyi_settings_get) | **GET** /fyi/settings | Get a list of subscriptions
[**fyi_settings_typecode_post**](FYIApi.md#fyi_settings_typecode_post) | **POST** /fyi/settings/{typecode} | Enable/Disable certain subscription
[**fyi_unreadnumber_get**](FYIApi.md#fyi_unreadnumber_get) | **GET** /fyi/unreadnumber | Get unread number of fyis. The HTTP method POST is also supported.


# **fyi_deliveryoptions_device_id_delete**
> object fyi_deliveryoptions_device_id_delete(device_id)

Delete a device

### Example


```python
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.FYIApi(api_client)
    device_id = 'device_id_example' # str | device ID

    try:
        # Delete a device
        api_response = api_instance.fyi_deliveryoptions_device_id_delete(device_id)
        print("The response of FYIApi->fyi_deliveryoptions_device_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FYIApi->fyi_deliveryoptions_device_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **device_id** | **str**| device ID | 

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
**200** | 200 means successful |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fyi_deliveryoptions_device_post**
> FyiDisclaimerTypecodePut200Response fyi_deliveryoptions_device_post(body)

Enable/Disable device option

### Example


```python
import openapi_client
from openapi_client.models.fyi_deliveryoptions_device_post_request import FyiDeliveryoptionsDevicePostRequest
from openapi_client.models.fyi_disclaimer_typecode_put200_response import FyiDisclaimerTypecodePut200Response
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.FYIApi(api_client)
    body = openapi_client.FyiDeliveryoptionsDevicePostRequest() # FyiDeliveryoptionsDevicePostRequest | device info

    try:
        # Enable/Disable device option
        api_response = api_instance.fyi_deliveryoptions_device_post(body)
        print("The response of FYIApi->fyi_deliveryoptions_device_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FYIApi->fyi_deliveryoptions_device_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**FyiDeliveryoptionsDevicePostRequest**](FyiDeliveryoptionsDevicePostRequest.md)| device info | 

### Return type

[**FyiDisclaimerTypecodePut200Response**](FyiDisclaimerTypecodePut200Response.md)

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

# **fyi_deliveryoptions_email_put**
> FyiDisclaimerTypecodePut200Response fyi_deliveryoptions_email_put(enabled)

Enable/Disable email option

### Example


```python
import openapi_client
from openapi_client.models.fyi_disclaimer_typecode_put200_response import FyiDisclaimerTypecodePut200Response
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.FYIApi(api_client)
    enabled = 'enabled_example' # str | true/false

    try:
        # Enable/Disable email option
        api_response = api_instance.fyi_deliveryoptions_email_put(enabled)
        print("The response of FYIApi->fyi_deliveryoptions_email_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FYIApi->fyi_deliveryoptions_email_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **enabled** | **str**| true/false | 

### Return type

[**FyiDisclaimerTypecodePut200Response**](FyiDisclaimerTypecodePut200Response.md)

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

# **fyi_deliveryoptions_get**
> FyiDeliveryoptionsGet200Response fyi_deliveryoptions_get()

Get delivery options

options for sending fyis to email and other devices


### Example


```python
import openapi_client
from openapi_client.models.fyi_deliveryoptions_get200_response import FyiDeliveryoptionsGet200Response
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.FYIApi(api_client)

    try:
        # Get delivery options
        api_response = api_instance.fyi_deliveryoptions_get()
        print("The response of FYIApi->fyi_deliveryoptions_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FYIApi->fyi_deliveryoptions_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**FyiDeliveryoptionsGet200Response**](FyiDeliveryoptionsGet200Response.md)

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

# **fyi_disclaimer_typecode_get**
> FyiDisclaimerTypecodeGet200Response fyi_disclaimer_typecode_get(typecode)

Get disclaimer for a certain kind of fyi

### Example


```python
import openapi_client
from openapi_client.models.fyi_disclaimer_typecode_get200_response import FyiDisclaimerTypecodeGet200Response
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.FYIApi(api_client)
    typecode = 'typecode_example' # str | fyi code, for example --M8, EA

    try:
        # Get disclaimer for a certain kind of fyi
        api_response = api_instance.fyi_disclaimer_typecode_get(typecode)
        print("The response of FYIApi->fyi_disclaimer_typecode_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FYIApi->fyi_disclaimer_typecode_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **typecode** | **str**| fyi code, for example --M8, EA | 

### Return type

[**FyiDisclaimerTypecodeGet200Response**](FyiDisclaimerTypecodeGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | receives the disclaimer message |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fyi_disclaimer_typecode_put**
> FyiDisclaimerTypecodePut200Response fyi_disclaimer_typecode_put(typecode)

Mark disclaimer read

### Example


```python
import openapi_client
from openapi_client.models.fyi_disclaimer_typecode_put200_response import FyiDisclaimerTypecodePut200Response
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.FYIApi(api_client)
    typecode = 'typecode_example' # str | fyi code, for example --M8, EA

    try:
        # Mark disclaimer read
        api_response = api_instance.fyi_disclaimer_typecode_put(typecode)
        print("The response of FYIApi->fyi_disclaimer_typecode_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FYIApi->fyi_disclaimer_typecode_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **typecode** | **str**| fyi code, for example --M8, EA | 

### Return type

[**FyiDisclaimerTypecodePut200Response**](FyiDisclaimerTypecodePut200Response.md)

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

# **fyi_notifications_get**
> List[NotificationsInner] fyi_notifications_get(max, exclude=exclude, include=include)

Get a list of notifications

### Example


```python
import openapi_client
from openapi_client.models.notifications_inner import NotificationsInner
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.FYIApi(api_client)
    max = 'max_example' # str | max number of fyis in response
    exclude = 'exclude_example' # str | if set, don't set include (optional)
    include = 'include_example' # str | if set, don't set exclude (optional)

    try:
        # Get a list of notifications
        api_response = api_instance.fyi_notifications_get(max, exclude=exclude, include=include)
        print("The response of FYIApi->fyi_notifications_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FYIApi->fyi_notifications_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **max** | **str**| max number of fyis in response | 
 **exclude** | **str**| if set, don&#39;t set include | [optional] 
 **include** | **str**| if set, don&#39;t set exclude | [optional] 

### Return type

[**List[NotificationsInner]**](NotificationsInner.md)

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

# **fyi_notifications_more_get**
> List[NotificationsInner] fyi_notifications_more_get(id)

Get more notifications based on a certain one

### Example


```python
import openapi_client
from openapi_client.models.notifications_inner import NotificationsInner
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.FYIApi(api_client)
    id = 'id_example' # str | id of last notification in the list

    try:
        # Get more notifications based on a certain one
        api_response = api_instance.fyi_notifications_more_get(id)
        print("The response of FYIApi->fyi_notifications_more_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FYIApi->fyi_notifications_more_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| id of last notification in the list | 

### Return type

[**List[NotificationsInner]**](NotificationsInner.md)

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

# **fyi_notifications_notification_id_put**
> object fyi_notifications_notification_id_put(notification_id)

Get a list of notifications

### Example


```python
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.FYIApi(api_client)
    notification_id = 'notification_id_example' # str | mark a notification read

    try:
        # Get a list of notifications
        api_response = api_instance.fyi_notifications_notification_id_put(notification_id)
        print("The response of FYIApi->fyi_notifications_notification_id_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FYIApi->fyi_notifications_notification_id_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **notification_id** | **str**| mark a notification read | 

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
**200** | when 200 receives, it means successful |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fyi_settings_get**
> List[FyiSettingsGet200ResponseInner] fyi_settings_get()

Get a list of subscriptions

Return the current choices of subscriptions, we can toggle the option


### Example


```python
import openapi_client
from openapi_client.models.fyi_settings_get200_response_inner import FyiSettingsGet200ResponseInner
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.FYIApi(api_client)

    try:
        # Get a list of subscriptions
        api_response = api_instance.fyi_settings_get()
        print("The response of FYIApi->fyi_settings_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FYIApi->fyi_settings_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[FyiSettingsGet200ResponseInner]**](FyiSettingsGet200ResponseInner.md)

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

# **fyi_settings_typecode_post**
> object fyi_settings_typecode_post(typecode, body)

Enable/Disable certain subscription

Configure which typecode you would like to enable/disable.


### Example


```python
import openapi_client
from openapi_client.models.fyi_settings_typecode_post_request import FyiSettingsTypecodePostRequest
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.FYIApi(api_client)
    typecode = 'typecode_example' # str | fyi code
    body = openapi_client.FyiSettingsTypecodePostRequest() # FyiSettingsTypecodePostRequest | 

    try:
        # Enable/Disable certain subscription
        api_response = api_instance.fyi_settings_typecode_post(typecode, body)
        print("The response of FYIApi->fyi_settings_typecode_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FYIApi->fyi_settings_typecode_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **typecode** | **str**| fyi code | 
 **body** | [**FyiSettingsTypecodePostRequest**](FyiSettingsTypecodePostRequest.md)|  | 

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
**200** | 200 means successful |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fyi_unreadnumber_get**
> FyiUnreadnumberGet200Response fyi_unreadnumber_get()

Get unread number of fyis. The HTTP method POST is also supported.

Returns the total number of unread fyis


### Example


```python
import openapi_client
from openapi_client.models.fyi_unreadnumber_get200_response import FyiUnreadnumberGet200Response
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:5000/v1/api
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:5000/v1/api"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.FYIApi(api_client)

    try:
        # Get unread number of fyis. The HTTP method POST is also supported.
        api_response = api_instance.fyi_unreadnumber_get()
        print("The response of FYIApi->fyi_unreadnumber_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FYIApi->fyi_unreadnumber_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**FyiUnreadnumberGet200Response**](FyiUnreadnumberGet200Response.md)

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


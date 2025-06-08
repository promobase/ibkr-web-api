# ibkr-web-api.ScannerApi

All URIs are relative to *http://localhost:5000/v1/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**hmds_scanner_post**](ScannerApi.md#hmds_scanner_post) | **POST** /hmds/scanner | Run Scanner (Beta)
[**iserver_scanner_params_get**](ScannerApi.md#iserver_scanner_params_get) | **GET** /iserver/scanner/params | Scanner Parameters
[**iserver_scanner_run_post**](ScannerApi.md#iserver_scanner_run_post) | **POST** /iserver/scanner/run | Scanner Run


# **hmds_scanner_post**
> ScannerResult hmds_scanner_post(body)

Run Scanner (Beta)

Using a direct connection to the market data farm, will provide results to the requested scanner.

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.hmds_scanner_post_request import HmdsScannerPostRequest
from ibkr-web-api.models.scanner_result import ScannerResult
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
    api_instance = ibkr-web-api.ScannerApi(api_client)
    body = ibkr-web-api.HmdsScannerPostRequest() # HmdsScannerPostRequest | request body

    try:
        # Run Scanner (Beta)
        api_response = api_instance.hmds_scanner_post(body)
        print("The response of ScannerApi->hmds_scanner_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ScannerApi->hmds_scanner_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**HmdsScannerPostRequest**](HmdsScannerPostRequest.md)| request body | 

### Return type

[**ScannerResult**](ScannerResult.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Bad request |  -  |
**200** | Valid result |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **iserver_scanner_params_get**
> IserverScannerParamsGet200Response iserver_scanner_params_get()

Scanner Parameters

Returns an object contains four lists contain all parameters for scanners

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.iserver_scanner_params_get200_response import IserverScannerParamsGet200Response
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
    api_instance = ibkr-web-api.ScannerApi(api_client)

    try:
        # Scanner Parameters
        api_response = api_instance.iserver_scanner_params_get()
        print("The response of ScannerApi->iserver_scanner_params_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ScannerApi->iserver_scanner_params_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**IserverScannerParamsGet200Response**](IserverScannerParamsGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | An object contains lists |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **iserver_scanner_run_post**
> List[IserverScannerRunPost200ResponseInner] iserver_scanner_run_post(body)

Scanner Run

Searches for contracts according to the filters specified in scanner/params endpoint

### Example


```python
import ibkr-web-api
from ibkr-web-api.models.iserver_scanner_run_post200_response_inner import IserverScannerRunPost200ResponseInner
from ibkr-web-api.models.scanner_params import ScannerParams
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
    api_instance = ibkr-web-api.ScannerApi(api_client)
    body = ibkr-web-api.ScannerParams() # ScannerParams | scanner-params request

    try:
        # Scanner Run
        api_response = api_instance.iserver_scanner_run_post(body)
        print("The response of ScannerApi->iserver_scanner_run_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ScannerApi->iserver_scanner_run_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**ScannerParams**](ScannerParams.md)| scanner-params request | 

### Return type

[**List[IserverScannerRunPost200ResponseInner]**](IserverScannerRunPost200ResponseInner.md)

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


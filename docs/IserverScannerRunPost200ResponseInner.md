# IserverScannerRunPost200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**server_id** | **str** |  | [optional] 
**column_name** | **str** |  | [optional] 
**symbol** | **str** | Underlying symbol | [optional] 
**conidex** | **str** | conid and exchange. Format supports conid or conid@exchange | [optional] 
**con_id** | **float** |  | [optional] 
**available_chart_periods** | **str** | List of available chart periods | [optional] 
**company_name** | **str** | Contracts company name | [optional] 
**contract_description_1** | **str** | Format contract name | [optional] 
**listing_exchange** | **str** |  | [optional] 
**sec_type** | **str** |  | [optional] 

## Example

```python
from ibkr_web_api.models.iserver_scanner_run_post200_response_inner import IserverScannerRunPost200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of IserverScannerRunPost200ResponseInner from a JSON string
iserver_scanner_run_post200_response_inner_instance = IserverScannerRunPost200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(IserverScannerRunPost200ResponseInner.to_json())

# convert the object into a dict
iserver_scanner_run_post200_response_inner_dict = iserver_scanner_run_post200_response_inner_instance.to_dict()
# create an instance of IserverScannerRunPost200ResponseInner from a dict
iserver_scanner_run_post200_response_inner_from_dict = IserverScannerRunPost200ResponseInner.from_dict(iserver_scanner_run_post200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



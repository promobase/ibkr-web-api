# IserverMarketdataSnapshotGet400Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**error** | **str** |  | [optional] 
**status_code** | **int** |  | [optional] 

## Example

```python
from ibkr_web_api.models.iserver_marketdata_snapshot_get400_response import IserverMarketdataSnapshotGet400Response

# TODO update the JSON string below
json = "{}"
# create an instance of IserverMarketdataSnapshotGet400Response from a JSON string
iserver_marketdata_snapshot_get400_response_instance = IserverMarketdataSnapshotGet400Response.from_json(json)
# print the JSON string representation of the object
print(IserverMarketdataSnapshotGet400Response.to_json())

# convert the object into a dict
iserver_marketdata_snapshot_get400_response_dict = iserver_marketdata_snapshot_get400_response_instance.to_dict()
# create an instance of IserverMarketdataSnapshotGet400Response from a dict
iserver_marketdata_snapshot_get400_response_from_dict = IserverMarketdataSnapshotGet400Response.from_dict(iserver_marketdata_snapshot_get400_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# IserverAccountAccountIdOrderWhatifPost200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | [**IserverAccountAccountIdOrderWhatifPost200ResponseAmount**](IserverAccountAccountIdOrderWhatifPost200ResponseAmount.md) |  | [optional] 
**equity** | [**IserverAccountAccountIdOrderWhatifPost200ResponseEquity**](IserverAccountAccountIdOrderWhatifPost200ResponseEquity.md) |  | [optional] 
**initial** | [**IserverAccountAccountIdOrderWhatifPost200ResponseEquity**](IserverAccountAccountIdOrderWhatifPost200ResponseEquity.md) |  | [optional] 
**maintenance** | [**IserverAccountAccountIdOrderWhatifPost200ResponseEquity**](IserverAccountAccountIdOrderWhatifPost200ResponseEquity.md) |  | [optional] 
**warn** | **str** |  | [optional] 
**error** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.iserver_account_account_id_order_whatif_post200_response import IserverAccountAccountIdOrderWhatifPost200Response

# TODO update the JSON string below
json = "{}"
# create an instance of IserverAccountAccountIdOrderWhatifPost200Response from a JSON string
iserver_account_account_id_order_whatif_post200_response_instance = IserverAccountAccountIdOrderWhatifPost200Response.from_json(json)
# print the JSON string representation of the object
print(IserverAccountAccountIdOrderWhatifPost200Response.to_json())

# convert the object into a dict
iserver_account_account_id_order_whatif_post200_response_dict = iserver_account_account_id_order_whatif_post200_response_instance.to_dict()
# create an instance of IserverAccountAccountIdOrderWhatifPost200Response from a dict
iserver_account_account_id_order_whatif_post200_response_from_dict = IserverAccountAccountIdOrderWhatifPost200Response.from_dict(iserver_account_account_id_order_whatif_post200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



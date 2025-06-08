# IserverAccountAccountIdOrderWhatifPost200ResponseAmount


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **str** | for example 23,000 USD | [optional] 
**commission** | **str** | for example 1.1 ... 1.2 USD | [optional] 
**total** | **str** |  | [optional] 

## Example

```python
from ibkr_web_api.models.iserver_account_account_id_order_whatif_post200_response_amount import IserverAccountAccountIdOrderWhatifPost200ResponseAmount

# TODO update the JSON string below
json = "{}"
# create an instance of IserverAccountAccountIdOrderWhatifPost200ResponseAmount from a JSON string
iserver_account_account_id_order_whatif_post200_response_amount_instance = IserverAccountAccountIdOrderWhatifPost200ResponseAmount.from_json(json)
# print the JSON string representation of the object
print(IserverAccountAccountIdOrderWhatifPost200ResponseAmount.to_json())

# convert the object into a dict
iserver_account_account_id_order_whatif_post200_response_amount_dict = iserver_account_account_id_order_whatif_post200_response_amount_instance.to_dict()
# create an instance of IserverAccountAccountIdOrderWhatifPost200ResponseAmount from a dict
iserver_account_account_id_order_whatif_post200_response_amount_from_dict = IserverAccountAccountIdOrderWhatifPost200ResponseAmount.from_dict(iserver_account_account_id_order_whatif_post200_response_amount_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



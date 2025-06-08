# IserverContractConidAlgosGet200ResponseInnerParametersInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | The algo parameter | 
**required** | **bool** | If true a value must be entered. | [optional] 
**name** | **str** | Descriptive name of the parameter. | [optional] 
**value_class_name** | **str** | Format of the parameter. | 
**min_value** | **float** | Smallest value, only applies to parameters with valueClassName&#x3D;Double. | [optional] 
**max_value** | **float** | Largest value, only applies to parameters with valueClassName&#x3D;Double. | [optional] 
**default_value** | **bool** | User configured preset for this parameter. | [optional] 
**legal_strings** | **str** | The list of choices | [optional] 
**description** | **str** | Detailed description of the parameter. | [optional] 
**gui_rank** | **float** | The order in UI, used when building dynamic UI so that more important parameters are presented first. | [optional] 
**price_market_rule** | **bool** | If true, must specify parameter using market rule format. Only applies to parameters with valueClassName&#x3D;Double. | [optional] 
**enabled_conditions** | **str** | The rules that UI should apply to algo parameters depending on chosen order type:  * MKT:speedUp:&#x3D;:no - hide SpeedUp param when MKT is chosen for order type.  * LMT:strategyType:&lt;&gt;:empty - strategyType param cannot be empty when LMT is chosen for order type.  * MKT:strategyType:&#x3D;:Marketable - set strategyType param to Marketable and disable (no other choice) when MKT is chosen for order type.  | [optional] 

## Example

```python
from ibkr_web_api.models.iserver_contract_conid_algos_get200_response_inner_parameters_inner import IserverContractConidAlgosGet200ResponseInnerParametersInner

# TODO update the JSON string below
json = "{}"
# create an instance of IserverContractConidAlgosGet200ResponseInnerParametersInner from a JSON string
iserver_contract_conid_algos_get200_response_inner_parameters_inner_instance = IserverContractConidAlgosGet200ResponseInnerParametersInner.from_json(json)
# print the JSON string representation of the object
print(IserverContractConidAlgosGet200ResponseInnerParametersInner.to_json())

# convert the object into a dict
iserver_contract_conid_algos_get200_response_inner_parameters_inner_dict = iserver_contract_conid_algos_get200_response_inner_parameters_inner_instance.to_dict()
# create an instance of IserverContractConidAlgosGet200ResponseInnerParametersInner from a dict
iserver_contract_conid_algos_get200_response_inner_parameters_inner_from_dict = IserverContractConidAlgosGet200ResponseInnerParametersInner.from_dict(iserver_contract_conid_algos_get200_response_inner_parameters_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



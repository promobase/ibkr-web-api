# Transactions

account transactions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | will always be getTransactions | [optional] 
**currency** | **str** | same as request | [optional] 
**includes_real_time** | **bool** | Indicates whether current day and realtime data is included in the result | [optional] 
**var_from** | **float** | Period start date. Epoch time, GMT | [optional] 
**to** | **float** | Period end date. Epoch time, GMT | [optional] 
**transactions** | [**List[TransactionsTransactionsInner]**](TransactionsTransactionsInner.md) | Sorted by date descending | [optional] 

## Example

```python
from ibkr_web_api.models.transactions import Transactions

# TODO update the JSON string below
json = "{}"
# create an instance of Transactions from a JSON string
transactions_instance = Transactions.from_json(json)
# print the JSON string representation of the object
print(Transactions.to_json())

# convert the object into a dict
transactions_dict = transactions_instance.to_dict()
# create an instance of Transactions from a dict
transactions_from_dict = Transactions.from_dict(transactions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



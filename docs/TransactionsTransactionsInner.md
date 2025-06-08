# TransactionsTransactionsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**acctid** | **str** |  | [optional] 
**conid** | **float** |  | [optional] 
**cur** | **str** | currency code | [optional] 
**fx_rate** | **float** | Conversion rate from asset currency to response currency | [optional] 
**desc** | **str** | Transaction description | [optional] 
**var_date** | **str** | Date of transaction.  Epoch time, GMT | [optional] 
**type** | **str** | Transaction Type Name: Examples: \&quot;Sell\&quot;, \&quot;Buy\&quot;, \&quot;Corporate Action\&quot;, \&quot;Dividend Payment\&quot;, \&quot;Transfer\&quot;, \&quot;Payment in Lieu\&quot; Dividends and Transfers do not have price and quantity in response  | [optional] 
**qty** | **float** | Not applicable for all transaction types | [optional] 
**pr** | **float** | In asset currency. Not be applicable for all transaction types. | [optional] 
**amt** | **float** | Raw value, no formatting. Net transaction amount (may include commission, tax). In asset currency | [optional] 

## Example

```python
from openapi_client.models.transactions_transactions_inner import TransactionsTransactionsInner

# TODO update the JSON string below
json = "{}"
# create an instance of TransactionsTransactionsInner from a JSON string
transactions_transactions_inner_instance = TransactionsTransactionsInner.from_json(json)
# print the JSON string representation of the object
print(TransactionsTransactionsInner.to_json())

# convert the object into a dict
transactions_transactions_inner_dict = transactions_transactions_inner_instance.to_dict()
# create an instance of TransactionsTransactionsInner from a dict
transactions_transactions_inner_from_dict = TransactionsTransactionsInner.from_dict(transactions_transactions_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



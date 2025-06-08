# IserverReplyReplyidPost400Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**error** | **str** | for example-order not confirmed | [optional] 
**status_code** | **int** |  | [optional] 

## Example

```python
from ibkr-web-api.models.iserver_reply_replyid_post400_response import IserverReplyReplyidPost400Response

# TODO update the JSON string below
json = "{}"
# create an instance of IserverReplyReplyidPost400Response from a JSON string
iserver_reply_replyid_post400_response_instance = IserverReplyReplyidPost400Response.from_json(json)
# print the JSON string representation of the object
print(IserverReplyReplyidPost400Response.to_json())

# convert the object into a dict
iserver_reply_replyid_post400_response_dict = iserver_reply_replyid_post400_response_instance.to_dict()
# create an instance of IserverReplyReplyidPost400Response from a dict
iserver_reply_replyid_post400_response_from_dict = IserverReplyReplyidPost400Response.from_dict(iserver_reply_replyid_post400_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# IserverReplyReplyidPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**confirmed** | **bool** | answer to question, true means yes, false means no | [optional] 

## Example

```python
from ibkr-web-api.models.iserver_reply_replyid_post_request import IserverReplyReplyidPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IserverReplyReplyidPostRequest from a JSON string
iserver_reply_replyid_post_request_instance = IserverReplyReplyidPostRequest.from_json(json)
# print the JSON string representation of the object
print(IserverReplyReplyidPostRequest.to_json())

# convert the object into a dict
iserver_reply_replyid_post_request_dict = iserver_reply_replyid_post_request_instance.to_dict()
# create an instance of IserverReplyReplyidPostRequest from a dict
iserver_reply_replyid_post_request_from_dict = IserverReplyReplyidPostRequest.from_dict(iserver_reply_replyid_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



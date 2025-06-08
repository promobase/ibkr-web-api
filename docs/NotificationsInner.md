# NotificationsInner

notification

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**d** | **str** | notification date | [optional] 
**id** | **str** | unique way to reference this notification | [optional] 
**fc** | **str** | FYI code, we can use it to find whether the disclaimer is accepted or not in settings | [optional] 
**md** | **str** | content of notification | [optional] 
**ms** | **str** | title of notification | [optional] 
**r** | **str** | 0-unread, 1-read | [optional] 

## Example

```python
from ibkr_web_api.models.notifications_inner import NotificationsInner

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationsInner from a JSON string
notifications_inner_instance = NotificationsInner.from_json(json)
# print the JSON string representation of the object
print(NotificationsInner.to_json())

# convert the object into a dict
notifications_inner_dict = notifications_inner_instance.to_dict()
# create an instance of NotificationsInner from a dict
notifications_inner_from_dict = NotificationsInner.from_dict(notifications_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



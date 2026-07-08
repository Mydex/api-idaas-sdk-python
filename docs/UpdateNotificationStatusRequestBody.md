# UpdateNotificationStatusRequestBody

Request body for updating notification status

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**identifier** | **UUID** | The notification identifier to update | 

## Example

```python
from api_idaas_sdk.models.update_notification_status_request_body import UpdateNotificationStatusRequestBody

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateNotificationStatusRequestBody from a JSON string
update_notification_status_request_body_instance = UpdateNotificationStatusRequestBody.from_json(json)
# print the JSON string representation of the object
print(UpdateNotificationStatusRequestBody.to_json())

# convert the object into a dict
update_notification_status_request_body_dict = update_notification_status_request_body_instance.to_dict()
# create an instance of UpdateNotificationStatusRequestBody from a dict
update_notification_status_request_body_from_dict = UpdateNotificationStatusRequestBody.from_dict(update_notification_status_request_body_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



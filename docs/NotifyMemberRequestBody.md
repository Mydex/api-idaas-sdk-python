# NotifyMemberRequestBody

Request body for sending a notification to a member

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**identifier_auth** | [**IdentifierAuthObject**](IdentifierAuthObject.md) |  | 
**message_email** | **str** | Email message content | 
**message_sms** | **str** | SMS message content | [optional] 

## Example

```python
from api_idaas_sdk.models.notify_member_request_body import NotifyMemberRequestBody

# TODO update the JSON string below
json = "{}"
# create an instance of NotifyMemberRequestBody from a JSON string
notify_member_request_body_instance = NotifyMemberRequestBody.from_json(json)
# print the JSON string representation of the object
print(NotifyMemberRequestBody.to_json())

# convert the object into a dict
notify_member_request_body_dict = notify_member_request_body_instance.to_dict()
# create an instance of NotifyMemberRequestBody from a dict
notify_member_request_body_from_dict = NotifyMemberRequestBody.from_dict(notify_member_request_body_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



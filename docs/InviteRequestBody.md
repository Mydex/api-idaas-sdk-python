# InviteRequestBody

Request body for storing and sending an identifier invite

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**identifier** | **UUID** | The parent identifier | 
**app_url** | **str** | The application URL | 
**client_id** | **str** | The OAuth2 client ID | 
**con_nid** | **str** | The connection NID | 
**org_id** | **str** | The organization ID | 
**project_id** | **str** | The project ID | 
**item_id** | **str** | The item ID | 
**type** | **str** | The type of invitation | 
**message_email** | **str** | Email message content | 
**message_sms** | **str** | SMS message content | [optional] 

## Example

```python
from api_idaas_sdk.models.invite_request_body import InviteRequestBody

# TODO update the JSON string below
json = "{}"
# create an instance of InviteRequestBody from a JSON string
invite_request_body_instance = InviteRequestBody.from_json(json)
# print the JSON string representation of the object
print(InviteRequestBody.to_json())

# convert the object into a dict
invite_request_body_dict = invite_request_body_instance.to_dict()
# create an instance of InviteRequestBody from a dict
invite_request_body_from_dict = InviteRequestBody.from_dict(invite_request_body_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



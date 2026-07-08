# InviteStatusRequestBody

Request body for checking invite status

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**identifier** | **UUID** | The parent identifier | 
**app_url** | **str** |  | 
**client_id** | **str** |  | 
**con_nid** | **str** |  | 
**org_id** | **str** |  | 
**project_id** | **str** |  | 
**item_id** | **str** |  | 
**type** | **str** |  | 

## Example

```python
from api_idaas_sdk.models.invite_status_request_body import InviteStatusRequestBody

# TODO update the JSON string below
json = "{}"
# create an instance of InviteStatusRequestBody from a JSON string
invite_status_request_body_instance = InviteStatusRequestBody.from_json(json)
# print the JSON string representation of the object
print(InviteStatusRequestBody.to_json())

# convert the object into a dict
invite_status_request_body_dict = invite_status_request_body_instance.to_dict()
# create an instance of InviteStatusRequestBody from a dict
invite_status_request_body_from_dict = InviteStatusRequestBody.from_dict(invite_status_request_body_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



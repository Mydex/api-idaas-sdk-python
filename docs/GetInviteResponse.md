# GetInviteResponse

Response when getting an invitation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **int** |  | [optional] 
**invite_url_code** | **str** | The invitation URL code | [optional] 
**parent_uuid** | **UUID** | The parent identifier UUID | [optional] 
**app_url** | **str** | The application URL | [optional] 
**client_id** | **str** | The OAuth2 client ID | [optional] 
**con_nid** | **str** | The connection NID | [optional] 
**org_id** | **str** | The organization ID | [optional] 
**project_id** | **str** | The project ID | [optional] 
**item_id** | **str** | The item ID | [optional] 
**type** | **str** | The type of invitation | [optional] 

## Example

```python
from api_idaas_sdk.models.get_invite_response import GetInviteResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GetInviteResponse from a JSON string
get_invite_response_instance = GetInviteResponse.from_json(json)
# print the JSON string representation of the object
print(GetInviteResponse.to_json())

# convert the object into a dict
get_invite_response_dict = get_invite_response_instance.to_dict()
# create an instance of GetInviteResponse from a dict
get_invite_response_from_dict = GetInviteResponse.from_dict(get_invite_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



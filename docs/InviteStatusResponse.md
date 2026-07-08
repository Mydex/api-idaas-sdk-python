# InviteStatusResponse

Response for checking invite status

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **int** | Whether the invite exists | [optional] 
**status** | **str** | The status of the invite (pending, used, expired) | [optional] 

## Example

```python
from api_idaas_sdk.models.invite_status_response import InviteStatusResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InviteStatusResponse from a JSON string
invite_status_response_instance = InviteStatusResponse.from_json(json)
# print the JSON string representation of the object
print(InviteStatusResponse.to_json())

# convert the object into a dict
invite_status_response_dict = invite_status_response_instance.to_dict()
# create an instance of InviteStatusResponse from a dict
invite_status_response_from_dict = InviteStatusResponse.from_dict(invite_status_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AuthErrorResponseError


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**reason** | **str** |  | [optional] 

## Example

```python
from api_idaas_sdk.models.auth_error_response_error import AuthErrorResponseError

# TODO update the JSON string below
json = "{}"
# create an instance of AuthErrorResponseError from a JSON string
auth_error_response_error_instance = AuthErrorResponseError.from_json(json)
# print the JSON string representation of the object
print(AuthErrorResponseError.to_json())

# convert the object into a dict
auth_error_response_error_dict = auth_error_response_error_instance.to_dict()
# create an instance of AuthErrorResponseError from a dict
auth_error_response_error_from_dict = AuthErrorResponseError.from_dict(auth_error_response_error_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# IdentifierAuthObject

Authentication data for an identifier

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**parent_uuid** | **UUID** | The parent identifier UUID | [optional] 
**app_url** | **str** | The application URL | [optional] 
**client_id** | **str** | The OAuth2 client ID | [optional] 
**con_nid** | **str** | The connection NID | [optional] 
**org_id** | **str** | The organization ID | [optional] 
**project_id** | **str** | The project ID | [optional] 
**item_id** | **str** | The item ID | [optional] 
**type** | **str** | The type of identifier/auth | [optional] 

## Example

```python
from api_idaas_sdk.models.identifier_auth_object import IdentifierAuthObject

# TODO update the JSON string below
json = "{}"
# create an instance of IdentifierAuthObject from a JSON string
identifier_auth_object_instance = IdentifierAuthObject.from_json(json)
# print the JSON string representation of the object
print(IdentifierAuthObject.to_json())

# convert the object into a dict
identifier_auth_object_dict = identifier_auth_object_instance.to_dict()
# create an instance of IdentifierAuthObject from a dict
identifier_auth_object_from_dict = IdentifierAuthObject.from_dict(identifier_auth_object_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



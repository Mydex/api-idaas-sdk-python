# IdentifierObject

An identifier record

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Database ID of the identifier | [optional] 
**identifier** | **UUID** | The UUID identifier | [optional] 
**parent_uuid** | **UUID** | The parent identifier UUID if this is a child | [optional] 
**type** | **str** | The type of identifier | [optional] 
**created** | **str** | Creation timestamp | [optional] 

## Example

```python
from api_idaas_sdk.models.identifier_object import IdentifierObject

# TODO update the JSON string below
json = "{}"
# create an instance of IdentifierObject from a JSON string
identifier_object_instance = IdentifierObject.from_json(json)
# print the JSON string representation of the object
print(IdentifierObject.to_json())

# convert the object into a dict
identifier_object_dict = identifier_object_instance.to_dict()
# create an instance of IdentifierObject from a dict
identifier_object_from_dict = IdentifierObject.from_dict(identifier_object_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



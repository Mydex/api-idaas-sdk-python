# GetIdentifiersResponse

Response when getting all identifiers for a member

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **int** |  | [optional] 
**identifiers** | [**List[IdentifierObject]**](IdentifierObject.md) |  | [optional] 

## Example

```python
from api_idaas_sdk.models.get_identifiers_response import GetIdentifiersResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GetIdentifiersResponse from a JSON string
get_identifiers_response_instance = GetIdentifiersResponse.from_json(json)
# print the JSON string representation of the object
print(GetIdentifiersResponse.to_json())

# convert the object into a dict
get_identifiers_response_dict = get_identifiers_response_instance.to_dict()
# create an instance of GetIdentifiersResponse from a dict
get_identifiers_response_from_dict = GetIdentifiersResponse.from_dict(get_identifiers_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CreateIdentifierResponse

Response when creating an identifier

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **int** | Whether the operation succeeded | [optional] 
**identifier** | **UUID** | The newly created identifier UUID | [optional] 

## Example

```python
from api_idaas_sdk.models.create_identifier_response import CreateIdentifierResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CreateIdentifierResponse from a JSON string
create_identifier_response_instance = CreateIdentifierResponse.from_json(json)
# print the JSON string representation of the object
print(CreateIdentifierResponse.to_json())

# convert the object into a dict
create_identifier_response_dict = create_identifier_response_instance.to_dict()
# create an instance of CreateIdentifierResponse from a dict
create_identifier_response_from_dict = CreateIdentifierResponse.from_dict(create_identifier_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



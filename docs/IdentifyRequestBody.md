# IdentifyRequestBody

Request body for identification URL setup

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**connection_nid** | **str** | The connection NID | 
**connection_token_hash** | **str** | The hashed connection token | 
**return_to** | **str** | The URL to return to after identification | 
**linking_token** | **str** | A unique ID representing the member in the subscriber&#39;s backend | [optional] 

## Example

```python
from api_idaas_sdk.models.identify_request_body import IdentifyRequestBody

# TODO update the JSON string below
json = "{}"
# create an instance of IdentifyRequestBody from a JSON string
identify_request_body_instance = IdentifyRequestBody.from_json(json)
# print the JSON string representation of the object
print(IdentifyRequestBody.to_json())

# convert the object into a dict
identify_request_body_dict = identify_request_body_instance.to_dict()
# create an instance of IdentifyRequestBody from a dict
identify_request_body_from_dict = IdentifyRequestBody.from_dict(identify_request_body_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



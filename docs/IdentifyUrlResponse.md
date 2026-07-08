# IdentifyUrlResponse

Response containing the Identify URL and QR code

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** | The one-time URL for FTC or identification | [optional] 
**qr** | **str** | QR code representation of the URL | [optional] 

## Example

```python
from api_idaas_sdk.models.identify_url_response import IdentifyUrlResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentifyUrlResponse from a JSON string
identify_url_response_instance = IdentifyUrlResponse.from_json(json)
# print the JSON string representation of the object
print(IdentifyUrlResponse.to_json())

# convert the object into a dict
identify_url_response_dict = identify_url_response_instance.to_dict()
# create an instance of IdentifyUrlResponse from a dict
identify_url_response_from_dict = IdentifyUrlResponse.from_dict(identify_url_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



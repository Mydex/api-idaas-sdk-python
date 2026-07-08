# FtcUrlResponse

Response containing the FTC URL and QR code

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** | The one-time URL for FTC or identification | [optional] 
**qr** | **str** | QR code representation of the URL | [optional] 

## Example

```python
from api_idaas_sdk.models.ftc_url_response import FtcUrlResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FtcUrlResponse from a JSON string
ftc_url_response_instance = FtcUrlResponse.from_json(json)
# print the JSON string representation of the object
print(FtcUrlResponse.to_json())

# convert the object into a dict
ftc_url_response_dict = ftc_url_response_instance.to_dict()
# create an instance of FtcUrlResponse from a dict
ftc_url_response_from_dict = FtcUrlResponse.from_dict(ftc_url_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



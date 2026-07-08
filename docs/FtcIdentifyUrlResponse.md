# FtcIdentifyUrlResponse

Response containing the FTC or Identify URL and QR code

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** | The one-time URL for FTC or identification | [optional] 
**qr** | **str** | QR code representation of the URL | [optional] 

## Example

```python
from api_idaas_sdk.models.ftc_identify_url_response import FtcIdentifyUrlResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FtcIdentifyUrlResponse from a JSON string
ftc_identify_url_response_instance = FtcIdentifyUrlResponse.from_json(json)
# print the JSON string representation of the object
print(FtcIdentifyUrlResponse.to_json())

# convert the object into a dict
ftc_identify_url_response_dict = ftc_identify_url_response_instance.to_dict()
# create an instance of FtcIdentifyUrlResponse from a dict
ftc_identify_url_response_from_dict = FtcIdentifyUrlResponse.from_dict(ftc_identify_url_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



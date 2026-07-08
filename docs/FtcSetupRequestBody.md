# FtcSetupRequestBody

Request body for First Time Connection setup

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**connection_nid** | **str** | The connection NID | 
**connection_token_hash** | **str** | The hashed connection token | 
**return_to** | **str** | The URL to return to after connection | 
**mydexid** | **str** | The MydexID if already known (required if version &gt; 1) | [optional] 
**version** | **int** | The connection version (default 1, must be &gt;&#x3D; 1) | [optional] 
**linking_token** | **str** | A unique ID representing the member in the subscriber&#39;s backend | [optional] 

## Example

```python
from api_idaas_sdk.models.ftc_setup_request_body import FtcSetupRequestBody

# TODO update the JSON string below
json = "{}"
# create an instance of FtcSetupRequestBody from a JSON string
ftc_setup_request_body_instance = FtcSetupRequestBody.from_json(json)
# print the JSON string representation of the object
print(FtcSetupRequestBody.to_json())

# convert the object into a dict
ftc_setup_request_body_dict = ftc_setup_request_body_instance.to_dict()
# create an instance of FtcSetupRequestBody from a dict
ftc_setup_request_body_from_dict = FtcSetupRequestBody.from_dict(ftc_setup_request_body_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



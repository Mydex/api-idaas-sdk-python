# api_idaas_sdk.ConnectionsApi

All URIs are relative to *https://idp.mydexid.org*

Method | HTTP request | Description
------------- | ------------- | -------------
[**post_ftc_setup**](ConnectionsApi.md#post_ftc_setup) | **POST** /ftc/setup | Set up a First Time Connection URL.
[**post_identify**](ConnectionsApi.md#post_identify) | **POST** /identify | Set up an identification URL.


# **post_ftc_setup**
> FtcUrlResponse post_ftc_setup(ftc_setup_request_body=ftc_setup_request_body)

Set up a First Time Connection URL.

Generates a one-time URL for a member to complete First Time Connection. Requires OAuth2.0 authentication.

### Example

* OAuth Authentication (oauth2):

```python
import api_idaas_sdk
from api_idaas_sdk.models.ftc_setup_request_body import FtcSetupRequestBody
from api_idaas_sdk.models.ftc_url_response import FtcUrlResponse
from api_idaas_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://idp.mydexid.org
# See configuration.py for a list of all supported configuration parameters.
configuration = api_idaas_sdk.Configuration(
    host = "https://idp.mydexid.org"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with api_idaas_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = api_idaas_sdk.ConnectionsApi(api_client)
    ftc_setup_request_body = api_idaas_sdk.FtcSetupRequestBody() # FtcSetupRequestBody |  (optional)

    try:
        # Set up a First Time Connection URL.
        api_response = api_instance.post_ftc_setup(ftc_setup_request_body=ftc_setup_request_body)
        print("The response of ConnectionsApi->post_ftc_setup:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsApi->post_ftc_setup: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ftc_setup_request_body** | [**FtcSetupRequestBody**](FtcSetupRequestBody.md)|  | [optional] 

### Return type

[**FtcUrlResponse**](FtcUrlResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Successfully created FTC setup URL. |  -  |
**400** | Bad Request |  -  |
**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_identify**
> IdentifyUrlResponse post_identify(identify_request_body=identify_request_body)

Set up an identification URL.

Generates a one-time URL for identifying a member without requiring them to know their MydexID. Requires OAuth2.0 authentication.

### Example

* OAuth Authentication (oauth2):

```python
import api_idaas_sdk
from api_idaas_sdk.models.identify_request_body import IdentifyRequestBody
from api_idaas_sdk.models.identify_url_response import IdentifyUrlResponse
from api_idaas_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://idp.mydexid.org
# See configuration.py for a list of all supported configuration parameters.
configuration = api_idaas_sdk.Configuration(
    host = "https://idp.mydexid.org"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with api_idaas_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = api_idaas_sdk.ConnectionsApi(api_client)
    identify_request_body = api_idaas_sdk.IdentifyRequestBody() # IdentifyRequestBody |  (optional)

    try:
        # Set up an identification URL.
        api_response = api_instance.post_identify(identify_request_body=identify_request_body)
        print("The response of ConnectionsApi->post_identify:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectionsApi->post_identify: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **identify_request_body** | [**IdentifyRequestBody**](IdentifyRequestBody.md)|  | [optional] 

### Return type

[**IdentifyUrlResponse**](IdentifyUrlResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Successfully created identify URL. |  -  |
**400** | Bad Request |  -  |
**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


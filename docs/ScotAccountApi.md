# api_idaas_sdk.ScotAccountApi

All URIs are relative to *https://idp.mydexid.org*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_mydex_id_from_scot_account_sub**](ScotAccountApi.md#get_mydex_id_from_scot_account_sub) | **GET** /members/scotaccount/{sub} | Check if a ScotAccount sub GUID has an associated MydexID.


# **get_mydex_id_from_scot_account_sub**
> str get_mydex_id_from_scot_account_sub(sub)

Check if a ScotAccount sub GUID has an associated MydexID.

Retrieves the MydexID associated with a ScotAccount GUID.

### Example

* OAuth Authentication (oauth2):

```python
import api_idaas_sdk
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
    api_instance = api_idaas_sdk.ScotAccountApi(api_client)
    sub = UUID('123e4567-e89b-12d3-a456-426614174000') # UUID | The ScotAccount GUID

    try:
        # Check if a ScotAccount sub GUID has an associated MydexID.
        api_response = api_instance.get_mydex_id_from_scot_account_sub(sub)
        print("The response of ScotAccountApi->get_mydex_id_from_scot_account_sub:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ScotAccountApi->get_mydex_id_from_scot_account_sub: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sub** | **UUID**| The ScotAccount GUID | 

### Return type

**str**

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successfully retrieved MydexID. |  -  |
**400** | Bad Request |  -  |
**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


# api_idaas_sdk.MyAccountApi

All URIs are relative to *https://idp.mydexid.org*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_mydex_id_from_my_account_svt**](MyAccountApi.md#get_mydex_id_from_my_account_svt) | **GET** /members/myaccount/{svt} | Check if a MyAccount SVT has an associated MydexID.


# **get_mydex_id_from_my_account_svt**
> str get_mydex_id_from_my_account_svt(svt)

Check if a MyAccount SVT has an associated MydexID.

Retrieves the MydexID associated with a MyAccount SVT.

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
    api_instance = api_idaas_sdk.MyAccountApi(api_client)
    svt = 'abc123xyz456' # str | The MyAccount security verification token

    try:
        # Check if a MyAccount SVT has an associated MydexID.
        api_response = api_instance.get_mydex_id_from_my_account_svt(svt)
        print("The response of MyAccountApi->get_mydex_id_from_my_account_svt:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MyAccountApi->get_mydex_id_from_my_account_svt: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **svt** | **str**| The MyAccount security verification token | 

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


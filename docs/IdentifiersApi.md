# api_idaas_sdk.IdentifiersApi

All URIs are relative to *https://idp.mydexid.org*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_identifier_invite**](IdentifiersApi.md#get_identifier_invite) | **GET** /members/invite/{invite} | Fetch an invitation code and identifier auth data.
[**patch_notify_status**](IdentifiersApi.md#patch_notify_status) | **PATCH** /members/notify/status | Update the status of a notification.
[**post_invite_status**](IdentifiersApi.md#post_invite_status) | **POST** /members/invite/status | Check the status of an invite.
[**post_notify_member_via_identifier**](IdentifiersApi.md#post_notify_member_via_identifier) | **POST** /members/notify | Send a notification to a member via its identifier.
[**post_store_and_send_identifier_invite**](IdentifiersApi.md#post_store_and_send_identifier_invite) | **POST** /members/invite | Store an invitation code and send notification.


# **get_identifier_invite**
> GetInviteResponse get_identifier_invite(invite)

Fetch an invitation code and identifier auth data.

Retrieves the invitation data for a given invite code.

### Example

* OAuth Authentication (oauth2):

```python
import api_idaas_sdk
from api_idaas_sdk.models.get_invite_response import GetInviteResponse
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
    api_instance = api_idaas_sdk.IdentifiersApi(api_client)
    invite = 'a1b2c3d4e5f6' # str | The invitation code

    try:
        # Fetch an invitation code and identifier auth data.
        api_response = api_instance.get_identifier_invite(invite)
        print("The response of IdentifiersApi->get_identifier_invite:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IdentifiersApi->get_identifier_invite: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invite** | **str**| The invitation code | 

### Return type

[**GetInviteResponse**](GetInviteResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successfully retrieved invitation. |  -  |
**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patch_notify_status**
> CreateIdentifierResponse patch_notify_status(update_notification_status_request_body=update_notification_status_request_body)

Update the status of a notification.

Updates the status of a notification identifier.

### Example

* OAuth Authentication (oauth2):

```python
import api_idaas_sdk
from api_idaas_sdk.models.create_identifier_response import CreateIdentifierResponse
from api_idaas_sdk.models.update_notification_status_request_body import UpdateNotificationStatusRequestBody
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
    api_instance = api_idaas_sdk.IdentifiersApi(api_client)
    update_notification_status_request_body = api_idaas_sdk.UpdateNotificationStatusRequestBody() # UpdateNotificationStatusRequestBody |  (optional)

    try:
        # Update the status of a notification.
        api_response = api_instance.patch_notify_status(update_notification_status_request_body=update_notification_status_request_body)
        print("The response of IdentifiersApi->patch_notify_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IdentifiersApi->patch_notify_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **update_notification_status_request_body** | [**UpdateNotificationStatusRequestBody**](UpdateNotificationStatusRequestBody.md)|  | [optional] 

### Return type

[**CreateIdentifierResponse**](CreateIdentifierResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successfully updated notification status. |  -  |
**400** | Bad Request |  -  |
**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_invite_status**
> InviteStatusResponse post_invite_status(invite_status_request_body=invite_status_request_body)

Check the status of an invite.

Checks the status of an invitation without modifying it.

### Example

* OAuth Authentication (oauth2):

```python
import api_idaas_sdk
from api_idaas_sdk.models.invite_status_request_body import InviteStatusRequestBody
from api_idaas_sdk.models.invite_status_response import InviteStatusResponse
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
    api_instance = api_idaas_sdk.IdentifiersApi(api_client)
    invite_status_request_body = api_idaas_sdk.InviteStatusRequestBody() # InviteStatusRequestBody |  (optional)

    try:
        # Check the status of an invite.
        api_response = api_instance.post_invite_status(invite_status_request_body=invite_status_request_body)
        print("The response of IdentifiersApi->post_invite_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IdentifiersApi->post_invite_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invite_status_request_body** | [**InviteStatusRequestBody**](InviteStatusRequestBody.md)|  | [optional] 

### Return type

[**InviteStatusResponse**](InviteStatusResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successfully checked invite status. |  -  |
**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_notify_member_via_identifier**
> CreateIdentifierResponse post_notify_member_via_identifier(notify_member_request_body=notify_member_request_body)

Send a notification to a member via its identifier.

Sends a notification (email or SMS) to a member using their identifier for authentication.

### Example

* OAuth Authentication (oauth2):

```python
import api_idaas_sdk
from api_idaas_sdk.models.create_identifier_response import CreateIdentifierResponse
from api_idaas_sdk.models.notify_member_request_body import NotifyMemberRequestBody
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
    api_instance = api_idaas_sdk.IdentifiersApi(api_client)
    notify_member_request_body = api_idaas_sdk.NotifyMemberRequestBody() # NotifyMemberRequestBody |  (optional)

    try:
        # Send a notification to a member via its identifier.
        api_response = api_instance.post_notify_member_via_identifier(notify_member_request_body=notify_member_request_body)
        print("The response of IdentifiersApi->post_notify_member_via_identifier:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IdentifiersApi->post_notify_member_via_identifier: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **notify_member_request_body** | [**NotifyMemberRequestBody**](NotifyMemberRequestBody.md)|  | [optional] 

### Return type

[**CreateIdentifierResponse**](CreateIdentifierResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successfully sent notification. |  -  |
**400** | Bad Request |  -  |
**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_store_and_send_identifier_invite**
> GetInviteResponse post_store_and_send_identifier_invite(invite_request_body=invite_request_body)

Store an invitation code and send notification.

Stores an invitation code and sends an invitation to the member via their identifier.

### Example

* OAuth Authentication (oauth2):

```python
import api_idaas_sdk
from api_idaas_sdk.models.get_invite_response import GetInviteResponse
from api_idaas_sdk.models.invite_request_body import InviteRequestBody
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
    api_instance = api_idaas_sdk.IdentifiersApi(api_client)
    invite_request_body = api_idaas_sdk.InviteRequestBody() # InviteRequestBody |  (optional)

    try:
        # Store an invitation code and send notification.
        api_response = api_instance.post_store_and_send_identifier_invite(invite_request_body=invite_request_body)
        print("The response of IdentifiersApi->post_store_and_send_identifier_invite:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IdentifiersApi->post_store_and_send_identifier_invite: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invite_request_body** | [**InviteRequestBody**](InviteRequestBody.md)|  | [optional] 

### Return type

[**GetInviteResponse**](GetInviteResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successfully stored invitation and sent notification. |  -  |
**400** | Bad Request |  -  |
**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


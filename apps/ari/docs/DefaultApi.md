# swagger_client.DefaultApi

All URIs are relative to *http://localhost:8088/ari*

Method | HTTP request | Description
------------- | ------------- | -------------
[**amqp_app_name_post**](DefaultApi.md#amqp_app_name_post) | **POST** /amqp/{appName} | Register a stasis application


# **amqp_app_name_post**
> amqp_app_name_post(app_name, x_asterisk_id=x_asterisk_id)

Register a stasis application

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.DefaultApi()
app_name = 'app_name_example' # str | Application name
x_asterisk_id = 'x_asterisk_id_example' # str | Asterisk ID used to route the request through the API Gateway (optional)

try:
    # Register a stasis application
    api_instance.amqp_app_name_post(app_name, x_asterisk_id=x_asterisk_id)
except ApiException as e:
    print("Exception when calling DefaultApi->amqp_app_name_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **app_name** | **str**| Application name | 
 **x_asterisk_id** | **str**| Asterisk ID used to route the request through the API Gateway | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


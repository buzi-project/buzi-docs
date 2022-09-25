# SmsApi

All URIs are relative to *https://petstore3.swagger.io*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**cancelMessage**](SmsApi.md#cancelMessage) | **POST** /v1/sms/messages/{messageId}/cancel | Cancel a message |
| [**createMessage**](SmsApi.md#createMessage) | **POST** /v1/sms/messages | Create Message |
| [**createPricing**](SmsApi.md#createPricing) | **PUT** /v1/sms/networks/{networkId}/pricing | Create network price |
| [**deleteMessage**](SmsApi.md#deleteMessage) | **DELETE** /v1/sms/messages/{messageId} | Deletes a message |
| [**getMessage**](SmsApi.md#getMessage) | **GET** /v1/sms/messages/{messageId} | Get message |
| [**getNetwork**](SmsApi.md#getNetwork) | **GET** /v1/sms/networks/{networkId} | Get network |
| [**getPricing**](SmsApi.md#getPricing) | **GET** /v1/sms/networks/{networkId}/pricing | List network rates |
| [**listMessages**](SmsApi.md#listMessages) | **GET** /v1/sms/messages | List messages |
| [**listNetworks**](SmsApi.md#listNetworks) | **GET** /v1/sms/networks | List networks |
| [**sendMessage**](SmsApi.md#sendMessage) | **POST** /v1/sms/messages/{messageId}/send | Sends a message |


<a name="cancelMessage"></a>
# **cancelMessage**
> Message cancelMessage(messageId)

Cancel a message

    Returns a single pet

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **messageId** | **Long**| ID of pet to return | [default to null] |

### Return type

[**Message**](../Models/Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="createMessage"></a>
# **createMessage**
> Message createMessage(CreateMessageInput)

Create Message

    Update an existing pet by Id

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **CreateMessageInput** | [**CreateMessageInput**](../Models/CreateMessageInput.md)| Update an existent pet in the store | |

### Return type

[**Message**](../Models/Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="createPricing"></a>
# **createPricing**
> Message createPricing(networkId)

Create network price

    Returns a single pet

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **networkId** | **Integer**|  | [default to null] |

### Return type

[**Message**](../Models/Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="deleteMessage"></a>
# **deleteMessage**
> Error deleteMessage(messageId, api\_key)

Deletes a message

    delete a message

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **messageId** | **Long**| Pet id to delete | [default to null] |
| **api\_key** | **String**|  | [optional] [default to null] |

### Return type

[**Error**](../Models/Error.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getMessage"></a>
# **getMessage**
> Message getMessage(messageId)

Get message

    Returns a single pet

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **messageId** | **Long**| ID of pet to return | [default to null] |

### Return type

[**Message**](../Models/Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getNetwork"></a>
# **getNetwork**
> Network getNetwork(networkId, country\_code)

Get network

    Returns a single pet

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **networkId** | **Integer**|  | [default to null] |
| **country\_code** | **Long**| ID of pet to return | [optional] [default to null] |

### Return type

[**Network**](../Models/Network.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getPricing"></a>
# **getPricing**
> List getPricing(networkId)

List network rates

    Returns a single pet

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **networkId** | **Integer**|  | [default to null] |

### Return type

[**List**](../Models/Pricing.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="listMessages"></a>
# **listMessages**
> List listMessages(inbox, status)

List messages

    Update an existing pet by Id

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **inbox** | **String**|  | [optional] [default to null] |
| **status** | **String**|  | [optional] [default to null] |

### Return type

[**List**](../Models/Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="listNetworks"></a>
# **listNetworks**
> List listNetworks(country\_code)

List networks

    Returns a single pet

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **country\_code** | **String**| ID of pet to return | [optional] [default to null] |

### Return type

[**List**](../Models/Network.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="sendMessage"></a>
# **sendMessage**
> Message sendMessage(messageId)

Sends a message

    Returns a single pet

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **messageId** | **Long**| ID of pet to return | [default to null] |

### Return type

[**Message**](../Models/Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


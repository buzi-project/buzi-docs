# Documentation for Swagger Petstore - OpenAPI 3.0

<a name="documentation-for-api-endpoints"></a>
## Documentation for API Endpoints

All URIs are relative to *https://petstore3.swagger.io*

| Class | Method | HTTP request | Description |
|------------ | ------------- | ------------- | -------------|
| *SmsApi* | [**cancelMessage**](Apis/SmsApi.md#cancelmessage) | **POST** /v1/sms/messages/{messageId}/cancel | Cancel a message |
*SmsApi* | [**createMessage**](Apis/SmsApi.md#createmessage) | **POST** /v1/sms/messages | Create Message |
*SmsApi* | [**createPricing**](Apis/SmsApi.md#createpricing) | **PUT** /v1/sms/networks/{networkId}/pricing | Create network price |
*SmsApi* | [**deleteMessage**](Apis/SmsApi.md#deletemessage) | **DELETE** /v1/sms/messages/{messageId} | Deletes a message |
*SmsApi* | [**getMessage**](Apis/SmsApi.md#getmessage) | **GET** /v1/sms/messages/{messageId} | Get message |
*SmsApi* | [**getNetwork**](Apis/SmsApi.md#getnetwork) | **GET** /v1/sms/networks/{networkId} | Get network |
*SmsApi* | [**getPricing**](Apis/SmsApi.md#getpricing) | **GET** /v1/sms/networks/{networkId}/pricing | List network rates |
*SmsApi* | [**listMessages**](Apis/SmsApi.md#listmessages) | **GET** /v1/sms/messages | List messages |
*SmsApi* | [**listNetworks**](Apis/SmsApi.md#listnetworks) | **GET** /v1/sms/networks | List networks |
*SmsApi* | [**sendMessage**](Apis/SmsApi.md#sendmessage) | **POST** /v1/sms/messages/{messageId}/send | Sends a message |


<a name="documentation-for-models"></a>
## Documentation for Models

 - [Cost](./Models/Cost.md)
 - [CreateMessageInput](./Models/CreateMessageInput.md)
 - [Error](./Models/Error.md)
 - [Message](./Models/Message.md)
 - [Network](./Models/Network.md)
 - [Pricing](./Models/Pricing.md)


<a name="documentation-for-authorization"></a>
## Documentation for Authorization

<a name="ApiKeyAuth"></a>
### ApiKeyAuth

- **Type**: API key
- **API key parameter name**: X-API-Key
- **Location**: HTTP header

<a name="BasicAuth"></a>
### BasicAuth

- **Type**: HTTP basic authentication

<a name="BearerAuth"></a>
### BearerAuth

- **Type**: HTTP basic authentication


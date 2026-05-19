# BuiltByBitApi.ResourcesEmbedApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getV2ResourcesEmbedDownload**](ResourcesEmbedApi.md#getV2ResourcesEmbedDownload) | **GET** /v2/resources/embed/download | Fetch the status of a download request
[**getV2ResourcesEmbedLatest**](ResourcesEmbedApi.md#getV2ResourcesEmbedLatest) | **GET** /v2/resources/embed/latest | Fetches the latest versions &amp; license information
[**postV2ResourcesEmbedDownload**](ResourcesEmbedApi.md#postV2ResourcesEmbedDownload) | **POST** /v2/resources/embed/download | Submit a new download request



## getV2ResourcesEmbedDownload

> GetV2ResourcesEmbedDownload200Response getV2ResourcesEmbedDownload(token)

Fetch the status of a download request

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesEmbedApi();
let token = "token_example"; // String | The token provided when submitting a download request.
apiInstance.getV2ResourcesEmbedDownload(token, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| The token provided when submitting a download request. | 

### Return type

[**GetV2ResourcesEmbedDownload200Response**](GetV2ResourcesEmbedDownload200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesEmbedLatest

> GetV2ResourcesEmbedLatest200Response getV2ResourcesEmbedLatest(opts)

Fetches the latest versions &amp; license information

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesEmbedApi();
let opts = {
  'nonce': "nonce_example" // String | 32 character hash provided by an anti-piracy placeholder of the NONCE type. Must be from a resource download (cannot be an addon download’s nonce, etc).
};
apiInstance.getV2ResourcesEmbedLatest(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **nonce** | **String**| 32 character hash provided by an anti-piracy placeholder of the NONCE type. Must be from a resource download (cannot be an addon download’s nonce, etc). | [optional] 

### Return type

[**GetV2ResourcesEmbedLatest200Response**](GetV2ResourcesEmbedLatest200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## postV2ResourcesEmbedDownload

> PostV2ResourcesEmbedDownload200Response postV2ResourcesEmbedDownload(opts)

Submit a new download request

Supported content types:  - &#39;resource_version&#39;  - &#39;api_asset&#39;

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesEmbedApi();
let opts = {
  'postV2ResourcesEmbedDownloadRequest': new BuiltByBitApi.PostV2ResourcesEmbedDownloadRequest() // PostV2ResourcesEmbedDownloadRequest | 
};
apiInstance.postV2ResourcesEmbedDownload(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **postV2ResourcesEmbedDownloadRequest** | [**PostV2ResourcesEmbedDownloadRequest**](PostV2ResourcesEmbedDownloadRequest.md)|  | [optional] 

### Return type

[**PostV2ResourcesEmbedDownload200Response**](PostV2ResourcesEmbedDownload200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


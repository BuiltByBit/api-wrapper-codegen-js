# BuiltByBitApi.ResourcesEmbedApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getV2ResourcesEmbedDownloadInitiate**](ResourcesEmbedApi.md#getV2ResourcesEmbedDownloadInitiate) | **GET** /v2/resources/embed/download/initiate | Initiate a download request
[**getV2ResourcesEmbedDownloadStatus**](ResourcesEmbedApi.md#getV2ResourcesEmbedDownloadStatus) | **GET** /v2/resources/embed/download/status | Fetch the status of a download request
[**getV2ResourcesEmbedLatest**](ResourcesEmbedApi.md#getV2ResourcesEmbedLatest) | **GET** /v2/resources/embed/latest | Fetches the latest versions &amp; license information



## getV2ResourcesEmbedDownloadInitiate

> GetV2ResourcesEmbedDownloadInitiate200Response getV2ResourcesEmbedDownloadInitiate(contentType, contentId, nonce)

Initiate a download request

See: https://builtbybit.com/help/developers/resource-apis/embed/

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
let contentType = "contentType_example"; // String | Either 'resource', 'resource_version', 'api_asset'
let contentId = 56; // Number | 
let nonce = "nonce_example"; // String | 32 character hash provided by an anti-piracy placeholder of the NONCE type. Must be from a resource download (cannot be an addon download’s nonce, etc).
apiInstance.getV2ResourcesEmbedDownloadInitiate(contentType, contentId, nonce, (error, data, response) => {
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
 **contentType** | **String**| Either &#39;resource&#39;, &#39;resource_version&#39;, &#39;api_asset&#39; | 
 **contentId** | **Number**|  | 
 **nonce** | **String**| 32 character hash provided by an anti-piracy placeholder of the NONCE type. Must be from a resource download (cannot be an addon download’s nonce, etc). | 

### Return type

[**GetV2ResourcesEmbedDownloadInitiate200Response**](GetV2ResourcesEmbedDownloadInitiate200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesEmbedDownloadStatus

> GetV2ResourcesEmbedDownloadStatus200Response getV2ResourcesEmbedDownloadStatus(opts)

Fetch the status of a download request

See: https://builtbybit.com/help/developers/resource-apis/embed/

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
  'token': "token_example" // String | The download request token returned from an initiate request.
};
apiInstance.getV2ResourcesEmbedDownloadStatus(opts, (error, data, response) => {
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
 **token** | **String**| The download request token returned from an initiate request. | [optional] 

### Return type

[**GetV2ResourcesEmbedDownloadStatus200Response**](GetV2ResourcesEmbedDownloadStatus200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesEmbedLatest

> GetV2ResourcesEmbedLatest200Response getV2ResourcesEmbedLatest(opts)

Fetches the latest versions &amp; license information

See: https://builtbybit.com/help/developers/resource-apis/embed/

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


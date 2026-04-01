# BuiltByBitApi.ResourcesBuyerApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getV2ResourcesBuyerLatest**](ResourcesBuyerApi.md#getV2ResourcesBuyerLatest) | **GET** /v2/resources/buyer/latest | Fetches the latest versions &amp; license information



## getV2ResourcesBuyerLatest

> GetV2ResourcesBuyerLatest200Response getV2ResourcesBuyerLatest(opts)

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

let apiInstance = new BuiltByBitApi.ResourcesBuyerApi();
let opts = {
  'nonce': "nonce_example" // String | 32 character hash provided by an anti-piracy placeholder of the NONCE type. Must be from a resource download (cannot be an addon download’s nonce, etc).
};
apiInstance.getV2ResourcesBuyerLatest(opts, (error, data, response) => {
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

[**GetV2ResourcesBuyerLatest200Response**](GetV2ResourcesBuyerLatest200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


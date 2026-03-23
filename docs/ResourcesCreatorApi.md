# BuiltByBitApi.ResourcesCreatorApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**postV2ResourcesCreatorUpdate**](ResourcesCreatorApi.md#postV2ResourcesCreatorUpdate) | **POST** /v2/resources/creator/update | Post a resource update



## postV2ResourcesCreatorUpdate

> PostV2ResourcesCreatorUpdate200Response postV2ResourcesCreatorUpdate(opts)

Post a resource update

Creates a new version for the resource and optionally posts a public update message. The uploaded file must be encoded using base64 as part of the JSON request body shown below.    The request body (including the base64 encoded file data) cannot exceed 100MB. This roughly equates to a 67MB upload limit for the raw file when taking into account base64 encoding losses.

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
let opts = {
  'postV2ResourcesCreatorUpdateRequest': new BuiltByBitApi.PostV2ResourcesCreatorUpdateRequest() // PostV2ResourcesCreatorUpdateRequest | 
};
apiInstance.postV2ResourcesCreatorUpdate(opts, (error, data, response) => {
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
 **postV2ResourcesCreatorUpdateRequest** | [**PostV2ResourcesCreatorUpdateRequest**](PostV2ResourcesCreatorUpdateRequest.md)|  | [optional] 

### Return type

[**PostV2ResourcesCreatorUpdate200Response**](PostV2ResourcesCreatorUpdate200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


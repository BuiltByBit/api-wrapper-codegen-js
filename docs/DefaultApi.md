# BuiltByBitApi.DefaultApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getV2Health**](DefaultApi.md#getV2Health) | **GET** /v2/health | Retrieve a health status
[**getV2ResourcesCreatorCoupons**](DefaultApi.md#getV2ResourcesCreatorCoupons) | **GET** /v2/resources/creator/coupons | Fetch a list of your coupons
[**getV2ResourcesCreatorStores**](DefaultApi.md#getV2ResourcesCreatorStores) | **GET** /v2/resources/creator/stores | Fetch a list of your stores



## getV2Health

> GetV2Health200Response getV2Health()

Retrieve a health status

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.DefaultApi();
apiInstance.getV2Health((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**GetV2Health200Response**](GetV2Health200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesCreatorCoupons

> GetV2ResourcesCreatorCoupons200Response getV2ResourcesCreatorCoupons()

Fetch a list of your coupons

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.DefaultApi();
apiInstance.getV2ResourcesCreatorCoupons((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**GetV2ResourcesCreatorCoupons200Response**](GetV2ResourcesCreatorCoupons200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesCreatorStores

> GetV2ResourcesCreatorStores200Response getV2ResourcesCreatorStores()

Fetch a list of your stores

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.DefaultApi();
apiInstance.getV2ResourcesCreatorStores((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**GetV2ResourcesCreatorStores200Response**](GetV2ResourcesCreatorStores200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


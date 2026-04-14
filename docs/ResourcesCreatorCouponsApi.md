# BuiltByBitApi.ResourcesCreatorCouponsApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getV2ResourcesCreatorCoupons**](ResourcesCreatorCouponsApi.md#getV2ResourcesCreatorCoupons) | **GET** /v2/resources/creator/coupons | Fetch a list of your coupons
[**getV2ResourcesCreatorCouponsEntries**](ResourcesCreatorCouponsApi.md#getV2ResourcesCreatorCouponsEntries) | **GET** /v2/resources/creator/coupons/entries | Fetch a list of your coupon entries
[**postV2ResourcesCreatorCoupons**](ResourcesCreatorCouponsApi.md#postV2ResourcesCreatorCoupons) | **POST** /v2/resources/creator/coupons | Create a new coupon



## getV2ResourcesCreatorCoupons

> GetV2ResourcesCreatorCoupons200Response getV2ResourcesCreatorCoupons(opts)

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

let apiInstance = new BuiltByBitApi.ResourcesCreatorCouponsApi();
let opts = {
  'couponIds': null // Array | A comma-separated list of coupon IDs to filter on. No filter is applied if empty.
};
apiInstance.getV2ResourcesCreatorCoupons(opts, (error, data, response) => {
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
 **couponIds** | [**Array**](.md)| A comma-separated list of coupon IDs to filter on. No filter is applied if empty. | [optional] 

### Return type

[**GetV2ResourcesCreatorCoupons200Response**](GetV2ResourcesCreatorCoupons200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesCreatorCouponsEntries

> GetV2ResourcesCreatorCouponsEntries200Response getV2ResourcesCreatorCouponsEntries(opts)

Fetch a list of your coupon entries

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorCouponsApi();
let opts = {
  'couponIds': null // Array | A comma-separated list of coupon IDs to filter on. No filter is applied if empty.
};
apiInstance.getV2ResourcesCreatorCouponsEntries(opts, (error, data, response) => {
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
 **couponIds** | [**Array**](.md)| A comma-separated list of coupon IDs to filter on. No filter is applied if empty. | [optional] 

### Return type

[**GetV2ResourcesCreatorCouponsEntries200Response**](GetV2ResourcesCreatorCouponsEntries200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## postV2ResourcesCreatorCoupons

> PostV2ResourcesCreatorCoupons200Response postV2ResourcesCreatorCoupons(opts)

Create a new coupon

This endpoint is currently limited to percent-based coupons with a maximum discount of 50%.

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorCouponsApi();
let opts = {
  'postV2ResourcesCreatorCouponsRequest': new BuiltByBitApi.PostV2ResourcesCreatorCouponsRequest() // PostV2ResourcesCreatorCouponsRequest | 
};
apiInstance.postV2ResourcesCreatorCoupons(opts, (error, data, response) => {
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
 **postV2ResourcesCreatorCouponsRequest** | [**PostV2ResourcesCreatorCouponsRequest**](PostV2ResourcesCreatorCouponsRequest.md)|  | [optional] 

### Return type

[**PostV2ResourcesCreatorCoupons200Response**](PostV2ResourcesCreatorCoupons200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


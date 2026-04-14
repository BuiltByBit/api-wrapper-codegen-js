# BuiltByBitApi.ResourcesCreatorBundlesApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getV2ResourcesCreatorBundles**](ResourcesCreatorBundlesApi.md#getV2ResourcesCreatorBundles) | **GET** /v2/resources/creator/bundles | Fetch a list of your bundles
[**getV2ResourcesCreatorBundlesEntries**](ResourcesCreatorBundlesApi.md#getV2ResourcesCreatorBundlesEntries) | **GET** /v2/resources/creator/bundles/entries | Fetch a list of your bundle entries



## getV2ResourcesCreatorBundles

> GetV2ResourcesCreatorBundles200Response getV2ResourcesCreatorBundles(opts)

Fetch a list of your bundles

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorBundlesApi();
let opts = {
  'bundleIds': null // Array | A comma-separated list of bundle IDs to filter on. No filter is applied if empty.
};
apiInstance.getV2ResourcesCreatorBundles(opts, (error, data, response) => {
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
 **bundleIds** | [**Array**](.md)| A comma-separated list of bundle IDs to filter on. No filter is applied if empty. | [optional] 

### Return type

[**GetV2ResourcesCreatorBundles200Response**](GetV2ResourcesCreatorBundles200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesCreatorBundlesEntries

> GetV2ResourcesCreatorBundlesEntries200Response getV2ResourcesCreatorBundlesEntries(opts)

Fetch a list of your bundle entries

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorBundlesApi();
let opts = {
  'bundleIds': null // Array | A comma-separated list of bundle IDs to filter on. No filter is applied if empty.
};
apiInstance.getV2ResourcesCreatorBundlesEntries(opts, (error, data, response) => {
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
 **bundleIds** | [**Array**](.md)| A comma-separated list of bundle IDs to filter on. No filter is applied if empty. | [optional] 

### Return type

[**GetV2ResourcesCreatorBundlesEntries200Response**](GetV2ResourcesCreatorBundlesEntries200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


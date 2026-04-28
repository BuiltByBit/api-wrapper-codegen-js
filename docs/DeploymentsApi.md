# BuiltByBitApi.DeploymentsApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**postV2DeploymentsUpgrade**](DeploymentsApi.md#postV2DeploymentsUpgrade) | **POST** /v2/deployments/upgrade | Upgrade a short-lived token



## postV2DeploymentsUpgrade

> PostV2DeploymentsUpgrade200Response postV2DeploymentsUpgrade(opts)

Upgrade a short-lived token



### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.DeploymentsApi();
let opts = {
  'postV2DeploymentsUpgradeRequest': new BuiltByBitApi.PostV2DeploymentsUpgradeRequest() // PostV2DeploymentsUpgradeRequest | 
};
apiInstance.postV2DeploymentsUpgrade(opts, (error, data, response) => {
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
 **postV2DeploymentsUpgradeRequest** | [**PostV2DeploymentsUpgradeRequest**](PostV2DeploymentsUpgradeRequest.md)|  | [optional] 

### Return type

[**PostV2DeploymentsUpgrade200Response**](PostV2DeploymentsUpgrade200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


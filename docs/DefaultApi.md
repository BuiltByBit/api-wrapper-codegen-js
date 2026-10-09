# BuiltByBitApi.DefaultApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getV2MembersSelf**](DefaultApi.md#getV2MembersSelf) | **GET** /v2/members/self | Fetch self member information



## getV2MembersSelf

> GetV2MembersSelf200Response getV2MembersSelf()

Fetch self member information

See: https://builtbybit.com/help/developers/global-apis/members/

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure OAuth2 access token for authorization: oauth2
let oauth2 = defaultClient.authentications['oauth2'];
oauth2.accessToken = 'YOUR ACCESS TOKEN';
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.DefaultApi();
apiInstance.getV2MembersSelf((error, data, response) => {
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

[**GetV2MembersSelf200Response**](GetV2MembersSelf200Response.md)

### Authorization

[oauth2](../README.md#oauth2), [token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


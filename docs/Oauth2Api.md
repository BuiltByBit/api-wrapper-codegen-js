# BuiltByBitApi.Oauth2Api

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getOauth2Token**](Oauth2Api.md#getOauth2Token) | **POST** /oauth2/token | Request an access token using an existing grant
[**getOauth2TokenRevoke**](Oauth2Api.md#getOauth2TokenRevoke) | **POST** /oauth2/token/revoke | Revoke an existing access or refresh token



## getOauth2Token

> GetOauth2Token200Response getOauth2Token(grantType, opts)

Request an access token using an existing grant

Supported grant types: &#x60;authorization_code&#x60;, and &#x60;refresh_token&#x60;.  Must authenticate via HTTP Basic Authentication, using your OAuth2 client credentials.

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.Oauth2Api();
let grantType = "grantType_example"; // String | 
let opts = {
  'code': "code_example", // String | Required if grant_type = `authorization_code`.
  'refreshToken': "refreshToken_example" // String | Required if grant_type = `refresh_token`.
};
apiInstance.getOauth2Token(grantType, opts, (error, data, response) => {
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
 **grantType** | **String**|  | 
 **code** | **String**| Required if grant_type &#x3D; &#x60;authorization_code&#x60;. | [optional] 
 **refreshToken** | **String**| Required if grant_type &#x3D; &#x60;refresh_token&#x60;. | [optional] 

### Return type

[**GetOauth2Token200Response**](GetOauth2Token200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json


## getOauth2TokenRevoke

> GetOauth2TokenRevoke200Response getOauth2TokenRevoke(authorization, token, opts)

Revoke an existing access or refresh token

Must authenticate via HTTP Basic Authentication, using your OAuth2 client credentials.

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.Oauth2Api();
let authorization = "authorization_example"; // String | OAuth2 client credentials in the Basic authorization format.
let token = "token_example"; // String | 
let opts = {
  'tokenHint': "tokenHint_example" // String | 
};
apiInstance.getOauth2TokenRevoke(authorization, token, opts, (error, data, response) => {
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
 **authorization** | **String**| OAuth2 client credentials in the Basic authorization format. | 
 **token** | **String**|  | 
 **tokenHint** | **String**|  | [optional] 

### Return type

[**GetOauth2TokenRevoke200Response**](GetOauth2TokenRevoke200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json


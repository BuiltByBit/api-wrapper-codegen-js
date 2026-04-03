# BuiltByBitApi.EventsApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getV2Events**](EventsApi.md#getV2Events) | **GET** /v2/events | Fetch a list of pending events
[**postV2EventsComplete**](EventsApi.md#postV2EventsComplete) | **POST** /v2/events/complete | Mark events as complete



## getV2Events

> GetV2Events200Response getV2Events()

Fetch a list of pending events

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.EventsApi();
apiInstance.getV2Events((error, data, response) => {
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

[**GetV2Events200Response**](GetV2Events200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## postV2EventsComplete

> PostV2EventsComplete200Response postV2EventsComplete(opts)

Mark events as complete

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';

let apiInstance = new BuiltByBitApi.EventsApi();
let opts = {
  'postV2EventsCompleteRequest': new BuiltByBitApi.PostV2EventsCompleteRequest() // PostV2EventsCompleteRequest | 
};
apiInstance.postV2EventsComplete(opts, (error, data, response) => {
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
 **postV2EventsCompleteRequest** | [**PostV2EventsCompleteRequest**](PostV2EventsCompleteRequest.md)|  | [optional] 

### Return type

[**PostV2EventsComplete200Response**](PostV2EventsComplete200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


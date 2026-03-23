# BuiltByBitApi.GlobalApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getV2Analytics**](GlobalApi.md#getV2Analytics) | **GET** /v2/analytics | Fetch a list of analytics definitions
[**getV2AnalyticsGraph**](GlobalApi.md#getV2AnalyticsGraph) | **GET** /v2/analytics/graph | Fetch analytics graph data
[**getV2AnalyticsSingle**](GlobalApi.md#getV2AnalyticsSingle) | **GET** /v2/analytics/single | Fetch a single analytics value
[**getV2Events**](GlobalApi.md#getV2Events) | **GET** /v2/events | Fetch a list of pending events
[**postV2EventsComplete**](GlobalApi.md#postV2EventsComplete) | **POST** /v2/events/complete | Mark events as complete



## getV2Analytics

> GetV2Analytics200Response getV2Analytics()

Fetch a list of analytics definitions

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.GlobalApi();
apiInstance.getV2Analytics((error, data, response) => {
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

[**GetV2Analytics200Response**](GetV2Analytics200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2AnalyticsGraph

> GetV2AnalyticsGraph200Response getV2AnalyticsGraph(opts)

Fetch analytics graph data

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.GlobalApi();
let opts = {
  'analytics': null, // Array | A list of analytic IDs to fetch data for.
  'period': "period_example", // String | The time period to fetch data over.
  'filters': null, // Array | A set of filters which may be used for the analytics.
  'startDate': "startDate_example", // String | Only respected when 'period' = 'custom_range', in the format 'YYYY-MM-DD'.
  'endDate': "endDate_example" // String | Only respected when 'period' = 'custom_range', in the format 'YYYY-MM-DD'.
};
apiInstance.getV2AnalyticsGraph(opts, (error, data, response) => {
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
 **analytics** | [**Array**](.md)| A list of analytic IDs to fetch data for. | [optional] 
 **period** | **String**| The time period to fetch data over. | [optional] 
 **filters** | [**Array**](.md)| A set of filters which may be used for the analytics. | [optional] 
 **startDate** | **String**| Only respected when &#39;period&#39; &#x3D; &#39;custom_range&#39;, in the format &#39;YYYY-MM-DD&#39;. | [optional] 
 **endDate** | **String**| Only respected when &#39;period&#39; &#x3D; &#39;custom_range&#39;, in the format &#39;YYYY-MM-DD&#39;. | [optional] 

### Return type

[**GetV2AnalyticsGraph200Response**](GetV2AnalyticsGraph200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2AnalyticsSingle

> GetV2AnalyticsSingle200Response getV2AnalyticsSingle(opts)

Fetch a single analytics value

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.GlobalApi();
let opts = {
  'analytics': null, // Array | A list of analytic IDs to fetch data for.
  'period': "period_example", // String | The time period to fetch data over.
  'filters': null, // Array | A set of filters which may be used for the analytics.
  'startDate': "startDate_example", // String | Only respected when 'period' = 'custom_range', in the format 'YYYY-MM-DD'.
  'endDate': "endDate_example" // String | Only respected when 'period' = 'custom_range', in the format 'YYYY-MM-DD'.
};
apiInstance.getV2AnalyticsSingle(opts, (error, data, response) => {
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
 **analytics** | [**Array**](.md)| A list of analytic IDs to fetch data for. | [optional] 
 **period** | **String**| The time period to fetch data over. | [optional] 
 **filters** | [**Array**](.md)| A set of filters which may be used for the analytics. | [optional] 
 **startDate** | **String**| Only respected when &#39;period&#39; &#x3D; &#39;custom_range&#39;, in the format &#39;YYYY-MM-DD&#39;. | [optional] 
 **endDate** | **String**| Only respected when &#39;period&#39; &#x3D; &#39;custom_range&#39;, in the format &#39;YYYY-MM-DD&#39;. | [optional] 

### Return type

[**GetV2AnalyticsSingle200Response**](GetV2AnalyticsSingle200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


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

let apiInstance = new BuiltByBitApi.GlobalApi();
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

let apiInstance = new BuiltByBitApi.GlobalApi();
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


# BuiltByBitApi.AnalyticsApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getV2Analytics**](AnalyticsApi.md#getV2Analytics) | **GET** /v2/analytics | Fetch a list of analytics definitions
[**getV2AnalyticsGraph**](AnalyticsApi.md#getV2AnalyticsGraph) | **GET** /v2/analytics/graph | Fetch analytics graph data
[**getV2AnalyticsSingle**](AnalyticsApi.md#getV2AnalyticsSingle) | **GET** /v2/analytics/single | Fetch a single analytics value



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

let apiInstance = new BuiltByBitApi.AnalyticsApi();
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

let apiInstance = new BuiltByBitApi.AnalyticsApi();
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

let apiInstance = new BuiltByBitApi.AnalyticsApi();
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


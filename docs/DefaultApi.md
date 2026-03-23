# BuiltByBitApi.DefaultApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getV2Analytics**](DefaultApi.md#getV2Analytics) | **GET** /v2/analytics | Fetch a list of analytics definitions
[**getV2AnalyticsGraph**](DefaultApi.md#getV2AnalyticsGraph) | **GET** /v2/analytics/graph | Fetch analytics graph data
[**getV2Events**](DefaultApi.md#getV2Events) | **GET** /v2/events | Fetch a list of pending events
[**postV2EventsComplete**](DefaultApi.md#postV2EventsComplete) | **POST** /v2/events/complete | Mark events as complete
[**postV2ResourcesCreatorUpdate**](DefaultApi.md#postV2ResourcesCreatorUpdate) | **POST** /v2/resources/creator/update | Post a resource update



## getV2Analytics

> GetV2Analytics200Response getV2Analytics()

Fetch a list of analytics definitions

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';

let apiInstance = new BuiltByBitApi.DefaultApi();
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

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2AnalyticsGraph

> GetV2AnalyticsGraph200Response getV2AnalyticsGraph(opts)

Fetch analytics graph data

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';

let apiInstance = new BuiltByBitApi.DefaultApi();
let opts = {
  'analytics': null, // Array | 
  'period': "period_example", // String | 
  'grouping': "grouping_example", // String | 
  'filters': "filters_example", // String | 
  'startDate': "startDate_example", // String | Only respected when 'period' = 'custom_range'.
  'endDate': "endDate_example" // String | Only respected when 'period' = 'custom_range'.
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
 **analytics** | [**Array**](.md)|  | [optional] 
 **period** | **String**|  | [optional] 
 **grouping** | **String**|  | [optional] 
 **filters** | **String**|  | [optional] 
 **startDate** | **String**| Only respected when &#39;period&#39; &#x3D; &#39;custom_range&#39;. | [optional] 
 **endDate** | **String**| Only respected when &#39;period&#39; &#x3D; &#39;custom_range&#39;. | [optional] 

### Return type

[**GetV2AnalyticsGraph200Response**](GetV2AnalyticsGraph200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2Events

> GetV2Events200Response getV2Events()

Fetch a list of pending events

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';

let apiInstance = new BuiltByBitApi.DefaultApi();
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

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## postV2EventsComplete

> PostV2EventsComplete200Response postV2EventsComplete(opts)

Mark events as complete

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';

let apiInstance = new BuiltByBitApi.DefaultApi();
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


## postV2ResourcesCreatorUpdate

> PostV2ResourcesCreatorUpdate200Response postV2ResourcesCreatorUpdate(opts)

Post a resource update

Creates a new version for the resource and optionally posts a public update message. The uploaded file must be encoded using base64 as part of the JSON request body shown below.    The request body (including the base64 encoded file data) cannot exceed 100MB. This roughly equates to a 67MB upload limit for the raw file when taking into account base64 encoding losses.

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';

let apiInstance = new BuiltByBitApi.DefaultApi();
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

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


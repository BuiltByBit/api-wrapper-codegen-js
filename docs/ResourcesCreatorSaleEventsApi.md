# BuiltByBitApi.ResourcesCreatorSaleEventsApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getV2ResourcesCreatorSaleEvents**](ResourcesCreatorSaleEventsApi.md#getV2ResourcesCreatorSaleEvents) | **GET** /v2/resources/creator/sale-events | Fetch a list of your sale events
[**getV2ResourcesCreatorSaleEventsEntries**](ResourcesCreatorSaleEventsApi.md#getV2ResourcesCreatorSaleEventsEntries) | **GET** /v2/resources/creator/sale-events/entries | Fetch a list of your sale event entries



## getV2ResourcesCreatorSaleEvents

> GetV2ResourcesCreatorSaleEvents200Response getV2ResourcesCreatorSaleEvents(opts)

Fetch a list of your sale events

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorSaleEventsApi();
let opts = {
  'saleEventIds': null // Array | A comma-separated list of sale event IDs to filter on. No filter is applied if empty.
};
apiInstance.getV2ResourcesCreatorSaleEvents(opts, (error, data, response) => {
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
 **saleEventIds** | [**Array**](.md)| A comma-separated list of sale event IDs to filter on. No filter is applied if empty. | [optional] 

### Return type

[**GetV2ResourcesCreatorSaleEvents200Response**](GetV2ResourcesCreatorSaleEvents200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesCreatorSaleEventsEntries

> GetV2ResourcesCreatorSaleEventsEntries200Response getV2ResourcesCreatorSaleEventsEntries(opts)

Fetch a list of your sale event entries

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorSaleEventsApi();
let opts = {
  'saleEventIds': null // Array | A comma-separated list of sale event IDs to filter on. No filter is applied if empty.
};
apiInstance.getV2ResourcesCreatorSaleEventsEntries(opts, (error, data, response) => {
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
 **saleEventIds** | [**Array**](.md)| A comma-separated list of sale event IDs to filter on. No filter is applied if empty. | [optional] 

### Return type

[**GetV2ResourcesCreatorSaleEventsEntries200Response**](GetV2ResourcesCreatorSaleEventsEntries200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


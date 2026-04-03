# BuiltByBitApi.DefaultApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getV2ResourcesCreatorBatch**](DefaultApi.md#getV2ResourcesCreatorBatch) | **GET** /v2/resources/creator/batch | Fetch a list of your batches edits
[**postV2ResourcesCreatorBatch**](DefaultApi.md#postV2ResourcesCreatorBatch) | **POST** /v2/resources/creator/batch | Submit a new batch edit



## getV2ResourcesCreatorBatch

> GetV2ResourcesCreatorBatch200Response getV2ResourcesCreatorBatch(opts)

Fetch a list of your batches edits

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.DefaultApi();
let opts = {
  'batchIds': null // Array | A comma-separated list of batch IDs to filter on. No filter is applied if empty.
};
apiInstance.getV2ResourcesCreatorBatch(opts, (error, data, response) => {
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
 **batchIds** | [**Array**](.md)| A comma-separated list of batch IDs to filter on. No filter is applied if empty. | [optional] 

### Return type

[**GetV2ResourcesCreatorBatch200Response**](GetV2ResourcesCreatorBatch200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## postV2ResourcesCreatorBatch

> PostV2ResourcesCreatorBatch200Response postV2ResourcesCreatorBatch(opts)

Submit a new batch edit

Batch edits will be processed in the background meaning a successful call to this endpoint does not guarantee that the edits have been completed. You will instead receive an identifier to a batch edit which you can then use to fetch the status of via the below endpoint. This is not an atomic operation meaning some resources may be edited successfully and others may not be due to an error. You may only batch edit resources you own currently.

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';

let apiInstance = new BuiltByBitApi.DefaultApi();
let opts = {
  'postV2ResourcesCreatorBatchRequest': new BuiltByBitApi.PostV2ResourcesCreatorBatchRequest() // PostV2ResourcesCreatorBatchRequest | 
};
apiInstance.postV2ResourcesCreatorBatch(opts, (error, data, response) => {
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
 **postV2ResourcesCreatorBatchRequest** | [**PostV2ResourcesCreatorBatchRequest**](PostV2ResourcesCreatorBatchRequest.md)|  | [optional] 

### Return type

[**PostV2ResourcesCreatorBatch200Response**](PostV2ResourcesCreatorBatch200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


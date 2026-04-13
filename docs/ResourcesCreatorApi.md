# BuiltByBitApi.ResourcesCreatorApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getV2ResourcesCreatorAddons**](ResourcesCreatorApi.md#getV2ResourcesCreatorAddons) | **GET** /v2/resources/creator/addons | Fetch a list of your resources&#39; addons
[**getV2ResourcesCreatorBatch**](ResourcesCreatorApi.md#getV2ResourcesCreatorBatch) | **GET** /v2/resources/creator/batch | Fetch a list of your batches edits
[**getV2ResourcesCreatorBundles**](ResourcesCreatorApi.md#getV2ResourcesCreatorBundles) | **GET** /v2/resources/creator/bundles | Fetch a list of your bundles
[**getV2ResourcesCreatorBundlesEntries**](ResourcesCreatorApi.md#getV2ResourcesCreatorBundlesEntries) | **GET** /v2/resources/creator/bundles/entries | Fetch a list of your bundle entries
[**getV2ResourcesCreatorCoupons**](ResourcesCreatorApi.md#getV2ResourcesCreatorCoupons) | **GET** /v2/resources/creator/coupons | Fetch a list of your coupons
[**getV2ResourcesCreatorCouponsEntries**](ResourcesCreatorApi.md#getV2ResourcesCreatorCouponsEntries) | **GET** /v2/resources/creator/coupons/entries | Fetch a list of your coupon entries
[**getV2ResourcesCreatorLicenses**](ResourcesCreatorApi.md#getV2ResourcesCreatorLicenses) | **GET** /v2/resources/creator/licenses | Fetch a list of your resources&#39; licenses
[**getV2ResourcesCreatorPurchases**](ResourcesCreatorApi.md#getV2ResourcesCreatorPurchases) | **GET** /v2/resources/creator/purchases | Fetch a list of your resources&#39; purchases
[**getV2ResourcesCreatorResources**](ResourcesCreatorApi.md#getV2ResourcesCreatorResources) | **GET** /v2/resources/creator/resources | Fetch a list of your resources
[**getV2ResourcesCreatorReviews**](ResourcesCreatorApi.md#getV2ResourcesCreatorReviews) | **GET** /v2/resources/creator/reviews | Fetch a list of your resources&#39; reviews
[**getV2ResourcesCreatorSaleEvents**](ResourcesCreatorApi.md#getV2ResourcesCreatorSaleEvents) | **GET** /v2/resources/creator/sale-events | Fetch a list of your sale events
[**getV2ResourcesCreatorSaleEventsEntries**](ResourcesCreatorApi.md#getV2ResourcesCreatorSaleEventsEntries) | **GET** /v2/resources/creator/sale-events/entries | Fetch a list of your sale event entries
[**getV2ResourcesCreatorStores**](ResourcesCreatorApi.md#getV2ResourcesCreatorStores) | **GET** /v2/resources/creator/stores | Fetch a list of your stores
[**getV2ResourcesCreatorUpdates**](ResourcesCreatorApi.md#getV2ResourcesCreatorUpdates) | **GET** /v2/resources/creator/updates | Fetch a list of your resource&#39;s updates
[**getV2ResourcesCreatorVersions**](ResourcesCreatorApi.md#getV2ResourcesCreatorVersions) | **GET** /v2/resources/creator/versions | Fetch a list of your resources&#39; versions
[**postV2ResourcesCreatorBatch**](ResourcesCreatorApi.md#postV2ResourcesCreatorBatch) | **POST** /v2/resources/creator/batch | Submit a new batch edit
[**postV2ResourcesCreatorCoupons**](ResourcesCreatorApi.md#postV2ResourcesCreatorCoupons) | **POST** /v2/resources/creator/coupons | Create a new coupon
[**postV2ResourcesCreatorUpdate**](ResourcesCreatorApi.md#postV2ResourcesCreatorUpdate) | **POST** /v2/resources/creator/update | Post a resource update



## getV2ResourcesCreatorAddons

> GetV2ResourcesCreatorAddons200Response getV2ResourcesCreatorAddons(opts)

Fetch a list of your resources&#39; addons

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
let opts = {
  'resourceIds': null // Array | A comma-separated list of resource IDs to filter on. No filter is applied if empty.
};
apiInstance.getV2ResourcesCreatorAddons(opts, (error, data, response) => {
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
 **resourceIds** | [**Array**](.md)| A comma-separated list of resource IDs to filter on. No filter is applied if empty. | [optional] 

### Return type

[**GetV2ResourcesCreatorAddons200Response**](GetV2ResourcesCreatorAddons200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


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

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
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

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
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

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
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


## getV2ResourcesCreatorCoupons

> GetV2ResourcesCreatorCoupons200Response getV2ResourcesCreatorCoupons(opts)

Fetch a list of your coupons

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
let opts = {
  'couponIds': null // Array | A comma-separated list of coupon IDs to filter on. No filter is applied if empty.
};
apiInstance.getV2ResourcesCreatorCoupons(opts, (error, data, response) => {
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
 **couponIds** | [**Array**](.md)| A comma-separated list of coupon IDs to filter on. No filter is applied if empty. | [optional] 

### Return type

[**GetV2ResourcesCreatorCoupons200Response**](GetV2ResourcesCreatorCoupons200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesCreatorCouponsEntries

> GetV2ResourcesCreatorCouponsEntries200Response getV2ResourcesCreatorCouponsEntries(opts)

Fetch a list of your coupon entries

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
let opts = {
  'couponIds': null // Array | A comma-separated list of coupon IDs to filter on. No filter is applied if empty.
};
apiInstance.getV2ResourcesCreatorCouponsEntries(opts, (error, data, response) => {
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
 **couponIds** | [**Array**](.md)| A comma-separated list of coupon IDs to filter on. No filter is applied if empty. | [optional] 

### Return type

[**GetV2ResourcesCreatorCouponsEntries200Response**](GetV2ResourcesCreatorCouponsEntries200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesCreatorLicenses

> GetV2ResourcesCreatorLicenses200Response getV2ResourcesCreatorLicenses(opts)

Fetch a list of your resources&#39; licenses

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
let opts = {
  'resourceIds': null // Array | A comma-separated list of resource IDs to filter on. No filter is applied if empty.
};
apiInstance.getV2ResourcesCreatorLicenses(opts, (error, data, response) => {
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
 **resourceIds** | [**Array**](.md)| A comma-separated list of resource IDs to filter on. No filter is applied if empty. | [optional] 

### Return type

[**GetV2ResourcesCreatorLicenses200Response**](GetV2ResourcesCreatorLicenses200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesCreatorPurchases

> GetV2ResourcesCreatorPurchases200Response getV2ResourcesCreatorPurchases(opts)

Fetch a list of your resources&#39; purchases

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
let opts = {
  'resourceIds': null, // Array | A comma-separated list of resource IDs to filter on. No filter is applied if empty.
  'buyerIds': null, // Array | A comma-separated list of buyer IDs to filter on. No filter is applied if empty
  'externalTids': null // Array | A comma-separated list of external transaction IDs (TIDs) to filter on. No filter is applied if empty.
};
apiInstance.getV2ResourcesCreatorPurchases(opts, (error, data, response) => {
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
 **resourceIds** | [**Array**](.md)| A comma-separated list of resource IDs to filter on. No filter is applied if empty. | [optional] 
 **buyerIds** | [**Array**](.md)| A comma-separated list of buyer IDs to filter on. No filter is applied if empty | [optional] 
 **externalTids** | [**Array**](.md)| A comma-separated list of external transaction IDs (TIDs) to filter on. No filter is applied if empty. | [optional] 

### Return type

[**GetV2ResourcesCreatorPurchases200Response**](GetV2ResourcesCreatorPurchases200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesCreatorResources

> GetV2ResourcesCreatorResources200Response getV2ResourcesCreatorResources(opts)

Fetch a list of your resources

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
let opts = {
  'resourceIds': null // Array | A comma-separated list of resource IDs to filter on. No filter is applied if empty.
};
apiInstance.getV2ResourcesCreatorResources(opts, (error, data, response) => {
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
 **resourceIds** | [**Array**](.md)| A comma-separated list of resource IDs to filter on. No filter is applied if empty. | [optional] 

### Return type

[**GetV2ResourcesCreatorResources200Response**](GetV2ResourcesCreatorResources200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesCreatorReviews

> GetV2ResourcesCreatorReviews200Response getV2ResourcesCreatorReviews(opts)

Fetch a list of your resources&#39; reviews

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
let opts = {
  'resourceIds': null // Array | A comma-separated list of resource IDs to filter on. No filter is applied if empty.
};
apiInstance.getV2ResourcesCreatorReviews(opts, (error, data, response) => {
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
 **resourceIds** | [**Array**](.md)| A comma-separated list of resource IDs to filter on. No filter is applied if empty. | [optional] 

### Return type

[**GetV2ResourcesCreatorReviews200Response**](GetV2ResourcesCreatorReviews200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


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

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
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

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
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


## getV2ResourcesCreatorStores

> GetV2ResourcesCreatorStores200Response getV2ResourcesCreatorStores()

Fetch a list of your stores

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
apiInstance.getV2ResourcesCreatorStores((error, data, response) => {
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

[**GetV2ResourcesCreatorStores200Response**](GetV2ResourcesCreatorStores200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesCreatorUpdates

> GetV2ResourcesCreatorUpdates200Response getV2ResourcesCreatorUpdates(opts)

Fetch a list of your resource&#39;s updates

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
let opts = {
  'resourceIds': null // Array | A comma-separated list of resource IDs to filter on. No filter is applied if empty.
};
apiInstance.getV2ResourcesCreatorUpdates(opts, (error, data, response) => {
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
 **resourceIds** | [**Array**](.md)| A comma-separated list of resource IDs to filter on. No filter is applied if empty. | [optional] 

### Return type

[**GetV2ResourcesCreatorUpdates200Response**](GetV2ResourcesCreatorUpdates200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesCreatorVersions

> GetV2ResourcesCreatorVersions200Response getV2ResourcesCreatorVersions(opts)

Fetch a list of your resources&#39; versions

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
let opts = {
  'resourceIds': null // Array | A comma-separated list of resource IDs to filter on. No filter is applied if empty.
};
apiInstance.getV2ResourcesCreatorVersions(opts, (error, data, response) => {
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
 **resourceIds** | [**Array**](.md)| A comma-separated list of resource IDs to filter on. No filter is applied if empty. | [optional] 

### Return type

[**GetV2ResourcesCreatorVersions200Response**](GetV2ResourcesCreatorVersions200Response.md)

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

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
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


## postV2ResourcesCreatorCoupons

> PostV2ResourcesCreatorCoupons200Response postV2ResourcesCreatorCoupons(opts)

Create a new coupon

This endpoint is currently limited to percent-based coupons with a maximum discount of 50%.

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
let opts = {
  'postV2ResourcesCreatorCouponsRequest': new BuiltByBitApi.PostV2ResourcesCreatorCouponsRequest() // PostV2ResourcesCreatorCouponsRequest | 
};
apiInstance.postV2ResourcesCreatorCoupons(opts, (error, data, response) => {
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
 **postV2ResourcesCreatorCouponsRequest** | [**PostV2ResourcesCreatorCouponsRequest**](PostV2ResourcesCreatorCouponsRequest.md)|  | [optional] 

### Return type

[**PostV2ResourcesCreatorCoupons200Response**](PostV2ResourcesCreatorCoupons200Response.md)

### Authorization

[token](../README.md#token)

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
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesCreatorApi();
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

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


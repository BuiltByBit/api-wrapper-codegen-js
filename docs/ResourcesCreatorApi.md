# BuiltByBitApi.ResourcesCreatorApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getV2ResourcesCreatorAddons**](ResourcesCreatorApi.md#getV2ResourcesCreatorAddons) | **GET** /v2/resources/creator/addons | Fetch a list of your resources&#39; addons
[**getV2ResourcesCreatorBundles**](ResourcesCreatorApi.md#getV2ResourcesCreatorBundles) | **GET** /v2/resources/creator/bundles | Fetch a list of your bundles
[**getV2ResourcesCreatorLicenses**](ResourcesCreatorApi.md#getV2ResourcesCreatorLicenses) | **GET** /v2/resources/creator/licenses | Fetch a list of your resources&#39; licenses
[**getV2ResourcesCreatorPurchases**](ResourcesCreatorApi.md#getV2ResourcesCreatorPurchases) | **GET** /v2/resources/creator/purchases | Fetch a list of your resources&#39; purchases
[**getV2ResourcesCreatorResources**](ResourcesCreatorApi.md#getV2ResourcesCreatorResources) | **GET** /v2/resources/creator/resources | Fetch a list of your resources
[**getV2ResourcesCreatorReviews**](ResourcesCreatorApi.md#getV2ResourcesCreatorReviews) | **GET** /v2/resources/creator/reviews | Fetch a list of your resources&#39; reviews
[**getV2ResourcesCreatorSaleEvents**](ResourcesCreatorApi.md#getV2ResourcesCreatorSaleEvents) | **GET** /v2/resources/creator/sale-events | Fetch a list of your sale events
[**getV2ResourcesCreatorUpdates**](ResourcesCreatorApi.md#getV2ResourcesCreatorUpdates) | **GET** /v2/resources/creator/updates | Fetch a list of your resource&#39;s updates
[**getV2ResourcesCreatorVersions**](ResourcesCreatorApi.md#getV2ResourcesCreatorVersions) | **GET** /v2/resources/creator/versions | Fetch a list of your resources&#39; versions
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


## getV2ResourcesCreatorBundles

> GetV2ResourcesCreatorBundles200Response getV2ResourcesCreatorBundles()

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
apiInstance.getV2ResourcesCreatorBundles((error, data, response) => {
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

[**GetV2ResourcesCreatorBundles200Response**](GetV2ResourcesCreatorBundles200Response.md)

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
  'resourceIds': null // Array | A comma-separated list of resource IDs to filter on. No filter is applied if empty.
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

> GetV2ResourcesCreatorSaleEvents200Response getV2ResourcesCreatorSaleEvents()

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
apiInstance.getV2ResourcesCreatorSaleEvents((error, data, response) => {
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

[**GetV2ResourcesCreatorSaleEvents200Response**](GetV2ResourcesCreatorSaleEvents200Response.md)

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


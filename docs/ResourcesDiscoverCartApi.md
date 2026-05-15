# BuiltByBitApi.ResourcesDiscoverCartApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getV2ResourcesDiscoverCartView**](ResourcesDiscoverCartApi.md#getV2ResourcesDiscoverCartView) | **GET** /v2/resources/discover/cart/view | View the user&#39;s cart items
[**postV2ResourcesDiscoverCartAdd**](ResourcesDiscoverCartApi.md#postV2ResourcesDiscoverCartAdd) | **POST** /v2/resources/discover/cart/add | Add items to a user&#39;s cart
[**postV2ResourcesDiscoverCartCheckout**](ResourcesDiscoverCartApi.md#postV2ResourcesDiscoverCartCheckout) | **POST** /v2/resources/discover/cart/checkout | Initiate a checkout of a user&#39;s cart
[**postV2ResourcesDiscoverCartCouponAdd**](ResourcesDiscoverCartApi.md#postV2ResourcesDiscoverCartCouponAdd) | **POST** /v2/resources/discover/cart/coupon/add | Add a coupon to the user&#39;s cart
[**postV2ResourcesDiscoverCartCouponRemove**](ResourcesDiscoverCartApi.md#postV2ResourcesDiscoverCartCouponRemove) | **POST** /v2/resources/discover/cart/coupon/remove | Remove a coupon from the user&#39;s cart
[**postV2ResourcesDiscoverCartRemove**](ResourcesDiscoverCartApi.md#postV2ResourcesDiscoverCartRemove) | **POST** /v2/resources/discover/cart/remove | Remove an item from the user&#39;s cart



## getV2ResourcesDiscoverCartView

> GetV2ResourcesDiscoverCartView200Response getV2ResourcesDiscoverCartView()

View the user&#39;s cart items



### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure OAuth2 access token for authorization: oauth2
let oauth2 = defaultClient.authentications['oauth2'];
oauth2.accessToken = 'YOUR ACCESS TOKEN';

let apiInstance = new BuiltByBitApi.ResourcesDiscoverCartApi();
apiInstance.getV2ResourcesDiscoverCartView((error, data, response) => {
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

[**GetV2ResourcesDiscoverCartView200Response**](GetV2ResourcesDiscoverCartView200Response.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## postV2ResourcesDiscoverCartAdd

> PostV2ResourcesDiscoverCartAdd2XXResponse postV2ResourcesDiscoverCartAdd(opts)

Add items to a user&#39;s cart

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure OAuth2 access token for authorization: oauth2
let oauth2 = defaultClient.authentications['oauth2'];
oauth2.accessToken = 'YOUR ACCESS TOKEN';

let apiInstance = new BuiltByBitApi.ResourcesDiscoverCartApi();
let opts = {
  'postV2ResourcesDiscoverCartAddRequest': new BuiltByBitApi.PostV2ResourcesDiscoverCartAddRequest() // PostV2ResourcesDiscoverCartAddRequest | A list of content to add to the user's cart. The outer list is keyed by the content type and the inner list are the content IDs.    For instance, if adding a resource with the ID 555, the body becomes:  ```json  {\"add\": {\"resource\": [555]}}  ```
};
apiInstance.postV2ResourcesDiscoverCartAdd(opts, (error, data, response) => {
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
 **postV2ResourcesDiscoverCartAddRequest** | [**PostV2ResourcesDiscoverCartAddRequest**](PostV2ResourcesDiscoverCartAddRequest.md)| A list of content to add to the user&#39;s cart. The outer list is keyed by the content type and the inner list are the content IDs.    For instance, if adding a resource with the ID 555, the body becomes:  &#x60;&#x60;&#x60;json  {\&quot;add\&quot;: {\&quot;resource\&quot;: [555]}}  &#x60;&#x60;&#x60; | [optional] 

### Return type

[**PostV2ResourcesDiscoverCartAdd2XXResponse**](PostV2ResourcesDiscoverCartAdd2XXResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## postV2ResourcesDiscoverCartCheckout

> PostV2ResourcesDiscoverCartCheckout200Response postV2ResourcesDiscoverCartCheckout(opts)

Initiate a checkout of a user&#39;s cart

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure OAuth2 access token for authorization: oauth2
let oauth2 = defaultClient.authentications['oauth2'];
oauth2.accessToken = 'YOUR ACCESS TOKEN';

let apiInstance = new BuiltByBitApi.ResourcesDiscoverCartApi();
let opts = {
  'body': {key: null} // Object | 
};
apiInstance.postV2ResourcesDiscoverCartCheckout(opts, (error, data, response) => {
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
 **body** | **Object**|  | [optional] 

### Return type

[**PostV2ResourcesDiscoverCartCheckout200Response**](PostV2ResourcesDiscoverCartCheckout200Response.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## postV2ResourcesDiscoverCartCouponAdd

> PostV2ResourcesDiscoverCartCouponAdd200Response postV2ResourcesDiscoverCartCouponAdd(opts)

Add a coupon to the user&#39;s cart

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure OAuth2 access token for authorization: oauth2
let oauth2 = defaultClient.authentications['oauth2'];
oauth2.accessToken = 'YOUR ACCESS TOKEN';

let apiInstance = new BuiltByBitApi.ResourcesDiscoverCartApi();
let opts = {
  'postV2ResourcesDiscoverCartCouponAddRequest': new BuiltByBitApi.PostV2ResourcesDiscoverCartCouponAddRequest() // PostV2ResourcesDiscoverCartCouponAddRequest | 
};
apiInstance.postV2ResourcesDiscoverCartCouponAdd(opts, (error, data, response) => {
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
 **postV2ResourcesDiscoverCartCouponAddRequest** | [**PostV2ResourcesDiscoverCartCouponAddRequest**](PostV2ResourcesDiscoverCartCouponAddRequest.md)|  | [optional] 

### Return type

[**PostV2ResourcesDiscoverCartCouponAdd200Response**](PostV2ResourcesDiscoverCartCouponAdd200Response.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## postV2ResourcesDiscoverCartCouponRemove

> PostV2ResourcesDiscoverCartCouponRemove200Response postV2ResourcesDiscoverCartCouponRemove(opts)

Remove a coupon from the user&#39;s cart

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure OAuth2 access token for authorization: oauth2
let oauth2 = defaultClient.authentications['oauth2'];
oauth2.accessToken = 'YOUR ACCESS TOKEN';

let apiInstance = new BuiltByBitApi.ResourcesDiscoverCartApi();
let opts = {
  'postV2ResourcesDiscoverCartCouponRemoveRequest': new BuiltByBitApi.PostV2ResourcesDiscoverCartCouponRemoveRequest() // PostV2ResourcesDiscoverCartCouponRemoveRequest | 
};
apiInstance.postV2ResourcesDiscoverCartCouponRemove(opts, (error, data, response) => {
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
 **postV2ResourcesDiscoverCartCouponRemoveRequest** | [**PostV2ResourcesDiscoverCartCouponRemoveRequest**](PostV2ResourcesDiscoverCartCouponRemoveRequest.md)|  | [optional] 

### Return type

[**PostV2ResourcesDiscoverCartCouponRemove200Response**](PostV2ResourcesDiscoverCartCouponRemove200Response.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## postV2ResourcesDiscoverCartRemove

> PostV2ResourcesDiscoverCartRemove200Response postV2ResourcesDiscoverCartRemove(opts)

Remove an item from the user&#39;s cart

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure OAuth2 access token for authorization: oauth2
let oauth2 = defaultClient.authentications['oauth2'];
oauth2.accessToken = 'YOUR ACCESS TOKEN';

let apiInstance = new BuiltByBitApi.ResourcesDiscoverCartApi();
let opts = {
  'postV2ResourcesDiscoverCartRemoveRequest': new BuiltByBitApi.PostV2ResourcesDiscoverCartRemoveRequest() // PostV2ResourcesDiscoverCartRemoveRequest | 
};
apiInstance.postV2ResourcesDiscoverCartRemove(opts, (error, data, response) => {
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
 **postV2ResourcesDiscoverCartRemoveRequest** | [**PostV2ResourcesDiscoverCartRemoveRequest**](PostV2ResourcesDiscoverCartRemoveRequest.md)|  | [optional] 

### Return type

[**PostV2ResourcesDiscoverCartRemove200Response**](PostV2ResourcesDiscoverCartRemove200Response.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


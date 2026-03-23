# BuiltByBitApi.DiscoveryApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getResourcesDiscoverCategories**](DiscoveryApi.md#getResourcesDiscoverCategories) | **GET** /v2/resources/discover/categories | Fetch a list of categories
[**getResourcesDiscoverResources**](DiscoveryApi.md#getResourcesDiscoverResources) | **GET** /v2/resources/discover/resources | Fetch a list of resources
[**getV2ResourcesDiscoverCartView**](DiscoveryApi.md#getV2ResourcesDiscoverCartView) | **GET** /v2/resources/discover/cart/view | View the user&#39;s cart items
[**getV2ResourcesDiscoverLicenses**](DiscoveryApi.md#getV2ResourcesDiscoverLicenses) | **GET** /v2/resources/discover/licenses | Fetch a list of the user&#39;s licenses
[**postV2ResourcesDiscoverCartAdd**](DiscoveryApi.md#postV2ResourcesDiscoverCartAdd) | **POST** /v2/resources/discover/cart/add | Add items to a user&#39;s cart
[**postV2ResourcesDiscoverCartCheckout**](DiscoveryApi.md#postV2ResourcesDiscoverCartCheckout) | **POST** /v2/resources/discover/cart/checkout | Initiate a checkout of a user&#39;s cart
[**postV2ResourcesDiscoverCartCouponAdd**](DiscoveryApi.md#postV2ResourcesDiscoverCartCouponAdd) | **POST** /v2/resources/discover/cart/coupon/add | Add a coupon to the user&#39;s cart
[**postV2ResourcesDiscoverCartCouponRemove**](DiscoveryApi.md#postV2ResourcesDiscoverCartCouponRemove) | **POST** /v2/resources/discover/cart/coupon/remove | Remove a coupon from the user&#39;s cart
[**postV2ResourcesDiscoverCartRemove**](DiscoveryApi.md#postV2ResourcesDiscoverCartRemove) | **POST** /v2/resources/discover/cart/remove | Remove an item from the user&#39;s cart



## getResourcesDiscoverCategories

> GetResourcesDiscoverCategories200Response getResourcesDiscoverCategories(opts)

Fetch a list of categories

Supported &#39;with&#39; hints:  - Children: includes all subcategories and their children

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';

let apiInstance = new BuiltByBitApi.DiscoveryApi();
let opts = {
  'categoryId': "categoryId_example", // String | A category ID to filter on.
  '_with': "_with_example" // String | A comma-separated list of submodels to include.
};
apiInstance.getResourcesDiscoverCategories(opts, (error, data, response) => {
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
 **categoryId** | **String**| A category ID to filter on. | [optional] 
 **_with** | **String**| A comma-separated list of submodels to include. | [optional] 

### Return type

[**GetResourcesDiscoverCategories200Response**](GetResourcesDiscoverCategories200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getResourcesDiscoverResources

> GetResourcesDiscoverResources200Response getResourcesDiscoverResources(opts)

Fetch a list of resources

Supported &#39;with&#39; hints:  - &#x60;filters&#x60;: include dynamic filter information in the response.  - See &#39;Resource&#39; model for additional &#39;with&#39; hints.

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.DiscoveryApi();
let opts = {
  'categoryId': "categoryId_example", // String | A category ID to filter on. If the provided category is a parent, resources from subcategories will also be included.
  '_with': Description,Creator, // String | A comma-separated list of additional data to include. See endpoint documentation for more information.
  'filters': {key: null}, // Object | A list of dynamic filters to apply.
  'resourceIds': "resourceIds_example", // String | A comma-separated list of resource IDs to filter on.
  'page': 1, // Number | The page number to return.
  'perPage': 25, // Number | The number of resources to return per page.
  'noDependencies': true // Boolean | 
};
apiInstance.getResourcesDiscoverResources(opts, (error, data, response) => {
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
 **categoryId** | **String**| A category ID to filter on. If the provided category is a parent, resources from subcategories will also be included. | [optional] 
 **_with** | **String**| A comma-separated list of additional data to include. See endpoint documentation for more information. | [optional] 
 **filters** | [**Object**](.md)| A list of dynamic filters to apply. | [optional] 
 **resourceIds** | **String**| A comma-separated list of resource IDs to filter on. | [optional] 
 **page** | **Number**| The page number to return. | [optional] [default to 1]
 **perPage** | **Number**| The number of resources to return per page. | [optional] [default to 25]
 **noDependencies** | **Boolean**|  | [optional] 

### Return type

[**GetResourcesDiscoverResources200Response**](GetResourcesDiscoverResources200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesDiscoverCartView

> GetV2ResourcesDiscoverCartView200Response getV2ResourcesDiscoverCartView()

View the user&#39;s cart items

Supported &#39;with hints&#39;:

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';

let apiInstance = new BuiltByBitApi.DiscoveryApi();
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

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesDiscoverLicenses

> GetV2ResourcesDiscoverLicenses200Response getV2ResourcesDiscoverLicenses(opts)

Fetch a list of the user&#39;s licenses

Supported &#39;with&#39; hints:  - Resource: the resource the license is for if content_type &#x3D; &#x60;resource&#x60;

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';

let apiInstance = new BuiltByBitApi.DiscoveryApi();
let opts = {
  'page': 56, // Number | The page number/offset to return items for.
  'perPage': 25, // Number | The number of items per page to return.
  '_with': "_with_example" // String | A comma-separated list of supported 'with hints'. See model & endpoint-level docs for more info.
};
apiInstance.getV2ResourcesDiscoverLicenses(opts, (error, data, response) => {
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
 **page** | **Number**| The page number/offset to return items for. | [optional] 
 **perPage** | **Number**| The number of items per page to return. | [optional] [default to 25]
 **_with** | **String**| A comma-separated list of supported &#39;with hints&#39;. See model &amp; endpoint-level docs for more info. | [optional] 

### Return type

[**GetV2ResourcesDiscoverLicenses200Response**](GetV2ResourcesDiscoverLicenses200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## postV2ResourcesDiscoverCartAdd

> PostV2ResourcesDiscoverCartAdd2XXResponse postV2ResourcesDiscoverCartAdd(opts)

Add items to a user&#39;s cart

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';

let apiInstance = new BuiltByBitApi.DiscoveryApi();
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

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## postV2ResourcesDiscoverCartCheckout

> PostV2ResourcesDiscoverCartCheckout200Response postV2ResourcesDiscoverCartCheckout(opts)

Initiate a checkout of a user&#39;s cart

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';

let apiInstance = new BuiltByBitApi.DiscoveryApi();
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

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## postV2ResourcesDiscoverCartCouponAdd

> PostV2ResourcesDiscoverCartCouponAdd200Response postV2ResourcesDiscoverCartCouponAdd(opts)

Add a coupon to the user&#39;s cart

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';

let apiInstance = new BuiltByBitApi.DiscoveryApi();
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

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## postV2ResourcesDiscoverCartCouponRemove

> PostV2ResourcesDiscoverCartCouponRemove200Response postV2ResourcesDiscoverCartCouponRemove(opts)

Remove a coupon from the user&#39;s cart

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';

let apiInstance = new BuiltByBitApi.DiscoveryApi();
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

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## postV2ResourcesDiscoverCartRemove

> PostV2ResourcesDiscoverCartRemove200Response postV2ResourcesDiscoverCartRemove(opts)

Remove an item from the user&#39;s cart

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';

let apiInstance = new BuiltByBitApi.DiscoveryApi();
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

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


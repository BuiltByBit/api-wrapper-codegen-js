# BuiltByBitApi.ResourcesDiscoverApi

All URIs are relative to *https://api.builtbybit.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getResourcesDiscoverCategories**](ResourcesDiscoverApi.md#getResourcesDiscoverCategories) | **GET** /v2/resources/discover/categories | Fetch a list of categories
[**getResourcesDiscoverResources**](ResourcesDiscoverApi.md#getResourcesDiscoverResources) | **GET** /v2/resources/discover/resources | Fetch a list of resources
[**getV2ResourcesDiscoverDownloadDirectInitiate**](ResourcesDiscoverApi.md#getV2ResourcesDiscoverDownloadDirectInitiate) | **GET** /v2/resources/discover/download/direct/initiate | Initiate a direct download request
[**getV2ResourcesDiscoverDownloadDirectPoll**](ResourcesDiscoverApi.md#getV2ResourcesDiscoverDownloadDirectPoll) | **GET** /v2/resources/discover/download/direct/status | Fetch the status of a direct download request
[**getV2ResourcesDiscoverLicenses**](ResourcesDiscoverApi.md#getV2ResourcesDiscoverLicenses) | **GET** /v2/resources/discover/licenses | Fetch a list of the user&#39;s licenses



## getResourcesDiscoverCategories

> GetResourcesDiscoverCategories200Response getResourcesDiscoverCategories(opts)

Fetch a list of categories

Supported &#39;with&#39; hints:  - Children: includes all subcategories and their children

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure API key authorization: token
let token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

let apiInstance = new BuiltByBitApi.ResourcesDiscoverApi();
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

[token](../README.md#token)

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

let apiInstance = new BuiltByBitApi.ResourcesDiscoverApi();
let opts = {
  'categoryId': "categoryId_example", // String | A category ID to filter on. If the provided category is a parent, resources from subcategories will also be included.
  '_with': Description,Creator, // String | A comma-separated list of additional data to include. See endpoint documentation for more information.
  'filters': {key: null}, // Object | A list of dynamic filters to apply.
  'resourceIds': "resourceIds_example", // String | A comma-separated list of resource IDs to filter on.
  'page': 1, // Number | The page number to return.
  'perPage': 25, // Number | The number of resources to return per page.
  'noDependencies': true, // Boolean | Whether or not to exclude resources with dependencies listed.
  'excludedResourceIds': "excludedResourceIds_example", // String | A comma-separated list of resource IDs to exclude. No filter will be applied if empty.
  'excludedCreatorIds': "excludedCreatorIds_example" // String | A comma-separated list of creator IDs to exclude. No filter will be applied if empty.
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
 **noDependencies** | **Boolean**| Whether or not to exclude resources with dependencies listed. | [optional] 
 **excludedResourceIds** | **String**| A comma-separated list of resource IDs to exclude. No filter will be applied if empty. | [optional] 
 **excludedCreatorIds** | **String**| A comma-separated list of creator IDs to exclude. No filter will be applied if empty. | [optional] 

### Return type

[**GetResourcesDiscoverResources200Response**](GetResourcesDiscoverResources200Response.md)

### Authorization

[token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesDiscoverDownloadDirectInitiate

> GetV2ResourcesDiscoverDownloadDirectInitiate200Response getV2ResourcesDiscoverDownloadDirectInitiate(contentType, contentId)

Initiate a direct download request

See: https://builtbybit.com/help/developers/discovery-api/downloading-and-one-click/

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure OAuth2 access token for authorization: oauth2
let oauth2 = defaultClient.authentications['oauth2'];
oauth2.accessToken = 'YOUR ACCESS TOKEN';

let apiInstance = new BuiltByBitApi.ResourcesDiscoverApi();
let contentType = "contentType_example"; // String | Either 'resource' or 'resource_version'
let contentId = 56; // Number | 
apiInstance.getV2ResourcesDiscoverDownloadDirectInitiate(contentType, contentId, (error, data, response) => {
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
 **contentType** | **String**| Either &#39;resource&#39; or &#39;resource_version&#39; | 
 **contentId** | **Number**|  | 

### Return type

[**GetV2ResourcesDiscoverDownloadDirectInitiate200Response**](GetV2ResourcesDiscoverDownloadDirectInitiate200Response.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getV2ResourcesDiscoverDownloadDirectPoll

> GetV2ResourcesDiscoverDownloadDirectPoll200Response getV2ResourcesDiscoverDownloadDirectPoll(opts)

Fetch the status of a direct download request

See: https://builtbybit.com/help/developers/discovery-api/downloading-and-one-click/

### Example

```javascript
import BuiltByBitApi from 'built_by_bit_api';
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure OAuth2 access token for authorization: oauth2
let oauth2 = defaultClient.authentications['oauth2'];
oauth2.accessToken = 'YOUR ACCESS TOKEN';

let apiInstance = new BuiltByBitApi.ResourcesDiscoverApi();
let opts = {
  'token': "token_example" // String | The download request token returned from an initiate request.
};
apiInstance.getV2ResourcesDiscoverDownloadDirectPoll(opts, (error, data, response) => {
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
 **token** | **String**| The download request token returned from an initiate request. | [optional] 

### Return type

[**GetV2ResourcesDiscoverDownloadDirectPoll200Response**](GetV2ResourcesDiscoverDownloadDirectPoll200Response.md)

### Authorization

[oauth2](../README.md#oauth2)

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
let defaultClient = BuiltByBitApi.ApiClient.instance;
// Configure OAuth2 access token for authorization: oauth2
let oauth2 = defaultClient.authentications['oauth2'];
oauth2.accessToken = 'YOUR ACCESS TOKEN';

let apiInstance = new BuiltByBitApi.ResourcesDiscoverApi();
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

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


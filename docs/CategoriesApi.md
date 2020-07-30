# meli.CategoriesApi

All URIs are relative to *https://api.mercadolibre.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**categoriesCategoryIdGet**](CategoriesApi.md#categoriesCategoryIdGet) | **GET** /categories/{category_id} | Return by category.
[**sitesSiteIdCategoriesGet**](CategoriesApi.md#sitesSiteIdCategoriesGet) | **GET** /sites/{site_id}/categories | Return a categories by site.
[**sitesSiteIdDomainDiscoverySearchGet**](CategoriesApi.md#sitesSiteIdDomainDiscoverySearchGet) | **GET** /sites/{site_id}/domain_discovery/search | Predictor



## categoriesCategoryIdGet

> categoriesCategoryIdGet(categoryId)

Return by category.

### Example

```javascript
import meli from 'mercadolibre-nodejs-sdk';

let apiInstance = new meli.CategoriesApi();
let categoryId = "categoryId_example"; // String | 
apiInstance.categoriesCategoryIdGet(categoryId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **categoryId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## sitesSiteIdCategoriesGet

> sitesSiteIdCategoriesGet(siteId)

Return a categories by site.

### Example

```javascript
import meli from 'mercadolibre-nodejs-sdk';

let apiInstance = new meli.CategoriesApi();
let siteId = "siteId_example"; // String | 
apiInstance.sitesSiteIdCategoriesGet(siteId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **siteId** | **String**|  | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## sitesSiteIdDomainDiscoverySearchGet

> sitesSiteIdDomainDiscoverySearchGet(siteId, q, limit)

Predictor

### Example

```javascript
import meli from 'mercadolibre-nodejs-sdk';

let apiInstance = new meli.CategoriesApi();
let siteId = "siteId_example"; // String | 
let q = "q_example"; // String | 
let limit = "limit_example"; // String | 
apiInstance.sitesSiteIdDomainDiscoverySearchGet(siteId, q, limit, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **siteId** | **String**|  | 
 **q** | **String**|  | 
 **limit** | **String**|  | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


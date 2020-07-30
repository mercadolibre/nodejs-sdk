# meli.ItemsHealthApi

All URIs are relative to *https://api.mercadolibre.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**itemsIdHealthActionsGet**](ItemsHealthApi.md#itemsIdHealthActionsGet) | **GET** /items/{id}/health/actions | Return item health actions by id.
[**itemsIdHealthGet**](ItemsHealthApi.md#itemsIdHealthGet) | **GET** /items/{id}/health | Return health by id.
[**sitesSiteIdHealthLevelsGet**](ItemsHealthApi.md#sitesSiteIdHealthLevelsGet) | **GET** /sites/{site_id}/health_levels | Return health levels.



## itemsIdHealthActionsGet

> itemsIdHealthActionsGet(id, accessToken)

Return item health actions by id.

### Example

```javascript
import meli from 'mercadolibre-nodejs-sdk';

let apiInstance = new meli.ItemsHealthApi();
let id = "id_example"; // String | 
let accessToken = "accessToken_example"; // String | 
apiInstance.itemsIdHealthActionsGet(id, accessToken, (error, data, response) => {
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
 **id** | **String**|  | 
 **accessToken** | **String**|  | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## itemsIdHealthGet

> itemsIdHealthGet(id, accessToken)

Return health by id.

### Example

```javascript
import meli from 'mercadolibre-nodejs-sdk';

let apiInstance = new meli.ItemsHealthApi();
let id = "id_example"; // String | 
let accessToken = "accessToken_example"; // String | 
apiInstance.itemsIdHealthGet(id, accessToken, (error, data, response) => {
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
 **id** | **String**|  | 
 **accessToken** | **String**|  | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## sitesSiteIdHealthLevelsGet

> sitesSiteIdHealthLevelsGet(siteId)

Return health levels.

### Example

```javascript
import meli from 'mercadolibre-nodejs-sdk';

let apiInstance = new meli.ItemsHealthApi();
let siteId = "siteId_example"; // String | 
apiInstance.sitesSiteIdHealthLevelsGet(siteId, (error, data, response) => {
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


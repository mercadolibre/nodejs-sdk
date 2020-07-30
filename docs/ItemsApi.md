# meli.ItemsApi

All URIs are relative to *https://api.mercadolibre.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**itemsIdGet**](ItemsApi.md#itemsIdGet) | **GET** /items/{id} | Return a Item.
[**itemsIdPut**](ItemsApi.md#itemsIdPut) | **PUT** /items/{id} | Update a Item.
[**itemsPost**](ItemsApi.md#itemsPost) | **POST** /items | Create a Item.



## itemsIdGet

> itemsIdGet(id)

Return a Item.

### Example

```javascript
import meli from 'mercadolibre-nodejs-sdk';

let apiInstance = new meli.ItemsApi();
let id = "id_example"; // String | 
apiInstance.itemsIdGet(id, (error, data, response) => {
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

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## itemsIdPut

> itemsIdPut(id, accessToken, item)

Update a Item.

### Example

```javascript
import meli from 'mercadolibre-nodejs-sdk';

let apiInstance = new meli.ItemsApi();
let id = "id_example"; // String | 
let accessToken = "accessToken_example"; // String | 
let item = new meli.Item(); // Item | 
apiInstance.itemsIdPut(id, accessToken, item, (error, data, response) => {
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
 **item** | [**Item**](Item.md)|  | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## itemsPost

> itemsPost(accessToken, item)

Create a Item.

### Example

```javascript
import meli from 'mercadolibre-nodejs-sdk';

let apiInstance = new meli.ItemsApi();
let accessToken = "accessToken_example"; // String | 
let item = new meli.Item(); // Item | 
apiInstance.itemsPost(accessToken, item, (error, data, response) => {
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
 **accessToken** | **String**|  | 
 **item** | [**Item**](Item.md)|  | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


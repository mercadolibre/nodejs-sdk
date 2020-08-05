# meli.RestClientApi

All URIs are relative to *https://api.mercadolibre.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**resourceDelete**](RestClientApi.md#resourceDelete) | **DELETE** /{resource} | Resource path DELETE
[**resourceGet**](RestClientApi.md#resourceGet) | **GET** /{resource} | Resource path GET
[**resourcePost**](RestClientApi.md#resourcePost) | **POST** /{resource} | Resourse path POST
[**resourcePut**](RestClientApi.md#resourcePut) | **PUT** /{resource} | Resourse path PUT



## resourceDelete

> resourceDelete(resource, accessToken)

Resource path DELETE

### Example

```javascript
import meli from 'mercadolibre-nodejs-sdk';

let apiInstance = new meli.RestClientApi();
let resource = "resource_example"; // String | 
let accessToken = "accessToken_example"; // String | 
apiInstance.resourceDelete(resource, accessToken, (error, data, response) => {
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
 **resource** | **String**|  | 
 **accessToken** | **String**|  | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## resourceGet

> resourceGet(resource, accessToken)

Resource path GET

### Example

```javascript
import meli from 'mercadolibre-nodejs-sdk';

let apiInstance = new meli.RestClientApi();
let resource = "resource_example"; // String | 
let accessToken = "accessToken_example"; // String | 
apiInstance.resourceGet(resource, accessToken, (error, data, response) => {
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
 **resource** | **String**|  | 
 **accessToken** | **String**|  | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## resourcePost

> resourcePost(resource, accessToken, body)

Resourse path POST

### Example

```javascript
import meli from 'mercadolibre-nodejs-sdk';

let apiInstance = new meli.RestClientApi();
let resource = "resource_example"; // String | 
let accessToken = "accessToken_example"; // String | 
let body = null; // Object | 
apiInstance.resourcePost(resource, accessToken, body, (error, data, response) => {
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
 **resource** | **String**|  | 
 **accessToken** | **String**|  | 
 **body** | **Object**|  | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## resourcePut

> resourcePut(resource, accessToken, body)

Resourse path PUT

### Example

```javascript
import meli from 'mercadolibre-nodejs-sdk';

let apiInstance = new meli.RestClientApi();
let resource = "resource_example"; // String | 
let accessToken = "accessToken_example"; // String | 
let body = null; // Object | 
apiInstance.resourcePut(resource, accessToken, body, (error, data, response) => {
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
 **resource** | **String**|  | 
 **accessToken** | **String**|  | 
 **body** | **Object**|  | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


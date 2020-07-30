# meli.OAuth20Api

All URIs are relative to *https://api.mercadolibre.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**auth**](OAuth20Api.md#auth) | **GET** /authorization | Authentication Endpoint
[**getToken**](OAuth20Api.md#getToken) | **POST** /oauth/token | Request Access Token



## auth

> auth(responseType, clientId, redirectUri)

Authentication Endpoint

### Example

```javascript
import meli from 'mercadolibre-nodejs-sdk';

let apiInstance = new meli.OAuth20Api();
let responseType = "'code'"; // String | 
let clientId = "clientId_example"; // String | 
let redirectUri = "redirectUri_example"; // String | 
apiInstance.auth(responseType, clientId, redirectUri, (error, data, response) => {
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
 **responseType** | **String**|  | [default to &#39;code&#39;]
 **clientId** | **String**|  | 
 **redirectUri** | **String**|  | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getToken

> getToken(opts)

Request Access Token

Partner makes a request to the token endpoint by adding the following parameters described below

### Example

```javascript
import meli from 'mercadolibre-nodejs-sdk';

let apiInstance = new meli.OAuth20Api();
let opts = {
  'grantType': "grantType_example", // String | 
  'clientId': "clientId_example", // String | 
  'clientSecret': "clientSecret_example", // String | 
  'redirectUri': "redirectUri_example", // String | 
  'code': "code_example", // String | 
  'refreshToken': "refreshToken_example" // String | 
};
apiInstance.getToken(opts, (error, data, response) => {
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
 **grantType** | **String**|  | [optional] 
 **clientId** | **String**|  | [optional] 
 **clientSecret** | **String**|  | [optional] 
 **redirectUri** | **String**|  | [optional] 
 **code** | **String**|  | [optional] 
 **refreshToken** | **String**|  | [optional] 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: Not defined


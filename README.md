
<h1 align="center">
  <a href="https://developers.mercadolibre.com">
    <img src="https://user-images.githubusercontent.com/1153516/29861072-689ec57e-8d3e-11e7-8368-dd923543258f.jpg" alt="Mercado Libre Developers" width="230"></a>
  </a>
  <br><br>
  MercadoLibre's Node.JS SDK
  <br>
</h1>

<h4 align="center">This is the official Node.JS SDK for MercadoLibre's Platform.</h4>


## Installation

```shell

npm install mercadolibre-nodejs-sdk --save

```

## Usage

```javascript
var meli = require('mercadolibre-nodejs-sdk');

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

## Or you can use the RestClient
```javascript
var meli = require('mercadolibre-nodejs-sdk');

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

## Examples for OAuth - get code
```javascript
var meli = require('mercadolibre-nodejs-sdk');
let apiInstance = new meli.OAuth20Api();

// Get the Auth URL, for example, country Argentina -> 1
const authUrl = apiInstance.apiClient.getBasePathFromSettings(1);
// Auth URLs Options by country
// [0]  - https://api.mercadolibre.com (default API endpoint)
// [1]  - https://auth.mercadolibre.com.ar
// [2]  - https://auth.mercadolivre.com.br
// [3]  - https://auth.mercadolibre.com.co
// [4]  - https://auth.mercadolibre.com.mx
// [5]  - https://auth.mercadolibre.com.uy
// [6]  - https://auth.mercadolibre.cl
// [7]  - https://auth.mercadolibre.com.cr
// [8]  - https://auth.mercadolibre.com.ec
// [9]  - https://auth.mercadolibre.com.ve
// [10] - https://auth.mercadolibre.com.pa
// [11] - https://auth.mercadolibre.com.pe
// [12] - https://auth.mercadolibre.com.pt
// [13] - https://auth.mercadolibre.com.do

// Use the correct auth URL
apiInstance.apiClient.basePath = authUrl;

let responseType = "code"; // String | 
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

## Examples for OAuth - get token
```javascript
var meli = require('mercadolibre-nodejs-sdk');

let apiInstance = new meli.OAuth20Api();
let opts = {
  'grantType': "authorization_code", // String | 
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

## Example using the RestClient with a POST Item
```javascript
var meli = require('mercadolibre-nodejs-sdk');

var meli = require('mercadolibre-nodejs-sdk');
const InlineObject = {
  "title": "Item de test - No Ofertar",
  "category_id": "MLA5991",
  "price": "350",
  "currency_id": "ARS",
  "available_quantity": "12",
  "buying_mode": "buy_it_now",
  "listing_type_id": "bronze",
  "condition": "new",
  "description": "Item de Teste. Mercado Livre SDK",
  "video_id": "RXWn6kftTHY",
  "pictures": [
    {
      "source": "https://upload.wikimedia.org/wikipedia/commons/f/fd/Ray_Ban_Original_Wayfarer.jpg"
    }
  ]
};

let apiInstance = new meli.RestClientApi();
let resource = "items"; // Example "items" | 
let accessToken = "accessToken_example"; // String | 
let body = InlineObject; // Object | 
apiInstance.resourcePost(resource, accessToken, body, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
});
```

## Documentation & Important notes

##### The URIs are relative to https://api.mercadolibre.com

##### The Authorization URL: https://auth.mercadolibre.com.ar/authorization

#####  All docs for the library are located [here](https://github.com/mercadolibre/nodejs-sdk/tree/master/docs)

#####  Check out our examples codes in the folder [examples](https://github.com/mercadolibre/nodejs-sdk/tree/master/examples)

##### Don’t forget to check out our [developer site](https://developers.mercadolibre.com/)
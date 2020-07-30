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
let resource = "resource_example"; // Example "items" | 
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

## Documentation for API Endpoints

The URIs are relative to *https://api.mercadolibre.com*

  

## Documentation for Authorization  

-  **Type**: OAuth

-  **Flow**: accessCode

-  **Authorization URL**: https://auth.mercadolibre.com.ar/authorization

-  **Scopes**:

- read: Grants read access

- write: Grants write access

- offline_access: Grants read and write access, and adds the possibility to get a refresh token and stay authenticated as the user.


## Examples

Don't forget to check out our examples codes in the folder [examples](https://github.com/mercadolibre/nodejs-sdk/tree/master/examples)

## Community

You can contact us if you have questions using the standard communication channels described in the [developer's site](https://developers.mercadolibre.com/)

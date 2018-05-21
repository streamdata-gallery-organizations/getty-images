{
  "info": {
    "name": "Getty Images Get Products",
    "_postman_id": "b68fe732-37ef-46b1-88e7-2f2c7387e192",
    "description": "This endpoint returns all products available to the username used during authentication. As such, this endpoint requires the use of\r\na fully authorized access_token. The product data can then be used as search filters, restricting results to images from a specific product.\r\n\r\nYou'll need an API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage for more information on how to sign up for an API key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "915d1e74-bbe4-41f0-aa8a-0c852fe1bf1e",
          "name": "Products_GetProducts",
          "request": {
            "url": "http://api.gettyimages.com/v3/products?fields=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept-Language",
                "value": "{}",
                "description": "Provide a header to specify the language of result values",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Provide access token in the format of 'Bearer {token}'",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint returns all products available to the username used during authentication"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21122cf7-a9a1-4b0f-a2f7-890429c19a83"
            }
          ]
        }
      ]
    }
  ]
}
{
  "info": {
    "name": "Getty Images Get Purchased Images",
    "_postman_id": "8c98652e-7aa4-42f8-94a1-287fde72aacc",
    "description": "This endpoint returns a list of all assets purchased on gettyimages.com by the username used for authentication. \r\nUse of this endpoint requires configuration changes to your API key. \r\nPlease contact [developersupport@gettyimages.com](mailto:developersupport@gettyimages.com) to learn more.\r\n\r\nYou'll need an API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage for more information on how to sign up for an API key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "ac39060a-25b2-423e-b69a-bd913783a6d4",
          "name": "Purchases_GetPreviousAssetPurchases",
          "request": {
            "url": "http://api.gettyimages.com/v3/purchased-assets?end_date=%7B%7D&page=%7B%7D&page_size=%7B%7D&start_date=%7B%7D",
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
            "description": "This endpoint returns a list of all assets purchased on gettyimages"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a883f563-a601-4df6-8ea8-293f4cc33810"
            }
          ]
        }
      ]
    }
  ]
}
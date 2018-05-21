{
  "info": {
    "name": "Getty Images Get Previously Purchased Images",
    "_postman_id": "559a1003-4572-4340-9673-d1c9cb6b6d80",
    "description": "This endpoint returns a list of all images purchased on gettyimages.com by the username used for authentication.\r\nUse of this endpoint requires configuration changes to your API key. Please contact [developersupport@gettyimages.com](mailto:developersupport@gettyimages.com)\r\nto learn more.\r\n\r\nYou'll need an API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage for more information on how to sign up for an API key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "dcb937ef-a283-401e-9dee-1aedf065ecb1",
          "name": "Purchases_GetPreviousPurchases",
          "request": {
            "url": "http://api.gettyimages.com/v3/purchased-images?end_date=%7B%7D&page=%7B%7D&page_size=%7B%7D&start_date=%7B%7D",
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
            "description": "This endpoint returns a list of all images purchased on gettyimages"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88349bb3-0d44-4dc2-a48a-da36f35f59ed"
            }
          ]
        }
      ]
    }
  ]
}
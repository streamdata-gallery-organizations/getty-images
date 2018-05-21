{
  "info": {
    "name": "Getty Images Get Collections",
    "_postman_id": "98b11dca-d078-435e-990c-31abad286d49",
    "description": "Use this endpoint to retrieve collections associated with your Getty Images account. To browse available collections see our [Image collections page]( http://www.gettyimages.com/creative-images/collections).\r\n\r\nYou'll need an API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html) page for more information on how to sign up for an API key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "b2f7d3b2-54ff-4ba4-86d2-e9ba26ca592b",
          "name": "Collections_GetCollections",
          "request": {
            "url": "http://api.gettyimages.com/v3/collections",
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
            "description": "Use this endpoint to retrieve collections associated with your Getty Images account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4e794e3-a77f-4fd0-99a3-f5f253e5bb8b"
            }
          ]
        }
      ]
    }
  ]
}
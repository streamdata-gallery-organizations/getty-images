{
  "info": {
    "name": "Getty Images Get Countries",
    "_postman_id": "adec4625-9a00-415f-b13f-558fb449ae98",
    "description": "Returns a list of country objects that contains country name, two letter ISO abbreviation and three letter ISO abbreviation.\r\n\r\nYou'll need an API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html) page for more information on how to sign up for an API key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "d5e03657-77f8-4bc0-8563-f5134fc9de51",
          "name": "Countries_GetCountries",
          "request": {
            "url": "http://api.gettyimages.com/v3/countries",
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
            "description": "Returns a list of country objects that contains country name, two letter ISO abbreviation and three letter ISO abbreviation"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8dd27f5b-bcaa-4c20-abc8-ffb3fc031de1"
            }
          ]
        }
      ]
    }
  ]
}
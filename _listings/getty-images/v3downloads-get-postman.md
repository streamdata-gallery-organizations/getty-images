{
  "info": {
    "name": "Getty Images Get Downloads",
    "_postman_id": "560fcf77-1f80-4283-b7b4-24bc9cac1321",
    "description": "Returns information about a customer's previously downloaded assets.\r\n\r\nYou'll need an API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html) page for more information on how to sign up for an API key. \r\n \r\n\t\r\nThis endpoint requires being a Getty Images customer to limit your results to only assets that you have a license to use, \r\nyou need to also include an authorization token in the header of your request. \r\nPlease consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html) for more information on authorization tokens.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "f2116dff-255c-449f-9b93-f9e17fed62a3",
          "name": "Downloads_GetDownloads",
          "request": {
            "url": "http://api.gettyimages.com/v3/downloads?company_downloads=%7B%7D&end_date=%7B%7D&page=%7B%7D&page_size=%7B%7D&product_type=%7B%7D&start_date=%7B%7D",
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
            "description": "Returns information about a customer's previously downloaded assets"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "619d6534-b9cc-472e-a9c9-86d90eb3a276"
            }
          ]
        }
      ]
    }
  ]
}
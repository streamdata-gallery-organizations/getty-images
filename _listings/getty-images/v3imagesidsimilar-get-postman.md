{
  "info": {
    "name": "Getty Images Search Similar Images",
    "_postman_id": "8aed0734-5cb5-4ec8-94e9-78a7a664d43c",
    "description": "This endpoint will search our asset database for images similar to the specified asset id. Due to a wide variety of available \r\nimage resolutions, the images are grouped into a handful of size categories for simplicity. \r\n\r\nYou'll need an API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html) \r\npage for more information on how to sign up for an API key. \r\n\r\n## Working with Fields Sets\r\n\r\nFields sets are used in the **fields** request parameter to receive a suite of metadata fields. The following fields sets are available:\r\n\r\n#### Summary Fields Set\r\n\r\nThe **summary_set** query string parameter fields value represents a small batch of metadata fields that are often used to build\r\nsearch response results. The following fields are provided for every image in your result set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n    [\r\n        \"asset_family\",\r\n        \"caption\",\r\n        \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n        \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n        ]\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields value represents a large batch of metadata fields that are often used to build a \r\ndetailed view of images. The following fields are provided for every image in your result set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n    [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n        \"asset_family\",\r\n        \"call_for_image\",\r\n        \"caption\",\r\n        \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n        \"copyright\",\r\n        \"date_created\",\r\n        \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n        ],\r\n        \"editorial_segments\",\r\n        \"event_ids\",\r\n        \"graphical_style\",\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n        \"orientation\",\r\n        \"product_types\",\r\n        \"quality_rank\",\r\n        \"referral_destinations\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Display Fields Set\r\n\r\nThe **display_set** query string parameter fields value represents the fields that provide you with URLs for the low resolution files \r\nthat are most frequently used to build a UI displaying search results. The following fields are provided for every image in your result\r\nset when you include **display_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n    [\r\n        \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n        ]\r\n    ]\r\n}\r\n```",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "b6f6c1f7-380e-419a-b22a-fca2d2323773",
          "name": "Images_GetSimilarImages",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.gettyimages.com",
              "path": [
                "v3/images/:id/similar"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page_size",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "This endpoint will search our asset database for images similar to the specified asset id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e92758e-d32c-4168-a28b-0f53ed55f588"
            }
          ]
        }
      ]
    }
  ]
}
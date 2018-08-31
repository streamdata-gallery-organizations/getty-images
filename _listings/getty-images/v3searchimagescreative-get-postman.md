{
  "info": {
    "name": "Getty Images Search for creative images only",
    "_postman_id": "e7c0cee7-44dc-4a72-bd8d-276c3875b952",
    "description": "Use this endpoint to search our contemporary stock photos, illustrations and archival images.\r\n\r\nYou'll need an API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html) \r\npage for more information on how to sign up for an API key. \r\n \r\nYou can show different information in the response by specifying values on the \"fields\" parameter (see details below).\r\nYou can search with only an API key, and that will give you search results that are equivalent to doing a search on the GettyImages.com site without being logged in (anonymous search).  If you are a Getty Images API customer and would like to ensure that your API searches return only assets that you have a license to use, you need to also include an authorization token in the header of your request.  Please consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html) for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md) for code examples of getting a token.\r\n\r\n## Working with Fields Sets\r\n\r\nFields sets are used in the **fields** request parameter to receive a suite of metadata fields. The following fields sets are available:\r\n\r\n#### Summary Fields Set\r\n\r\nThe **summary_set** query string parameter fields value represents a small batch of metadata fields that are often used to \r\nbuild search response results. The following fields are provided for every image in your result set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\": \r\n    [\r\n        \"asset_family\",\r\n        \"caption\",\r\n        \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n        \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n        ],\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields value represents a large batch of metadata fields that are often used to \r\nbuild a detailed view of images. The following fields are provided for every image in your result set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\": \r\n    [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n        \"asset_family\",\r\n        \"call_for_image\",\r\n        \"caption\",\r\n        \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n        \"copyright\",\r\n        \"date_created\",\r\n        \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n        ],\r\n        \"editorial_segments\",\r\n        \"event_ids\",\r\n        \"graphical_style\",\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n        \"orientation\",\r\n        \"product_types\",\r\n        \"quality_rank\",\r\n        \"referral_destinations\",\r\n        \"title\"\r\n    ]\r\n]\r\n```\r\n\r\n#### Display Fields Set\r\n\r\nThe **display_set** query string parameter fields value represents the fields that provide you with URLs for the low resolution\r\nfiles that are most frequently used to build a UI displaying search results. The following fields are provided for every image \r\nin your result set when you include **display_set** in your request.\r\n\r\n```Go\r\n{\r\n    \"images\": \r\n    [\r\n        \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n        ]\r\n    ]\r\n}\r\n```",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "f02cb96a-1a83-4029-a6bd-550ea2f1f7d6",
          "name": "Search_GetCreativeImagesByPhrase",
          "request": {
            "url": "http://api.gettyimages.com/v3/search/images/creative?age_of_people=%7B%7D&artists=%7B%7D&collections_filter_type=%7B%7D&collection_codes=%7B%7D&color=%7B%7D&compositions=%7B%7D&embed_content_only=%7B%7D&ethnicity=%7B%7D&exclude_nudity=%7B%7D&fields=%7B%7D&file_types=%7B%7D&graphical_styles=%7B%7D&keyword_ids=%7B%7D&license_models=%7B%7D&minimum_size=%7B%7D&number_of_people=%7B%7D&orientations=%7B%7D&page=%7B%7D&page_size=%7B%7D&phrase=%7B%7D&prestige_content_only=%7B%7D&product_types=%7B%7D&sort_order=%7B%7D",
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
            "description": "Use this endpoint to search our contemporary stock photos, illustrations and archival images"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "449bce53-a29f-4ba0-9059-91469363922c"
            }
          ]
        }
      ]
    }
  ]
}
{
  "info": {
    "name": "Getty Images Get Images",
    "_postman_id": "cfbd11fd-19a3-4ed9-8a36-28d0ffcd6a5d",
    "description": "This endpoint returns the detailed image metadata for all specified images. Due to a wide variety of available image resolutions,\r\nthe images are grouped into a handful of size categories for simplicity. \r\n\r\nYou'll need an API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html) \r\npage for more information on how to sign up for an API key. \r\n\r\n## Working with Fields Sets\r\n\r\nFields sets are used in the **fields** request parameter to receive a suite of metadata fields. The following fields sets are available:\r\n\r\n#### Summary Fields Set\r\n\r\nThe **summary_set** query string parameter fields value represents a small batch of metadata fields that are often used to build \r\nsearch response results. The following fields are provided for every image in your result set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n    [\r\n        \"artist\",\r\n        \"asset_family\",\r\n        \"caption\",\r\n        \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields value represents a large batch of metadata fields that are often used to build a \r\ndetailed view of images. The following fields are provided for every image in your result set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n    [\r\n        \"allowed_use\",\r\n        \"artist\", \r\n        \"artist_title\", \r\n        \"asset_family\",\r\n        \"call_for_image\",\r\n        \"caption\", \r\n        \"city\",\r\n        \"collection_code\",\r\n        \"collection_id\", \r\n        \"collection_name\",\r\n        \"color_type\", \r\n        \"copyright\", \r\n        \"country\", \r\n        \"credit_line\", \r\n        \"date_created\", \r\n        \"date_submitted\",\r\n        \"download_sizes\", \r\n        \"editorial_segments\",\r\n        \"event_ids\",\r\n        \"graphical_style\",\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n        \"orientation\",\r\n        \"prestige\",\r\n        \"product_types\",\r\n        \"quality_rank\",\r\n        \"referral_destinations\",\r\n        \"state_province\", \r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Display Fields Set\r\n\r\nThe **display_set** query string parameter fields value represents the fields that provide you with URLs for the low resolution\r\nfiles that are most frequently used to build a UI displaying search results. The following fields are provided for every image \r\nin your result set when you include **display_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n    [\r\n        \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n            },\r\n            {\r\n                \"name\": \"thumb\"\r\n            }\r\n        ]\r\n    ]\r\n}\r\n```\r\n\r\n## Request Usage Considerations\r\n\r\n- Specifying the \"entity_details\" response field can have significant performance implications. The field should be used only when necessary.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "3704b089-63fa-49bb-b413-11a86fb11ed2",
          "name": "Images_GetBatch",
          "request": {
            "url": "http://api.gettyimages.com/v3/images?fields=%7B%7D&ids=%7B%7D",
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
            "description": "This endpoint returns the detailed image metadata for all specified images"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "912fcdb3-3963-4b98-8f7c-16f81e601ee3"
            }
          ]
        }
      ]
    }
  ]
}
{
  "info": {
    "name": "Getty Images Get Asset Change Notification",
    "_postman_id": "2343a511-32b7-4667-bf4a-e00782751cc4",
    "description": "# Delete Asset Changes\r\n\r\nConfirm asset changes acknowledges receipt of asset changes (from the PUT asset changes endpoint).\r\n\r\n##  Quickstart\r\n\r\nYou'll need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html) access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html) page for more information on how to sign up for an API key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "bd96b59d-b010-45a2-afcc-7e66e517f881",
          "name": "AssetChanges_DeleteAssetChanges",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.gettyimages.com",
              "path": [
                "v3/asset-changes/change-sets/:change-set-id"
              ],
              "variable": [
                {
                  "id": "change-set-id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
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
            "description": "# Delete Asset Changes\r\n\r\nConfirm asset changes acknowledges receipt of asset changes (from the PUT asset changes endpoint)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d87ab604-9c4e-4eb3-9a06-d44c3b26d7d5"
            }
          ]
        }
      ]
    }
  ]
}
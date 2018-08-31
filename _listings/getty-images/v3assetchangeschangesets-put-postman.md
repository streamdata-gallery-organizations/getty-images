{
  "info": {
    "name": "Getty Images Get Asset Change Notifications",
    "_postman_id": "ba94923c-2e21-4387-8cb9-531f41a9aae1",
    "description": "# Asset Changes\r\n\r\nGet notifications about new, updated or deleted assets.\r\n\r\n##  Quickstart\r\n\r\nYou'll need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html) access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html) page for more information on how to sign up for an API key. \r\n\r\n    \r\nPartner channels that have not been checked within the last 120 days will be removed and that partner will no longer be able \r\nto get change notifications from that channel.\r\nPartners who would like to start using the Asset Changes API again after a period of dormancy should contact their sales\r\nrepresentative to be set up again.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "4fbe59e3-9fa7-4a1a-9b1d-166e7274a7bb",
          "name": "AssetChanges_PutAssetChanges",
          "request": {
            "url": "http://api.gettyimages.com/v3/asset-changes/change-sets?batch_size=%7B%7D&channel_id=%7B%7D",
            "method": "PUT",
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
            "description": "# Asset Changes\r\n\r\nGet notifications about new, updated or deleted assets"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "036656ab-f5b1-4a04-8c33-05c64cefd341"
            }
          ]
        }
      ]
    }
  ]
}
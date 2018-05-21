{
  "info": {
    "name": "Getty Images Get Asset Change Channels",
    "_postman_id": "74c90847-e401-49d4-982e-d07c4a154ccf",
    "description": "# Get Partner Channels\r\n\r\nRetrieves the channel data for the partner. This data can be used to populate the channel_id parameter in the Put Asset Changes query.\r\n\r\n##  Quickstart\r\n\r\nYou'll need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html) access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html) page for more information on how to sign up for an API key. \r\n\r\nOnly channels that have been queried in the last 120 days will be included in the list of channels.\r\nPartners who have a channel that has been removed should contact their sales representative to be set up again.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "cf541ae8-6b28-4320-a763-f43b2d7be10f",
          "name": "AssetChanges_GetPartnerChannel",
          "request": {
            "url": "http://api.gettyimages.com/v3/asset-changes/channels",
            "method": "GET",
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
            "description": "# Get Partner Channels\r\n\r\nRetrieves the channel data for the partner"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6fb41640-6572-4a88-896e-0f83fd0eac8e"
            }
          ]
        }
      ]
    }
  ]
}
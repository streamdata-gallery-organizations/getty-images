{
  "info": {
    "name": "Getty Images Get metadata for multiple events",
    "_postman_id": "adeda0f6-2740-4d9e-b545-208f708ede48",
    "description": "This endpoint returns the detailed event metadata for all specified events. Getty Images news, sports and entertainment photographers and\r\nvideographers cover editorially relevant events occurring around the world.  All images or video clips produced in association with \r\nan event, are assigned the same EventID. EventIDs are part of the meta-data returned in SearchForImages Results. Only content \r\nproduced under a Getty Images brand name (Getty Images News, Getty Images Sports, Getty Images Entertainment, Film Magic, Wire Image) \r\nwill be consistently assigned an EventID. The Event framework may also be used to group similar content, such as \r\n\"Hats from the Royal Wedding\" or \"Odd-ballOffbeat images of the week\". \r\n\r\nYou'll need an API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html) page for more information on how to sign up for an API key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "49a031cf-968f-477e-909d-a264f7e78e8c",
          "name": "Events_GetBatch",
          "request": {
            "url": "http://api.gettyimages.com/v3/events?fields=%7B%7D&ids=%7B%7D",
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
            "description": "This endpoint returns the detailed event metadata for all specified events"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "656c28e6-8274-4c15-a6e9-a8a5e33d8dba"
            }
          ]
        }
      ]
    }
  ]
}
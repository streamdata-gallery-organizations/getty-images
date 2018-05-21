{
  "info": {
    "name": "Getty Images Get metadata for a single event",
    "_postman_id": "63f44f94-bcf7-429f-b972-ce6995c87e36",
    "description": "This endpoint returns the detailed event metadata for a specified event. Getty Images news, sports and entertainment \r\nphotographers and videographers cover editorially relevant events occurring around the world.  \r\nAll images or video clips produced in association with an event, are assigned the same EventID. \r\nEventIDs are part of the meta-data returned in SearchForImages Results. Only content produced under a Getty Images \r\nbrand name (Getty Images News, Getty Images Sports, Getty Images Entertainment, Film Magic, Wire Image) will be \r\nconsistently assigned an EventID. The Event framework may also be used to group similar content, such as \r\n\"Hats from the Royal Wedding\" or \"Odd-ballOffbeat images of the week\". \r\n\r\nYou'll need an API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage for more information on how to sign up for an API key.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "09e16e5c-4a29-426f-9c67-f746dfa370c2",
          "name": "Events_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.gettyimages.com",
              "path": [
                "v3/events/:id"
              ],
              "query": [
                {
                  "key": "fields",
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
            "description": "This endpoint returns the detailed event metadata for a specified event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae3f910e-7a13-4271-bd38-05e71454d334"
            }
          ]
        }
      ]
    }
  ]
}
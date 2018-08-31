{
  "info": {
    "name": "Getty Images",
    "_postman_id": "5a9fa16a-601d-4bb7-a94e-749116323110",
    "description": "Build applications using the world's most powerful imagery",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "ae9fea4e-070f-43ca-80f9-3a5f53793aa4",
          "name": "Artists_GetImagesByArtist",
          "request": {
            "url": "http://api.gettyimages.com/v3/artists/images?artist_name=%7B%7D&fields=%7B%7D&page=%7B%7D&page_size=%7B%7D",
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
            "description": "Search for images by a photographer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ac010f6-cbfb-47a1-87f5-6c03265bd347"
            }
          ]
        }
      ]
    }
  ]
}
{
  "info": {
    "name": "Getty Images Search Images",
    "_postman_id": "103e396f-8ec9-4858-87b0-667221386dd0",
    "description": "Use this endpoint to search over a blend of our contemporary stock photos, illustrations, archival images, editorial photos, illustrations and archival images.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "a3bcbb98-1609-4b20-af5b-a260e6ab6806",
          "name": "Search_GetImagesByPhrase",
          "request": {
            "url": "http://api.gettyimages.com/v3/search/images?age_of_people=%7B%7D&artists=%7B%7D&collections_filter_type=%7B%7D&collection_codes=%7B%7D&color=%7B%7D&compositions=%7B%7D&embed_content_only=%7B%7D&ethnicity=%7B%7D&event_ids=%7B%7D&exclude_nudity=%7B%7D&fields=%7B%7D&file_types=%7B%7D&graphical_styles=%7B%7D&keyword_ids=%7B%7D&license_models=%7B%7D&minimum_size=%7B%7D&number_of_people=%7B%7D&orientations=%7B%7D&page=%7B%7D&page_size=%7B%7D&phrase=%7B%7D&prestige_content_only=%7B%7D&product_types=%7B%7D&sort_order=%7B%7D&specific_people=%7B%7D",
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
            "description": "Use this endpoint to search over a blend of our contemporary stock photos, illustrations, archival images, editorial photos, illustrations and archival images"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0cbc0662-ce75-49f4-a360-638047127b7a"
            }
          ]
        }
      ]
    }
  ]
}
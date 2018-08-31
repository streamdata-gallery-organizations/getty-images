{
  "info": {
    "name": "Getty Images Search Editorial Images",
    "_postman_id": "b9b57bbd-5b5e-4606-a87d-603e37c459f8",
    "description": "Use this endpoint to search our editorial stock photos, illustrations and archival images.  Editorial images represent newsworthy events or illustrate matters of general interest, such as news, sport and entertainment and are generally intended for editorial use.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "29696116-4693-409f-a207-31a7fee719c0",
          "name": "Search_GetEditorialImagesByPhrase",
          "request": {
            "url": "http://api.gettyimages.com/v3/search/images/editorial?age_of_people=%7B%7D&artists=%7B%7D&collections_filter_type=%7B%7D&collection_codes=%7B%7D&compositions=%7B%7D&editorial_segments=%7B%7D&embed_content_only=%7B%7D&end_date=%7B%7D&entity_uris=%7B%7D&ethnicity=%7B%7D&event_ids=%7B%7D&exclude_nudity=%7B%7D&fields=%7B%7D&file_types=%7B%7D&graphical_styles=%7B%7D&keyword_ids=%7B%7D&minimum_quality_rank=%7B%7D&minimum_size=%7B%7D&number_of_people=%7B%7D&orientations=%7B%7D&page=%7B%7D&page_size=%7B%7D&phrase=%7B%7D&product_types=%7B%7D&sort_order=%7B%7D&specific_people=%7B%7D&start_date=%7B%7D",
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
            "description": "Use this endpoint to search our editorial stock photos, illustrations and archival images"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa10ca92-52cc-4083-acc1-5c26a4787f22"
            }
          ]
        }
      ]
    }
  ]
}
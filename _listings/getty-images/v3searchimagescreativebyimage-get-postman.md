{
  "info": {
    "name": "Getty Images Search Images by Image",
    "_postman_id": "190643cc-da07-464a-bb77-bced8ef14ddf",
    "description": "Allows searching for similar creative images by passing the URL to an existing image.\r\n\r\nBefore calling the search by image endpoint, an image must be uploaded to a specific AWS S3 bucket. The bucket name is `search-by-image.s3.amazonaws.com`.\r\nFor example, using cURL:\r\n```sh\r\ncurl -i -X PUT https://search-by-image.s3.amazonaws.com/my-test-image.jpg -H \"Content-Type: image/jpeg\" --data-binary \"@testimage.jpg\"\r\n```\r\n\r\nUploads can be overwritten if the names are the same, so using a prefix like the API Key, application name or company name would help keep that\r\nfrom happening.\r\n\r\nOnce the image has been uploaded, use the full URL in the `image_url` parameter, e.g. `image_url=https://search-by-image.s3.amazonaws.com/my-test-image.jpg`.\r\n\r\nSubsequent searches for the same image can be executed using the `image_fingerprint` that is returned by the inital search.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "images",
      "item": [
        {
          "id": "7edf9aa3-f107-442d-be1c-f16840d05c77",
          "name": "Search_GetCreativeImagesByUrl",
          "request": {
            "url": "http://api.gettyimages.com/v3/search/images/creative/by-image?fields=%7B%7D&image_fingerprint=%7B%7D&image_url=%7B%7D&page=%7B%7D&page_size=%7B%7D&product_types=%7B%7D",
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
            "description": "Allows searching for similar creative images by passing the URL to an existing image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d07499e-7b57-41a8-98e4-b70b645dacd5"
            }
          ]
        }
      ]
    }
  ]
}
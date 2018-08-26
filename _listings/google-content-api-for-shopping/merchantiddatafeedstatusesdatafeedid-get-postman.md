{
  "info": {
    "name": "Google Content API for Shopping API Get Data Feed Status",
    "_postman_id": "4b086824-f7a3-4e15-83d0-410aae28e017",
    "description": "Retrieves the status of a datafeed from your Merchant Center account. This method can only be called for non-multi-client accounts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "data",
      "item": [
        {
          "id": "44fb4394-dfd3-44a6-94aa-1d2a113b8df9",
          "name": "content.datafeedstatuses.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "content",
                "v2",
                ":merchantId/datafeedstatuses/:datafeedId"
              ],
              "variable": [
                {
                  "id": "datafeedId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "merchantId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the status of a datafeed from your Merchant Center account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21b683c4-55cc-469b-9fb5-60374b618b2f"
            }
          ]
        }
      ]
    }
  ]
}
{
  "info": {
    "name": "Google Content API for Shopping API Get Data Feed",
    "_postman_id": "0cd9de2a-c8cf-463d-aaa5-23d87045b37a",
    "description": "Retrieves a datafeed from your Merchant Center account. This method can only be called for non-multi-client accounts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "data",
      "item": [
        {
          "id": "9d4ebdf7-c3c0-49d8-875c-470709da5e20",
          "name": "content.datafeeds.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "content",
                "v2",
                ":merchantId/datafeeds/:datafeedId"
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
            "description": "Retrieves a datafeed from your Merchant Center account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8cd95b19-7c91-42b3-8a2f-ba307c6fbf04"
            }
          ]
        }
      ]
    }
  ]
}
{
  "info": {
    "name": "Google Content API for Shopping API Delete Data Feed",
    "_postman_id": "568d43a1-b9b3-42c5-b291-b1b35aa838e0",
    "description": "Deletes a datafeed from your Merchant Center account. This method can only be called for non-multi-client accounts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "data",
      "item": [
        {
          "id": "0877d1e3-d436-452f-a0d4-05fc87b9cdfc",
          "name": "content.datafeeds.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "content",
                "v2",
                ":merchantId/datafeeds/:datafeedId"
              ],
              "query": [
                {
                  "key": "dryRun",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a datafeed from your Merchant Center account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02e5ade4-16f7-487b-b562-cc08cf09f4cf"
            }
          ]
        }
      ]
    }
  ]
}
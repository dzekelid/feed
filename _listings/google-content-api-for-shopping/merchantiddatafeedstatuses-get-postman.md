{
  "info": {
    "name": "Google Content API for Shopping API Get Data Feed Status",
    "_postman_id": "e68ee864-fcd5-4f18-8d84-f0a45fa808a3",
    "description": "Lists the statuses of the datafeeds in your Merchant Center account. This method can only be called for non-multi-client accounts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "data",
      "item": [
        {
          "id": "4cc1195a-04d4-4936-a0c3-4f92e52ea86b",
          "name": "content.datafeedstatuses.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "content",
                "v2",
                ":merchantId/datafeedstatuses"
              ],
              "query": [
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
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
            "description": "Lists the statuses of the datafeeds in your Merchant Center account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1548dc02-b8f2-4386-8238-c55172ce40d0"
            }
          ]
        }
      ]
    }
  ]
}
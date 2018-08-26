{
  "info": {
    "name": "Steem get_feed_history",
    "_postman_id": "927cb4e0-e0e7-498a-94ad-0a78674c5d2b",
    "description": "get_feed_history",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "1d274fac-357f-4587-95f4-bb5cdcd84b3c",
          "name": "get-feed-history",
          "request": {
            "url": "http://api.steemjs.com/get_feed_history",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "get_feed_history"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9cf4281d-4c01-48ab-ad96-939cd8e0dbbe"
            }
          ]
        }
      ]
    }
  ]
}
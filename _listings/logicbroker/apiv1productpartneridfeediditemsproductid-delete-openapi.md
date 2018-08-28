---
swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 0
info:
  title: Logic Broker CommerceAPI Remove product feed item.
  version: 1.0.0
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Product/{partnerId}/{feedId}/Items/{productId}:
    delete:
      summary: Remove product feed item.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_RemoveFeedItem
      x-api-path-slug: apiv1productpartneridfeediditemsproductid-delete
      parameters:
      - in: path
        name: feedId
        description: Feed identifier
      - in: path
        name: partnerId
        description: Partner account number
      - in: path
        name: productId
        description: Product identifier within the feed
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Product
      - Feed
      - Item
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---
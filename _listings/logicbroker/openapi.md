swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 1
info:
  title: CommerceAPI
  version: 1.0.0
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
    put:
      summary: Update product feed item.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_UpdateFeedItem
      x-api-path-slug: apiv1productpartneridfeediditemsproductid-put
      parameters:
      - in: body
        name: data
        description: Data fields to update
        schema:
          $ref: '#/definitions/holder'
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
      - Product
      - Feed
      - Item
    get:
      summary: Get product feed item.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_GetFeedItem
      x-api-path-slug: apiv1productpartneridfeediditemsproductid-get
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
      - Product
      - Feed
      - Item
  /api/v1/Product/{partnerId}/{feedId}/Items:
    get:
      summary: Get items in the product feed.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_GetFeedItems
      x-api-path-slug: apiv1productpartneridfeediditems-get
      parameters:
      - in: path
        name: feedId
        description: Feed identifier
      - in: query
        name: isCompliant
        description: Compliant filter
      - in: query
        name: page
        description: Page number
      - in: query
        name: pageSize
        description: Page size
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - Items
      - In
      - Product
      - Feed
  /api/v1/Product/{partnerId}/{feedId}:
    delete:
      summary: Delete product feed.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_DeleteFeed
      x-api-path-slug: apiv1productpartneridfeedid-delete
      parameters:
      - in: path
        name: feedId
        description: Feed identifier
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - Product
      - Feed
    put:
      summary: Send product feed.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_SendFeed
      x-api-path-slug: apiv1productpartneridfeedid-put
      parameters:
      - in: path
        name: feedId
        description: Feed identifier
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - Send
      - Product
      - Feed
    get:
      summary: Get product feed status.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_GetFeedStatus
      x-api-path-slug: apiv1productpartneridfeedid-get
      parameters:
      - in: path
        name: feedId
        description: Feed identifier
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - Product
      - Feed
      - Status
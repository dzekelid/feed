---
swagger: "2.0"
x-collection-name: Google Content API for Shopping
x-complete: 0
info:
  title: Google Content API for Shopping API Update Data Feed
  description: Updates a datafeed of your Merchant Center account. This method can
    only be called for non-multi-client accounts.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /content/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /datafeedstatuses/batch:
    post:
      summary: Data Feed Status
      description: Retrieves data feed batch status.
      operationId: content.datafeedstatuses.custombatch
      x-api-path-slug: datafeedstatusesbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feed
      - Status
  /{merchantId}/datafeeds:
    post:
      summary: Create Data Feed
      description: Registers a datafeed with your Merchant Center account. This method
        can only be called for non-multi-client accounts.
      operationId: content.datafeeds.insert
      x-api-path-slug: merchantiddatafeeds-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feed
  /{merchantId}/datafeeds/{datafeedId}:
    delete:
      summary: Delete Data Feed
      description: Deletes a datafeed from your Merchant Center account. This method
        can only be called for non-multi-client accounts.
      operationId: content.datafeeds.delete
      x-api-path-slug: merchantiddatafeedsdatafeedid-delete
      parameters:
      - in: path
        name: datafeedId
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feed
    get:
      summary: Get Data Feed
      description: Retrieves a datafeed from your Merchant Center account. This method
        can only be called for non-multi-client accounts.
      operationId: content.datafeeds.get
      x-api-path-slug: merchantiddatafeedsdatafeedid-get
      parameters:
      - in: path
        name: datafeedId
      - in: path
        name: merchantId
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feed
    patch:
      summary: Update Data Feed
      description: Updates a datafeed of your Merchant Center account. This method
        can only be called for non-multi-client accounts. This method supports patch
        semantics.
      operationId: content.datafeeds.patch
      x-api-path-slug: merchantiddatafeedsdatafeedid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: datafeedId
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feed
    put:
      summary: Update Data Feed
      description: Updates a datafeed of your Merchant Center account. This method
        can only be called for non-multi-client accounts.
      operationId: content.datafeeds.update
      x-api-path-slug: merchantiddatafeedsdatafeedid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: datafeedId
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feed
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
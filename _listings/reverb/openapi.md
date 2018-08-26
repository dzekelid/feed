---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /my/feed:
    get:
      summary: Get My Feed
      description: Get listings from your feed
      operationId: getMyFeed
      x-api-path-slug: myfeed-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Feed
  /my/feed/customize:
    get:
      summary: Get My Feed Customize
      description: get your feed customization options
      operationId: getMyFeedCustomize
      x-api-path-slug: myfeedcustomize-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Feed
      - Customize
  /my/feed/grid:
    get:
      summary: Get My Feed Gr
      description: Get my feed gr.
      operationId: getMyFeedGr
      x-api-path-slug: myfeedgrid-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Feed
      - Grid
---
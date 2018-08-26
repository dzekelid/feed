---
swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 1
info:
  title: Urban Airship
  description: the-urban-airships-api-powers-mobile-applications-with-push-rich-push-inapp-purchases-and-subscription-services-
  version: v3
host: go.urbanairship.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /feeds/{feed_id}:
    get:
      summary: Get Feeds Feed
      description: Returns information about a particular feed.
      operationId: feeds.feed_id.get
      x-api-path-slug: feedsfeed-id-get
      parameters:
      - in: query
        name: feed_id
        description: A particular feed
      - in: path
        name: feed_id
      responses:
        200:
          description: OK
      tags:
      - Feeds
      - Feed
      - Id
    put:
      summary: Put Feeds Feed
      description: Updates a feed.
      operationId: feeds.feed_id.put
      x-api-path-slug: feedsfeed-id-put
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: feed_id
        description: A particular feed
      - in: path
        name: feed_id
      responses:
        200:
          description: OK
      tags:
      - Feeds
      - Feed
      - Id
    delete:
      summary: Delete Feeds Feed
      description: Deletes a feed.
      operationId: feeds.feed_id.delete
      x-api-path-slug: feedsfeed-id-delete
      parameters:
      - in: query
        name: feed_id
        description: A particular feed
      - in: path
        name: feed_id
      responses:
        200:
          description: OK
      tags:
      - Feeds
      - Feed
      - Id
---
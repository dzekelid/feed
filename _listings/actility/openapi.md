swagger: "2.0"
x-collection-name: Actility
x-complete: 1
info:
  title: ThingPark DX Maker API
  description: api-providing-features-for-device-makers-such-as-preprovisioning-on-standalone-join-servers-
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /maker/v011/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /feeds:
    post:
      summary: Feed request
      description: Feeds the platform with geolocation data. Data is then dispatched
        and processed based on available information.
      operationId: feeds-the-platform-with-geolocation-data-data-is-then-dispatched-and-processed-based-on-available-in
      x-api-path-slug: feeds-post
      parameters:
      - in: body
        name: feedRequest
        description: Contents of the feed request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Feed
      - Request
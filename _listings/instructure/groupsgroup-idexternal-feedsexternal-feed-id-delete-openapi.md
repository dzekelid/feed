---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Groups API Delete an external feed
  description: Delete an external feed.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/external_feeds/external_feed_id:
    delete:
      summary: Delete an external feed
      description: Delete an external feed.
      operationId: delete-an-external-feed
      x-api-path-slug: coursescourse-idexternal-feedsexternal-feed-id-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - External
      - Feeds
      - External
      - Feed
      - Id
  /courses/{course_id}/gradebook_history/feed:
    get:
      summary: List uncollated submission versions
      description: List uncollated submission versions.
      operationId: list-uncollated-submission-versions
      x-api-path-slug: coursescourse-idgradebook-historyfeed-get
      parameters:
      - in: query
        name: ascending
        description: Returns submission versions in ascending date order (oldest first)
      - in: query
        name: assignment_id
        description: The ID of the assignment for which you want to see submissions
      - in: query
        name: course_id
        description: The id of the contextual course for this API call
      - in: query
        name: user_id
        description: The ID of the user for which you want to see submissions
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Gradebook
      - History
      - Feed
  /groups/{group_id}/external_feeds/external_feed_id:
    delete:
      summary: Delete an external feed
      description: Delete an external feed.
      operationId: delete-an-external-feed
      x-api-path-slug: groupsgroup-idexternal-feedsexternal-feed-id-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - External
      - Feeds
      - External
      - Feed
      - Id
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
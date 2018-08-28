swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
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
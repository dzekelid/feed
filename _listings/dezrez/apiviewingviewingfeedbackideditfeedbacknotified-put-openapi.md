---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Edit that the feedback for a Viewing was notified to the vendor.
  version: 1.0.0
  description: Edit that the feedback for a viewing was notified to the vendor..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/list/feedbackfollowups/filters/{id}:
    delete:
      summary: Marks Feedback Follow Up List Filter as deleted
      description: Marks feedback follow up list filter as deleted.
      operationId: List_DeleteFeedbackFollowUpListFilterByid
      x-api-path-slug: apilistfeedbackfollowupsfiltersid-delete
      parameters:
      - in: path
        name: id
        description: Id of filter to delete
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Feedback
      - Follow
      - Up
      - List
      - Filter
      - As
      - Deleted
  /api/viewing/{viewingFeedbackId}/editfeedbacknotified:
    put:
      summary: Edit that the feedback for a Viewing was notified to the vendor.
      description: Edit that the feedback for a viewing was notified to the vendor..
      operationId: Viewing_EditFeedbackNotifiedByviewingFeedbackIdByvendorNotifiedIdBytypeBynotifiedDateBynegIds
      x-api-path-slug: apiviewingviewingfeedbackideditfeedbacknotified-put
      parameters:
      - in: query
        name: negIds
      - in: query
        name: notifiedDate
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: type
        description: Task type for how vendor was communicated e
      - in: query
        name: vendorNotifiedId
        description: vendor notified id
      - in: path
        name: viewingFeedbackId
        description: viewing feedback id
      responses:
        200:
          description: OK
      tags:
      - Edit
      - That
      - Feedbacka
      - Viewing
      - Was
      - Notified
      - To
      - Vendor
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
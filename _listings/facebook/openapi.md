swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{application}/feed:
    get:
      summary: Get Application Feed
      description: The application's wall.
      operationId: getApplicationFeed
      x-api-path-slug: applicationfeed-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Feed
    post:
      summary: Post Application Feed
      description: Posts a status message on the application's profile page
      operationId: postApplicationFeed
      x-api-path-slug: applicationfeed-post
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      - in: query
        name: message
        description: Status Message content
      responses:
        200:
          description: OK
      tags:
      - Application
      - Feed
  /{event}/feed:
    get:
      summary: Get Event Feed
      description: This event's wall
      operationId: getEventFeed
      x-api-path-slug: eventfeed-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Feed
    post:
      summary: Post Event Feed
      description: Posts a status message on this event's wall
      operationId: postEventFeed
      x-api-path-slug: eventfeed-post
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      - in: query
        name: message
        description: Status Message content
      responses:
        200:
          description: OK
      tags:
      - Event
      - Feed
  /{group}/feed:
    get:
      summary: Get Group Feed
      description: This group's wall
      operationId: getGroupFeed
      x-api-path-slug: groupfeed-get
      parameters:
      - in: path
        name: group
        description: Represents the ID of the group object
      responses:
        200:
          description: OK
      tags:
      - Group
      - Feed
    post:
      summary: Post Group Feed
      description: Posts a status message on this group's wall
      operationId: postGroupFeed
      x-api-path-slug: groupfeed-post
      parameters:
      - in: path
        name: group
        description: Represents the ID of the group object
      - in: query
        name: message
        description: Status Message content
      responses:
        200:
          description: OK
      tags:
      - Group
      - Feed
  /{page}/feed:
    get:
      summary: Get Page Feed
      description: This page's wall
      operationId: getPageFeed
      x-api-path-slug: pagefeed-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Feed
    post:
      summary: Post Page Feed
      description: Posts a status message on this page's wall
      operationId: postPageFeed
      x-api-path-slug: pagefeed-post
      parameters:
      - in: query
        name: message
        description: Status Message content
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Feed
  /{user}/feed:
    get:
      summary: Get User Feed
      description: This user's wall
      operationId: getUserFeed
      x-api-path-slug: userfeed-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Feed
    post:
      summary: Post User Feed
      description: Posts a status message on this user's wall
      operationId: postUserFeed
      x-api-path-slug: userfeed-post
      parameters:
      - in: query
        name: message
        description: Status Message content
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Feed
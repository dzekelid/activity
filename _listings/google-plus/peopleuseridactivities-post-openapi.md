---
swagger: "2.0"
x-collection-name: Google Plus
x-complete: 0
info:
  title: Google Plus Create Activity
  version: 1.0.0
  description: Create a new activity for the authenticated user.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activities:
    get:
      summary: Get Activities
      description: Search public activities.
      operationId: plus.activities.search
      x-api-path-slug: activities-get
      parameters:
      - in: query
        name: language
        description: Specify the preferred language to search with
      - in: query
        name: maxResults
        description: The maximum number of activities to include in the response,
          which is used for paging
      - in: query
        name: orderBy
        description: Specifies how to order search results
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      - in: query
        name: query
        description: Full-text search query string
      responses:
        200:
          description: OK
      tags:
      - Activity
  /activities/{activityId}:
    get:
      summary: Get Activity
      description: Get an activity.
      operationId: plusDomains.activities.get
      x-api-path-slug: activitiesactivityid-get
      parameters:
      - in: path
        name: activityId
        description: The ID of the activity to get
      responses:
        200:
          description: OK
      tags:
      - Activity
  /people/{userId}/activities/{collection}:
    get:
      summary: Get Colelction Activities
      description: List all of the activities in the specified collection for a particular
        user.
      operationId: plus.activities.list
      x-api-path-slug: peopleuseridactivitiescollection-get
      parameters:
      - in: path
        name: collection
        description: The collection of activities to list
      - in: query
        name: maxResults
        description: The maximum number of activities to include in the response,
          which is used for paging
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      - in: path
        name: userId
        description: The ID of the user to get activities for
      responses:
        200:
          description: OK
      tags:
      - Activity
  /activities/{activityId}/comments:
    get:
      summary: Get Activity Commenets
      description: List all of the comments for an activity.
      operationId: plusDomains.comments.list
      x-api-path-slug: activitiesactivityidcomments-get
      parameters:
      - in: path
        name: activityId
        description: The ID of the activity to get comments for
      - in: query
        name: maxResults
        description: The maximum number of comments to include in the response, which
          is used for paging
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      - in: query
        name: sortOrder
        description: The order in which to sort the list of comments
      responses:
        200:
          description: OK
      tags:
      - Activity
    post:
      summary: Create Activity Comment
      description: Create a new comment in reply to an activity.
      operationId: plusDomains.comments.insert
      x-api-path-slug: activitiesactivityidcomments-post
      parameters:
      - in: path
        name: activityId
        description: The ID of the activity to reply to
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Activity
  /people/{userId}/activities:
    post:
      summary: Create Activity
      description: Create a new activity for the authenticated user.
      operationId: plusDomains.activities.insert
      x-api-path-slug: peopleuseridactivities-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: preview
        description: If true, extract the potential media attachments for a URL
      - in: path
        name: userId
        description: The ID of the user to create the activity on behalf of
      responses:
        200:
          description: OK
      tags:
      - Activity
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
---
swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 0
info:
  title: Constant Contact Get Activity
  description: Get Activity
  version: 1.0.0
host: api.constantcontact.com
basePath: /ws/customers/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{username}/activities:
    post:
      summary: Add Activity
      description: Add Activity
      operationId: add-activity
      x-api-path-slug: usernameactivities-post
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Activity
  /{username}/activities/{activity-id}:
    get:
      summary: Get Activity
      description: Get Activity
      operationId: get-activity
      x-api-path-slug: usernameactivitiesactivityid-get
      parameters:
      - in: path
        name: activity-id
      - in: path
        name: username
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
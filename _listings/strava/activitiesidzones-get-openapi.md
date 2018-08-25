---
swagger: "2.0"
x-collection-name: Strava
x-complete: 0
info:
  title: Strava Get Activity Zones
  description: Premium Feature. Returns the zones of a given activity.
  version: 1.0.0
host: www.strava.com
basePath: /api/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activities:
    post:
      summary: Create an Activity
      description: Creates a manual activity for an athlete. Requires write permissions,
        as requested during the authorization process.
      operationId: createActivity
      x-api-path-slug: activities-post
      parameters:
      - in: formData
        name: commute
        description: Set to 1 to mark as commute
      - in: formData
        name: description
        description: Description of the activity
      - in: formData
        name: distance
        description: In meters
      - in: formData
        name: elapsed_time
        description: In seconds
      - in: formData
        name: name
        description: The name of the activity
      - in: formData
        name: photo_ids
        description: List of native photo ids to attach to the activity
      - in: formData
        name: private
        description: set to 1 to mark the resulting activity as private, ???view_private???
          permissions will be necessary to view the activity
      - in: formData
        name: start_date_local
        description: ISO 8601 formatted date time
      - in: formData
        name: trainer
        description: Set to 1 to mark as a trainer activity
      - in: formData
        name: type
        description: Type of activity
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Activity
  /activities/{id}:
    get:
      summary: Get Activity
      description: Returns the given activity that is owned by the authenticated athlete.
      operationId: getActivityById
      x-api-path-slug: activitiesid-get
      parameters:
      - in: path
        name: id
        description: The identifier of the activity
      - in: query
        name: include_all_efforts
        description: To include all segments efforts
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Activity
    put:
      summary: Update Activity
      description: Updates the given activity that is owned by the authenticated athlete.
      operationId: updateActivityById
      x-api-path-slug: activitiesid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The identifier of the activity
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Activity
  /activities/{id}/laps:
    get:
      summary: List Activity Laps
      description: Returns the laps of an activity identified by an identifier.
      operationId: getLapsByActivityId
      x-api-path-slug: activitiesidlaps-get
      parameters:
      - in: path
        name: id
        description: The identifier of the activity
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Activity
      - Laps
  /activities/{id}/zones:
    get:
      summary: Get Activity Zones
      description: Premium Feature. Returns the zones of a given activity.
      operationId: getZonesByActivityId
      x-api-path-slug: activitiesidzones-get
      parameters:
      - in: path
        name: id
        description: The identifier of the activity
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Activity
      - Zones
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
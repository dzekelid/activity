---
swagger: "2.0"
x-collection-name: AWS Step Functions
x-complete: 0
info:
  title: AWS Step Functions API Create Activity
  version: 1.0.0
  description: Creates an activity.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateActivity:
    get:
      summary: Create Activity
      description: Creates an activity.
      operationId: createActivity
      x-api-path-slug: actioncreateactivity-get
      parameters:
      - in: query
        name: name
        description: The name of the activity to create
        type: string
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
---
swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 0
info:
  title: Logic Broker CommerceAPI Update activity event
  version: 1.0.0
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/ActivityEvents:
    get:
      summary: Get events for given fitlers
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: ActivityEvent_SearchActivityEvent
      x-api-path-slug: apiv1activityevents-get
      parameters:
      - in: query
        name: Filters.category
        description: Gets or sets the invoice number
      - in: query
        name: Filters.documentType
        description: Gets or sets the shipment number
      - in: query
        name: Filters.from
        description: Gets or sets the start date
      - in: query
        name: Filters.level
        description: Gets or sets the status
      - in: query
        name: Filters.linkKey
        description: Gets or sets the order number
      - in: query
        name: Filters.logicbrokerKey
        description: Gets or sets the order number
      - in: query
        name: Filters.page
        description: Gets or sets the page
      - in: query
        name: Filters.processed
        description: Gets or sets the company id
      - in: query
        name: Filters.receiverId
        description: Gets or sets the company id
      - in: query
        name: Filters.senderId
        description: Gets or sets the partner company id
      - in: query
        name: Filters.to
        description: Gets or sets the end date
      - in: query
        name: Filters.typeId
        description: Gets or sets the event type id
      - in: query
        name: Filters.viewed
        description: Gets or sets the company id
      responses:
        200:
          description: OK
      tags:
      - Eventsgiven
      - Fitlers
    post:
      summary: Create an activity event.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: ActivityEvent_CreateEvent
      x-api-path-slug: apiv1activityevents-post
      parameters:
      - in: body
        name: ActivityEvent
        description: The Activity Event
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Activity
      - Event
  /api/v1/ActivityEvents/EventTypes:
    get:
      summary: Gets a list of all possible event types.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: ActivityEvent_GetEventTypes
      x-api-path-slug: apiv1activityeventseventtypes-get
      responses:
        200:
          description: OK
      tags:
      - S
      - List
      - Of
      - ""
      - Possible
      - Event
      - Types
  /api/v1/ActivityEvents/{EventId}:
    get:
      summary: Gets the event with the specified id.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: ActivityEvent_GetActivityEvent
      x-api-path-slug: apiv1activityeventseventid-get
      parameters:
      - in: path
        name: EventId
        description: The id to search for
      responses:
        200:
          description: OK
      tags:
      - S
      - Event
      - Specified
      - Id
    put:
      summary: Update activity event
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: ActivityEvent_UpdateActivityEvent
      x-api-path-slug: apiv1activityeventseventid-put
      parameters:
      - in: body
        name: activityEvent
        description: The updated activityEvent
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: EventId
        description: The Event Id
      responses:
        200:
          description: OK
      tags:
      - Activity
      - Event
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
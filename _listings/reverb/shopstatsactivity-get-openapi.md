---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: Reverb Get Shop Stats Activity
  description: Get shop activity for a particular time period
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shop/stats/activity:
    get:
      summary: Get Shop Stats Activity
      description: Get shop activity for a particular time period
      operationId: getShopStatsActivity
      x-api-path-slug: shopstatsactivity-get
      parameters:
      - in: query
        name: end_time
        description: Filter by date in ISO8601 format - e
      - in: query
        name: start_time
        description: Filter by date in ISO8601 format - e
      responses:
        200:
          description: OK
      tags:
      - Shop
      - Stats
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
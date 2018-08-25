---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
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
---
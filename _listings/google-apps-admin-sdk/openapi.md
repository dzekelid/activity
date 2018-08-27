swagger: "2.0"
x-collection-name: Google Apps Admin SDK
x-complete: 1
info:
  title: Google Apps Admin SDK Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activity/users/{userKey}/applications/{applicationName}/watch:
    post:
      summary: Change Activity
      description: Push changes to activities
      operationId: reports.activities.watch
      x-api-path-slug: activityusersuserkeyapplicationsapplicationnamewatch-post
      parameters:
      - in: query
        name: actorIpAddress
        description: IP Address of host where the event was performed
      - in: path
        name: applicationName
        description: Application name for which the events are to be retrieved
      - in: query
        name: customerId
        description: Represents the customer for which the data is to be fetched
      - in: query
        name: endTime
        description: Return events which occured at or before this time
      - in: query
        name: eventName
        description: Name of the event being queried
      - in: query
        name: filters
        description: Event parameters in the form [parameter1 name][operator][parameter1
          value],[parameter2 name][operator][parameter2 value],
      - in: query
        name: maxResults
        description: Number of activity records to be shown in each page
      - in: query
        name: pageToken
        description: Token to specify next page
      - in: body
        name: resource
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: startTime
        description: Return events which occured at or after this time
      - in: path
        name: userKey
        description: Represents the profile id or the user email for which the data
          should be filtered
      responses:
        200:
          description: OK
      tags:
      - Activities
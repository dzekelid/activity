swagger: "2.0"
x-collection-name: AWS Step Functions
x-complete: 1
info:
  title: AWS Step Functions API
  version: 1.0.0
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
  /?Action=DeleteActivity:
    get:
      summary: Delete Activity
      description: Deletes an activity.
      operationId: deleteActivity
      x-api-path-slug: actiondeleteactivity-get
      parameters:
      - in: query
        name: activityArn
        description: The Amazon Resource Name (ARN) of the activity to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Activity
  /?Action=DescribeActivity:
    get:
      summary: Describe Activity
      description: Describes an activity.
      operationId: describeActivity
      x-api-path-slug: actiondescribeactivity-get
      parameters:
      - in: query
        name: activityArn
        description: The Amazon Resource Name (ARN) of the activity to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Activity
  /?Action=ListActivities:
    get:
      summary: List Activities
      description: Lists the existing activities.
      operationId: listActivities
      x-api-path-slug: actionlistactivities-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of results that will be returned per call
        type: string
      - in: query
        name: nextToken
        description: If a nextToken was returned by a previous call, there are more
          results available
        type: string
      responses:
        200:
          description: OK
      tags:
      - Activity
  /?Action=GetActivityTask:
    get:
      summary: Get Activity Task
      description: "Used by workers to retrieve a task (with the specified activity
        ARN) which has been scheduled \n    for execution by a running state machine."
      operationId: getActivityTask
      x-api-path-slug: actiongetactivitytask-get
      parameters:
      - in: query
        name: activityArn
        description: The Amazon Resource Name (ARN) of the activity to retrieve tasks
          from (assigned when you create the task      using CreateActivity
        type: string
      - in: query
        name: workerName
        description: You can provide an arbitrary name in order to identify the worker
          that the task is assigned to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Activity Task
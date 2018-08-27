swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/activity_stream:
    get:
      summary: Course activity stream
      description: Course activity stream.
      operationId: course-activity-stream
      x-api-path-slug: coursescourse-idactivity-stream-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Activity
      - Stream
  /courses/{course_id}/activity_stream/summary:
    get:
      summary: Course activity stream summary
      description: Course activity stream summary.
      operationId: course-activity-stream-summary
      x-api-path-slug: coursescourse-idactivity-streamsummary-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Activity
      - Stream
      - Summary
  /courses/{course_id}/analytics/activity:
    get:
      summary: Get course-level participation data
      description: Get course-level participation data.
      operationId: get-courselevel-participation-data
      x-api-path-slug: coursescourse-idanalyticsactivity-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Analytics
      - Activity
  /courses/{course_id}/analytics/users/student_id/activity:
    get:
      summary: Get user-in-a-course-level participation data
      description: Get user-in-a-course-level participation data.
      operationId: get-userinacourselevel-participation-data
      x-api-path-slug: coursescourse-idanalyticsusersstudent-idactivity-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Analytics
      - Users
      - Student
      - Id
      - Activity
  /groups/{group_id}/activity_stream:
    get:
      summary: Group activity stream
      description: Group activity stream.
      operationId: group-activity-stream
      x-api-path-slug: groupsgroup-idactivity-stream-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Activity
      - Stream
  /groups/{group_id}/activity_stream/summary:
    get:
      summary: Group activity stream summary
      description: Group activity stream summary.
      operationId: group-activity-stream-summary
      x-api-path-slug: groupsgroup-idactivity-streamsummary-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Activity
      - Stream
      - Summary
  /users/activity_stream:
    get:
      summary: List the activity stream
      description: List the activity stream.
      operationId: list-the-activity-stream
      x-api-path-slug: usersactivity-stream-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Activity
      - Stream
  /users/self/activity_stream:
    delete:
      summary: Hide all stream items
      description: Hide all stream items.
      operationId: hide-all-stream-items
      x-api-path-slug: usersselfactivity-stream-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
    get:
      summary: List the activity stream
      description: List the activity stream.
      operationId: list-the-activity-stream
      x-api-path-slug: usersselfactivity-stream-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
  /users/self/activity_stream/summary:
    get:
      summary: Activity stream summary
      description: Activity stream summary.
      operationId: activity-stream-summary
      x-api-path-slug: usersselfactivity-streamsummary-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
      - Summary
  /users/self/activity_stream/{id}:
    delete:
      summary: Hide a stream item
      description: Hide a stream item.
      operationId: hide-a-stream-item
      x-api-path-slug: usersselfactivity-streamid-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
      - Id
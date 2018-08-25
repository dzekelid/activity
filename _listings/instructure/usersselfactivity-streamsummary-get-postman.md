{
  "info": {
    "name": "Instructure Canvas Users API Activity stream summary",
    "_postman_id": "73ce9127-2ba5-4fae-8756-979df012d03b",
    "description": "Activity stream summary.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "68199f46-afdf-4612-827b-cc6a2ae82126",
          "name": "list-the-activity-stream",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/activity_stream",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the activity stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3ffd12c-3a98-4199-b866-8e297d00c672"
            }
          ]
        },
        {
          "id": "7d94bd06-6d77-467b-8530-760ce01f437d",
          "name": "list-the-activity-stream1",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/activity_stream",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the activity stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56f65fdd-236b-40eb-9376-7ca90a3dab57"
            }
          ]
        },
        {
          "id": "f5a147db-ac85-4f7b-a7b7-9faf5b966ba1",
          "name": "hide-all-stream-items",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/activity_stream",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Hide all stream items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d81024ed-af25-4d03-a619-50be6a2f81b4"
            }
          ]
        },
        {
          "id": "05ef9c64-b31f-4bc3-be78-ca7830a15720",
          "name": "activity-stream-summary",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/activity_stream/summary",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Activity stream summary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae730287-809f-4d4d-adaa-6f88e9bf0222"
            }
          ]
        }
      ]
    }
  ]
}
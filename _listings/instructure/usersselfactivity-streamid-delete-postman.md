{
  "info": {
    "name": "Instructure Canvas Users API Hide a stream item",
    "_postman_id": "53902175-26a2-49a9-b28f-56a4c3bdbfaf",
    "description": "Hide a stream item.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "d271aece-c1e6-4067-bee7-f3d138270c08",
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
              "id": "a6f5dd5c-f054-4b95-bf10-3b2350ad1590"
            }
          ]
        },
        {
          "id": "874e94f0-0016-483e-b6b3-481875019c5b",
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
              "id": "b0c3b7c6-583f-4333-942b-0093fe2260fc"
            }
          ]
        },
        {
          "id": "9ca54aa6-31ce-41c3-a06c-57ed0d5265ce",
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
              "id": "01a4a2ee-a40d-4a52-ae88-663001e66a19"
            }
          ]
        },
        {
          "id": "e0d505a1-13e9-4704-be4c-80b81e070d19",
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
              "id": "d16d71f4-0a6e-49f1-9c40-7e9ceec1f454"
            }
          ]
        },
        {
          "id": "216de1d9-e680-464d-af4a-32dee9d2c012",
          "name": "hide-a-stream-item",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/activity_stream/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Hide a stream item."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e636a95a-393f-48ca-b7c4-6f2093d58ef5"
            }
          ]
        }
      ]
    }
  ]
}
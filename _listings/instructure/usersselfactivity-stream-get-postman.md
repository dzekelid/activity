{
  "info": {
    "name": "Instructure Canvas Users API List the activity stream",
    "_postman_id": "0d37bfcb-f151-4389-9c5e-a0a9db49864f",
    "description": "List the activity stream.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "d16b48de-0376-4996-b584-aa496c5e8564",
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
              "id": "7b120f02-1d8b-45c9-99ca-e7134652bffb"
            }
          ]
        },
        {
          "id": "de84a2b5-bff8-4eae-93a4-537dff19c0f6",
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
              "id": "e8013f18-3335-43e7-8fec-9c4f738bac7b"
            }
          ]
        },
        {
          "id": "71d437b9-4a89-4344-8065-9cb78576e237",
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
              "id": "05e89a8b-5012-40b8-80ba-1bdf4fced739"
            }
          ]
        }
      ]
    }
  ]
}
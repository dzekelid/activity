{
  "info": {
    "name": "Instructure Canvas Users API Hide all stream items",
    "_postman_id": "2296c9a1-6247-4d0b-bc22-316d6408ecd7",
    "description": "Hide all stream items.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "bb063c99-09a2-4aa0-ab75-d9dfce238c63",
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
              "id": "a1a529fb-0572-4fad-b5b0-853eb8f0c5e2"
            }
          ]
        },
        {
          "id": "e33c1ba6-196a-410d-8978-35e754232f9c",
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
              "id": "83843c6a-e1d8-4ced-8fa9-3c6272bca9a9"
            }
          ]
        }
      ]
    }
  ]
}
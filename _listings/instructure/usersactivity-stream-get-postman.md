{
  "info": {
    "name": "Instructure Canvas Users API List the activity stream",
    "_postman_id": "899cb640-9108-4bb2-bdb5-8597f45db687",
    "description": "List the activity stream.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "82885616-a0b3-442b-9e3b-278cbd87d4cb",
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
              "id": "38db9aab-e0bb-4949-ab0a-b3a6407ebf05"
            }
          ]
        }
      ]
    }
  ]
}
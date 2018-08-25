{
  "info": {
    "name": "Google Plus Get Activities",
    "_postman_id": "dd503e80-22ed-47c3-86e0-a2182ca2fb6e",
    "description": "Search public activities.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "552ac8e0-e131-409a-b6df-393b3117d2a7",
          "name": "plus.activities.search",
          "request": {
            "url": "http://example.com/api/activities?language=%7B%7D&maxResults=%7B%7D&orderBy=%7B%7D&pageToken=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search public activities."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6422be6-352a-4c71-9598-63af4e1240d9"
            }
          ]
        }
      ]
    }
  ]
}
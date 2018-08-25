{
  "info": {
    "name": "Data.gov API Get Activity",
    "_postman_id": "8ce794da-a6bb-43ca-9bd5-2fc96d0c0ef0",
    "description": "Fetch site activity, optionally filterd by user of org",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "29a625d4-2988-424b-8c6b-002365f04784",
          "name": "getActivity",
          "request": {
            "url": "http://catalog.data.gov/api/3/activity?organization=%7B%7D&page=%7B%7D&page_size=%7B%7D&user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch site activity, optionally filterd by user of org"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "956952fe-6aa2-4465-a724-c4464d65141b"
            }
          ]
        }
      ]
    }
  ]
}
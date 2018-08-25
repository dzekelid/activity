{
  "info": {
    "name": "Flickr Activity User Comments",
    "_postman_id": "e44b2806-3e4a-4f23-9745-67ee7763b618",
    "description": "Returns a list of recent activity on photos commented on by the calling user. Do not poll this method more than once an hour.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "911d01ff-cf43-453f-b3f2-5abc0ab3a9c0",
          "name": "getRestMethodFlickr.activity.usercomments",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.activity.userComments?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of recent activity on photos commented on by the calling user. Do not poll this method more than once an hour."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "610d8751-9606-4733-b9c4-1df1741396b3"
            }
          ]
        }
      ]
    }
  ]
}
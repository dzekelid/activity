{
  "info": {
    "name": "Flickr Activity User Photos",
    "_postman_id": "3e140639-9c5e-4b59-b5e3-97a528539119",
    "description": "Returns a list of recent activity on photos commented on by the calling user. Do not poll this method more than once an hour.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "bd434f28-eaea-444d-b24e-d3cb1467076c",
          "name": "getRestMethodFlickr.activity.userphotos",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.activity.userPhotos?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&timeframe=%7B%7D",
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
              "id": "c9004f8b-e635-46c6-9362-393ebd84db81"
            }
          ]
        }
      ]
    }
  ]
}
{
  "info": {
    "name": "SendGrid Get Access Settings Activity",
    "_postman_id": "6f2ccacf-c6fd-4902-b128-3550518f1c26",
    "description": "**This endpoint allows you to retrieve a list of all of the IP addresses that recently attempted to access your account either through the User Interface or the API.**\n\nIP Access Management allows you to control which IP addresses can be used to access your account, either through the User Interface or the API. There is no limit to the number of IP addresses that you can add to your whitelist. It is possible to remove your own IP address from the whitelist, thus preventing yourself from accessing your account.\n\nFor more information, please see our [User Guide](http://sendgrid.com/docs/User_Guide/Settings/ip_access_management.html).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "email",
      "item": [
        {
          "id": "a04c1c47-5727-409b-81da-157d095af87e",
          "name": "access_settings.activity.get",
          "request": {
            "url": "http://api.sendgrid.com/v3/access_settings/activity?limit=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**This endpoint allows you to retrieve a list of all of the IP addresses that recently attempted to access your account either through the User Interface or the API"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57b3b068-56c5-4856-8c31-68c19cc7c076"
            }
          ]
        }
      ]
    }
  ]
}
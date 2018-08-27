{
  "info": {
    "name": "AWS Step Functions API Delete Activity",
    "_postman_id": "f6e899f6-b114-442f-9d96-cda11f88fbc2",
    "description": "Deletes an activity.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "e67c21a5-a45e-48eb-900d-ec12c7259543",
          "name": "createActivity",
          "request": {
            "url": "http://example.com/api/?Action=CreateActivity?name=name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an activity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60b00fce-0a28-4c1e-af99-cf167950c1c4"
            }
          ]
        },
        {
          "id": "f6559974-562f-4583-9d98-9210de7ea809",
          "name": "deleteActivity",
          "request": {
            "url": "http://example.com/api/?Action=DeleteActivity?activityArn=activityArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an activity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ab289b7-cb42-46fe-9203-99e495ffec44"
            }
          ]
        }
      ]
    },
    {
      "name": "State Machine",
      "item": [
        {
          "id": "028ed70b-928c-47d0-a376-6d49aa1530f2",
          "name": "createStateMachine",
          "request": {
            "url": "http://example.com/api/?Action=CreateStateMachine?definition=definition&name=name&roleArn=roleArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a state machine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90e3472a-1bfd-4376-acd2-479ac79d3586"
            }
          ]
        }
      ]
    }
  ]
}
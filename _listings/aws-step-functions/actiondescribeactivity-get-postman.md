{
  "info": {
    "name": "AWS Step Functions API Describe Activity",
    "_postman_id": "1d3d2e88-eced-4f4b-9e5e-c0629d802733",
    "description": "Describes an activity.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "4b245d5e-feaa-4827-ae99-61bad91c479b",
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
              "id": "3f223835-ee06-42ae-9b2f-518a417488a8"
            }
          ]
        },
        {
          "id": "a9b078b2-83d9-4cfe-8c3e-a15957edfd71",
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
              "id": "39148dba-5bfc-4002-8175-f5c19c2e50d3"
            }
          ]
        },
        {
          "id": "89fb9770-20f7-425e-8bf6-0ec49e0454a5",
          "name": "describeActivity",
          "request": {
            "url": "http://example.com/api/?Action=DescribeActivity?activityArn=activityArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes an activity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b55974d3-88f1-4be9-bb76-d763353b5fb5"
            }
          ]
        }
      ]
    },
    {
      "name": "State Machine",
      "item": [
        {
          "id": "32153b1a-d85c-4e24-8595-9808a59cfee4",
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
              "id": "3393a8a1-c792-45ae-9be2-170f9126559a"
            }
          ]
        },
        {
          "id": "798cc874-4ae7-41a1-9a7b-ef908a2b2fa8",
          "name": "deleteStateMachine",
          "request": {
            "url": "http://example.com/api/?Action=DeleteStateMachine?stateMachineArn=stateMachineArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a state machine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12c696c7-58ff-4492-b151-34566127a7ea"
            }
          ]
        }
      ]
    }
  ]
}
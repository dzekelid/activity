{
  "info": {
    "name": "AWS Step Functions API List Activities",
    "_postman_id": "497a9186-66a8-4c7c-b8af-332b63324486",
    "description": "Lists the existing activities.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "f9e8e00c-7480-4ab8-909a-2d2877b09125",
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
              "id": "31c99106-ce7a-4458-9c97-8ce7fc370fef"
            }
          ]
        },
        {
          "id": "c1e5bde3-de01-40e6-b924-c50c417e9cbc",
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
              "id": "25751618-3275-4383-80c1-5c0a7f9888e7"
            }
          ]
        },
        {
          "id": "a6596fc6-36e7-493d-b64e-5131678ca13b",
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
              "id": "ec26446f-e8cf-4e43-8350-93db283cda43"
            }
          ]
        },
        {
          "id": "7cadc1e8-74fb-4ec2-b376-f6dfe2dd3c76",
          "name": "listActivities",
          "request": {
            "url": "http://example.com/api/?Action=ListActivities?maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the existing activities."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b8ab621-03d2-491e-85f5-5759d7b32c5c"
            }
          ]
        }
      ]
    },
    {
      "name": "State Machine",
      "item": [
        {
          "id": "b0b4919e-825f-49da-88e5-8acab16a540c",
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
              "id": "553816bf-d110-464a-a287-8861eec5ce37"
            }
          ]
        },
        {
          "id": "77829e81-427f-4eb3-b428-0cb1ecc3ca18",
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
              "id": "283625ea-1d9a-4b72-a277-93588e9c879a"
            }
          ]
        },
        {
          "id": "3d2e0746-1e6b-4989-9e23-0ac34561879f",
          "name": "describeStateMachine",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStateMachine?stateMachineArn=stateMachineArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes a state machine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbe4bc54-a2d3-4626-ae9c-dd9778d94129"
            }
          ]
        }
      ]
    },
    {
      "name": "Execution",
      "item": [
        {
          "id": "0d52bbdf-16b7-47d0-b900-0f8308c23194",
          "name": "describeExecution",
          "request": {
            "url": "http://example.com/api/?Action=DescribeExecution?executionArn=executionArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes an execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb2e9abf-a6fc-47c7-878c-d33177a6b054"
            }
          ]
        },
        {
          "id": "4c2e2b3c-bbbc-433e-b1bd-a5b8ab717c54",
          "name": "getExecutionHistory",
          "request": {
            "url": "http://example.com/api/?Action=GetExecutionHistory?executionArn=executionArn&maxResults=maxResults&nextToken=nextToken&reverseOrder=reverseOrder",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the history of the specified execution as a list of events."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebf0ba54-87fa-4a71-87dc-ea1d72b94dd3"
            }
          ]
        }
      ]
    },
    {
      "name": "Activity Task",
      "item": [
        {
          "id": "d7255e7b-bdcb-4541-b45d-6fcb6b832c1e",
          "name": "getActivityTask",
          "request": {
            "url": "http://example.com/api/?Action=GetActivityTask?activityArn=activityArn&workerName=workerName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Used by workers to retrieve a task (with the specified activity ARN) which has been scheduled \n    for execution by a running state machine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1238b51d-da75-4af8-bf4a-c6bf0e4808ac"
            }
          ]
        }
      ]
    }
  ]
}
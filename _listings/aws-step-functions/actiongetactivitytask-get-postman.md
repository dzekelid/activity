{
  "info": {
    "name": "AWS Step Functions API Get Activity Task",
    "_postman_id": "fa0c1825-660f-43db-af54-82d32e2a0175",
    "description": "Used by workers to retrieve a task (with the specified activity ARN) which has been scheduled \n    for execution by a running state machine.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity Task",
      "item": [
        {
          "id": "855d69bf-80a8-47f2-b215-34adb62ba6af",
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
              "id": "a582e6a0-6de3-40d1-82b9-0f65a7054fed"
            }
          ]
        }
      ]
    }
  ]
}
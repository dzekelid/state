{
  "info": {
    "name": "AWS Step Functions API Delete State Machine",
    "_postman_id": "ffe86154-daa0-4083-abb9-c2c10ce79270",
    "description": "Deletes a state machine.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "State Machine",
      "item": [
        {
          "id": "26e94eb9-e94f-4fc9-8877-42b8ffc0b9d7",
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
              "id": "ce1d378c-3eda-4735-83e1-ae08b66916ec"
            }
          ]
        },
        {
          "id": "5cd2a0d2-492a-4ba8-b485-40eac5aab77a",
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
              "id": "8ed34f10-f9eb-46b0-bd31-cc250a15ba60"
            }
          ]
        }
      ]
    }
  ]
}
{
  "info": {
    "name": "AWS Step Functions API Describe State Machine",
    "_postman_id": "91e9603a-4a22-4a98-909d-fc0dc0729bd8",
    "description": "Describes a state machine.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "State Machine",
      "item": [
        {
          "id": "4ae060d7-4a08-4fe1-95da-3430318d6acd",
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
              "id": "636536e9-6e6f-4033-a443-bf26f6a56429"
            }
          ]
        },
        {
          "id": "1e502d57-2007-47c4-a503-51a300a3ec18",
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
              "id": "a4682622-062e-4abb-bc5b-2a93624f2c43"
            }
          ]
        },
        {
          "id": "dd771c06-9103-46b9-ac7b-0bea32cc8ada",
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
              "id": "2ea99ca5-69ba-4380-80e2-44c87f75abbe"
            }
          ]
        }
      ]
    }
  ]
}
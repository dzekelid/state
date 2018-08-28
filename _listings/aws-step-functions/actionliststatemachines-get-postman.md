{
  "info": {
    "name": "AWS Step Functions API List State Machines",
    "_postman_id": "1f074860-fc2c-41c1-b9a9-4f6b728ee27e",
    "description": "Lists the existing state machines.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "State Machine",
      "item": [
        {
          "id": "30428337-5f3c-4ece-a96e-1771eff2ea66",
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
              "id": "9b78ba0b-93e1-496f-a6fd-fa4ec781ce3a"
            }
          ]
        },
        {
          "id": "809316ca-f0da-4a62-84af-374031390343",
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
              "id": "051699b2-7488-4f64-9a0c-2fda40f8f461"
            }
          ]
        },
        {
          "id": "0b56a284-76b9-45fc-9d64-6ae4823613d9",
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
              "id": "e8dd1520-6bb2-48d4-bcff-56f01dff5886"
            }
          ]
        },
        {
          "id": "cf04eec0-1782-4ae3-905c-e22a8aff1e7b",
          "name": "listExecutions",
          "request": {
            "url": "http://example.com/api/?Action=ListExecutions?maxResults=maxResults&nextToken=nextToken&stateMachineArn=stateMachineArn&statusFilter=statusFilter",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the executions of a state machine that meet the filtering criteria."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff496a2e-cf76-4dee-a871-c0a9a8a90095"
            }
          ]
        },
        {
          "id": "dce645bc-2aea-4f02-b2db-ad3171a47d19",
          "name": "listStateMachines",
          "request": {
            "url": "http://example.com/api/?Action=ListStateMachines?maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the existing state machines."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "020eb1be-374b-4040-b0dc-addffa684cab"
            }
          ]
        }
      ]
    }
  ]
}
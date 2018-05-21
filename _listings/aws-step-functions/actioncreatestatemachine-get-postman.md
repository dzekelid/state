{
  "info": {
    "name": "AWS Step Functions API Create State Machine",
    "_postman_id": "9d6bc11f-71ea-4408-8bdc-f530c392309b",
    "description": "Creates a state machine.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "State Machine",
      "item": [
        {
          "id": "2eccd81e-835a-491d-a45d-acbb45e36c9f",
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
              "id": "e72f8df5-d1e1-4a9e-a1dd-c721ceb03132"
            }
          ]
        }
      ]
    }
  ]
}
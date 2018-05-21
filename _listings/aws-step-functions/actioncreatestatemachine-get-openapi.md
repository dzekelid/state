---
swagger: "2.0"
x-collection-name: AWS Step Functions
x-complete: 0
info:
  title: AWS Step Functions API Create State Machine
  version: 1.0.0
  description: Creates a state machine.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateStateMachine:
    get:
      summary: Create State Machine
      description: Creates a state machine.
      operationId: createStateMachine
      x-api-path-slug: actioncreatestatemachine-get
      parameters:
      - in: query
        name: definition
        description: The Amazon States Language definition of the state machine
        type: string
      - in: query
        name: name
        description: The name of the state machine
        type: string
      - in: query
        name: roleArn
        description: The Amazon Resource Name (ARN) of the IAM role to use for this
          state machine
        type: string
      responses:
        200:
          description: OK
      tags:
      - State Machine
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---
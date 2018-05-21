---
swagger: "2.0"
x-collection-name: AWS CloudWatch
x-complete: 1
info:
  title: AWS CloudWatch API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SetAlarmState:
    "":
      summary: Set Alarm State
      description: Temporarily sets the state of an alarm for testing purposes.
      operationId: setalarmstate
      x-api-path-slug: actionsetalarmstate-
      parameters:
      - in: query
        name: AlarmName
        description: The name for the alarm
        type: string
      - in: query
        name: StateReason
        description: The reason that this alarm is set to this specific state, in
          text format
        type: string
      - in: query
        name: StateReasonData
        description: The reason that this alarm is set to this specific state, in
          JSON format
        type: string
      - in: query
        name: StateValue
        description: The value of the state
        type: string
      responses:
        200:
          description: OK
      tags:
      - Aler State
---
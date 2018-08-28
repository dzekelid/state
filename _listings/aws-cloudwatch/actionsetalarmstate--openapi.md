---
swagger: "2.0"
x-collection-name: AWS CloudWatch
x-complete: 0
info:
  title: Amazon CloudWatch API Set Alarm State
  version: 1.0.0
  description: Temporarily sets the state of an alarm for testing purposes.
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
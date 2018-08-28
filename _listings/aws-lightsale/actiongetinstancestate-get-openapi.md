---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 0
info:
  title: Amazon Lightsale API Get Instance State
  version: 1.0.0
  description: Returns the state of a specific instance.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetInstancePortStates:
    get:
      summary: Get Instance Port States
      description: |-
        Returns the port states for a specific virtual private server, or
                instance.
      operationId: getInstancePortStates
      x-api-path-slug: actiongetinstanceportstates-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstanceState:
    get:
      summary: Get Instance State
      description: Returns the state of a specific instance.
      operationId: getInstanceState
      x-api-path-slug: actiongetinstancestate-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance to get state information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
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
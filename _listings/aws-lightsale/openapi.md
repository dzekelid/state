swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 1
info:
  title: AWS Lightsale API
  version: 1.0.0
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
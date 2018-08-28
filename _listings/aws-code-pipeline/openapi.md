swagger: "2.0"
x-collection-name: AWS Code Pipeline
x-complete: 1
info:
  title: AWS Code Pipeline API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetPipelineState:
    get:
      summary: Get Pipeline State
      description: |-
        Returns information about the state of a pipeline, including the stages and
                    actions.
      operationId: getPipelineState
      x-api-path-slug: actiongetpipelinestate-get
      parameters:
      - in: query
        name: Attribute
        description: The attribute to reset
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: name
        description: The name of the pipeline about which you want to get information
        type: string
      - in: query
        name: SnapshotId
        description: The ID of the snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
      - State
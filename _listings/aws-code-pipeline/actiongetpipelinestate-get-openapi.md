---
swagger: "2.0"
x-collection-name: AWS Code Pipeline
x-complete: 0
info:
  title: AWS Code Pipeline API Get Pipeline State
  version: 1.0.0
  description: |-
    Returns information about the state of a pipeline, including the stages and
                actions.
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
---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Clears a state item.
  version: 1.0.0
  description: Clears a state item..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/coreplatformstate/{stateItemReference}:
    delete:
      summary: Clears a state item.
      description: Clears a state item..
      operationId: CorePlatformState_ClearStateItemBystateItemReference
      x-api-path-slug: apicoreplatformstatestateitemreference-delete
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: stateItemReference
        description: The state item reference
      responses:
        200:
          description: OK
      tags:
      - Clears
      - State
      - Item
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
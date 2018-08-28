---
swagger: "2.0"
x-collection-name: Google App Engine
x-complete: 0
info:
  title: Google App Engine Admin API Get State
  description: Gets the latest state of a long-running operation. Clients can use
    this method to poll the operation result at intervals as recommended by the API
    service.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: appengine.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/apps/{appsId}/operations/{operationsId}:
    get:
      summary: Get State
      description: Gets the latest state of a long-running operation. Clients can
        use this method to poll the operation result at intervals as recommended by
        the API service.
      operationId: appengine.apps.operations.get
      x-api-path-slug: v1appsappsidoperationsoperationsid-get
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: path
        name: operationsId
        description: Part of `name`
      responses:
        200:
          description: OK
      tags:
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
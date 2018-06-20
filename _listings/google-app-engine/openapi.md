---
swagger: "2.0"
x-collection-name: Google App Engine
x-complete: 1
info:
  title: Google App Engine Admin
  description: provisions-and-manages-app-engine-applications-
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
---
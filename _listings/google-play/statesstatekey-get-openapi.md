---
swagger: "2.0"
x-collection-name: Google Play
x-complete: 0
info:
  title: Google Play Get State Key
  version: 1.0.0
  description: Retrieves the data corresponding to the passed key. If the key does
    not exist on the server, an HTTP 404 will be returned.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /states:
    get:
      summary: Get State Keys
      description: Lists all the states keys, and optionally the state data.
      operationId: appstate.states.list
      x-api-path-slug: states-get
      parameters:
      - in: query
        name: includeData
        description: Whether to include the full data in addition to the version number
      responses:
        200:
          description: OK
      tags:
      - Application State
  /states/{stateKey}:
    delete:
      summary: Delete State Key
      description: Deletes a key and the data associated with it. The key is removed
        and no longer counts against the key quota. Note that since this method is
        not safe in the face of concurrent modifications, it should only be used for
        development and testing purposes. Invoking this method in shipping code can
        result in data loss and data corruption.
      operationId: appstate.states.delete
      x-api-path-slug: statesstatekey-delete
      parameters:
      - in: path
        name: stateKey
        description: The key for the data to be retrieved
      responses:
        200:
          description: OK
      tags:
      - Application State
    get:
      summary: Get State Key
      description: Retrieves the data corresponding to the passed key. If the key
        does not exist on the server, an HTTP 404 will be returned.
      operationId: appstate.states.get
      x-api-path-slug: statesstatekey-get
      parameters:
      - in: path
        name: stateKey
        description: The key for the data to be retrieved
      responses:
        200:
          description: OK
      tags:
      - Application State
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
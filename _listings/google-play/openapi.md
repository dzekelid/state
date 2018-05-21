---
swagger: "2.0"
x-collection-name: Google Play
x-complete: 1
info:
  title: Google Play
  version: 1.0.0
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
    put:
      summary: Update State Key
      description: Update the data associated with the input key if and only if the
        passed version matches the currently stored version. This method is safe in
        the face of concurrent writes. Maximum per-key size is 128KB.
      operationId: appstate.states.update
      x-api-path-slug: statesstatekey-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: currentStateVersion
        description: The version of the app state your application is attempting to
          update
      - in: path
        name: stateKey
        description: The key for the data to be retrieved
      responses:
        200:
          description: OK
      tags:
      - Application State
  /states/{stateKey}/clear:
    post:
      summary: Clear State Key
      description: Clears (sets to empty) the data for the passed key if and only
        if the passed version matches the currently stored version. This method results
        in a conflict error on version mismatch.
      operationId: appstate.states.clear
      x-api-path-slug: statesstatekeyclear-post
      parameters:
      - in: query
        name: currentDataVersion
        description: The version of the data to be cleared
      - in: path
        name: stateKey
        description: The key for the data to be retrieved
      responses:
        200:
          description: OK
      tags:
      - Application State
---
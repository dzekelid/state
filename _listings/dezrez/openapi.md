swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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
  /api/coreplatformstate/platformissue:
    post:
      summary: Allows business workflows to post system issues to the platform state
        service.
      description: Allows business workflows to post system issues to the platform
        state service..
      operationId: CorePlatformState_PostPlatformIssueByalertDataContract
      x-api-path-slug: apicoreplatformstateplatformissue-post
      parameters:
      - in: body
        name: alertDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - Business
      - Workflows
      - To
      - Post
      - System
      - Issues
      - To
      - Platform
      - State
      - Service
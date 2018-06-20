---
swagger: "2.0"
x-collection-name: Healthcare.gov
x-complete: 1
info:
  title: Healthcare
  version: 1.0.0
host: www.healthcare.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/states{mediaTypeExtension}:
    get:
      summary: Get States
      description: Returns pages content.
      operationId: getApiStatesMediatypeextension
      x-api-path-slug: apistatesmediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      responses:
        200:
          description: OK
      tags:
      - States
  /es/{stateName}{mediaTypeExtension}:
    get:
      summary: Get Es Statename
      description: Returns pages content.
      operationId: getEsStatenameMediatypeextension
      x-api-path-slug: esstatenamemediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      - in: path
        name: stateName
      responses:
        200:
          description: OK
      tags:
      - Es
      - Statename
  /{stateName}{mediaTypeExtension}:
    get:
      summary: Get Statename
      description: Returns pages content.
      operationId: getStatenameMediatypeextension
      x-api-path-slug: statenamemediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      - in: path
        name: stateName
      responses:
        200:
          description: OK
      tags:
      - Statename
---
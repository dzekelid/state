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
      summary: Get API States Media Type Extension
      description: Returns pages content.
      operationId: returns-pages-content
      x-api-path-slug: apistatesmediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - States
      - Media
      - Type
      - Extension
  /es/{stateName}{mediaTypeExtension}/:
    get:
      summary: Get State Name Media Type Extension
      description: Returns pages content.
      operationId: returns-pages-content
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
      - Insurance
      - State
      - Name
      - Media
      - Type
      - Extension
  /{stateName}{mediaTypeExtension}/:
    get:
      summary: Get State Name Media Type Extension
      description: Returns pages content.
      operationId: returns-pages-content
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
      - Insurance
      - State
      - Name
      - Media
      - Type
      - Extension
---
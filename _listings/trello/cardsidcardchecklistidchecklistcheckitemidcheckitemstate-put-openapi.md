---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Put Cards Checklist Checkitem Checkitem State
  description: Put cards checklist checkitem checkitem state.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cards/{idCard}/checklist/{idChecklist}/checkItem/{idCheckItem}/state:
    put:
      summary: Put Cards Checklist Checkitem Checkitem State
      description: Put cards checklist checkitem checkitem state.
      operationId: updateCardsChecklistCheckItemStateByIdCardByIdChecklistByIdCheckItem
      x-api-path-slug: cardsidcardchecklistidchecklistcheckitemidcheckitemstate-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Checklist Check Item State to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idCheckItem
        description: idCheckItem
      - in: path
        name: idChecklist
        description: idChecklist
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Checklist
      - Checkitem
      - Checkitem
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
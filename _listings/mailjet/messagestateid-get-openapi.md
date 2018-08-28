---
swagger: "2.0"
x-collection-name: Mailjet
x-complete: 0
info:
  title: Mailjet Messages API Message State
  description: Returns message state.
  version: v3
host: api.mailjet.com
basePath: v3/REST/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  messagestate/{id}:
    get:
      summary: Message State
      description: Returns message state.
      operationId: getMessagestate
      x-api-path-slug: messagestateid-get
      parameters:
      - in: query
        name: id
        description: Id of the message
      responses:
        200:
          description: OK
      tags:
      - Message
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
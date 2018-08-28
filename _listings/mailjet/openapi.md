swagger: "2.0"
x-collection-name: Mailjet
x-complete: 1
info:
  title: Mailjet Messages API
  description: allows-you-to-list-and-view-the-details-of-a-message-an-email-processed-by-mailjet
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
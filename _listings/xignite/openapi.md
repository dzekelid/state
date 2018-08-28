swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetStateRate:
    get:
      summary: Get State Rate
      description: Returns a state rate
      operationId: postGetstaterate
      x-api-path-slug: getstaterate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - State
      - Rate
  /GetStateRates:
    get:
      summary: Get State Rates
      description: Returns state rates for a date range.
      operationId: postGetstaterates
      x-api-path-slug: getstaterates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - State
      - Rates
---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Get State List
  description: "Returns all the states of a certain country\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [perPage] value is invalid\n\n\n404\nCMN-102\nResource for parameter [stateId]
    is not found"
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/dictionary/state:
    get:
      summary: Get State List
      description: "Returns all the states of a certain country\nUsage Plan Group\nLight\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [perPage] value is invalid\n\n\n404\nCMN-102\nResource for parameter [stateId]
        is not found"
      operationId: listStates
      x-api-path-slug: restapiv1-0dictionarystate-get
      parameters:
      - in: query
        name: countryId
        description: Internal identifier of a country
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      - in: query
        name: withPhoneNumbers
        description: If True, the list of states with phone numbers available for
          buying is returned
      responses:
        200:
          description: OK
      tags:
      - State
      - List
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
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 1
info:
  title: RingCentral Connect Platform API Explorer
  description: this-is-an-interactive-api-explorer-for-the-ringcentral-connect-platform--to-use-this-service-you-will-need-to-have-a-developer-account---links--a-hrefhttpsnetstorage-ringcentral-comdpwapiexplorerrcplatform-basic-ymlv20180514092722-target-blankringcentral-api-specaspannbspnbspopenapi-fka-swagger-formatnbspnbspnbspnbspspana-hrefhttpsgithub-comoaiopenapispecification-target-blanklearn-more-about-openapia
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
  /restapi/v1.0/dictionary/state/{stateId}:
    get:
      summary: Get State
      description: "Returns the information on a specific state.\nUsage Plan Group\nLight\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource
        for parameter [stateId] is not found"
      operationId: loadState
      x-api-path-slug: restapiv1-0dictionarystatestateid-get
      parameters:
      - in: path
        name: stateId
        description: Internal identifier of a state
      responses:
        200:
          description: OK
      tags:
      - State
---
swagger: "2.0"
x-collection-name: Paylocity
x-complete: 0
info:
  title: Paylocity Add/update primary state tax
  description: Sends new or updated employee primary state tax information directly
    to Web Pay.
  termsOfService: WebLink.OpenApiDoc.TermsOfService
  version: "2"
host: api.paylocity.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/companies/{companyId}/employees/{employeeId}/nonprimaryStateTax:
    put:
      summary: Add/update non-primary state tax
      description: Sends new or updated employee non-primary state tax information
        directly to Web Pay.
      operationId: v2.companies.companyId.employees.employeeId.nonprimaryStateTax.put
      x-api-path-slug: v2companiescompanyidemployeesemployeeidnonprimarystatetax-put
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: employeeId
        description: Employee Id
      - in: body
        name: json
        description: Non-Primary State Tax Model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - NonprimaryStateTax
  /v2/companies/{companyId}/employees/{employeeId}/primaryStateTax:
    put:
      summary: Add/update primary state tax
      description: Sends new or updated employee primary state tax information directly
        to Web Pay.
      operationId: v2.companies.companyId.employees.employeeId.primaryStateTax.put
      x-api-path-slug: v2companiescompanyidemployeesemployeeidprimarystatetax-put
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: employeeId
        description: Employee Id
      - in: body
        name: json
        description: Primary State Tax Model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - PrimaryStateTax
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
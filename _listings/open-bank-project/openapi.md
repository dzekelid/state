swagger: "2.0"
x-collection-name: Open Bank Project
x-complete: 1
info:
  title: Account and Transaction API Specification
  description: swagger-for-account-and-transaction-api-specification
  termsOfService: https://www.openbanking.org.uk/terms
  contact:
    name: Service Desk
    email: ServiceDesk@openbanking.org.uk
  version: 1.0.0
basePath: /open-banking/v2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{AccountId}/statements:
    get:
      summary: Get Account Statements
      description: Get Statements related to an account
      operationId: GetAccountStatements
      x-api-path-slug: accountsaccountidstatements-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Account
      - Statements
  /accounts/{AccountId}/statements/{StatementId}:
    get:
      summary: Get Statement
      description: Get Statement related to an account
      operationId: GetAccountStatement
      x-api-path-slug: accountsaccountidstatementsstatementid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Statement
  /accounts/{AccountId}/statements/{StatementId}/file:
    get:
      summary: Get Statement File
      description: Get Statement File related to an account
      operationId: GetAccountStatementFile
      x-api-path-slug: accountsaccountidstatementsstatementidfile-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Statement
      - File
  /accounts/{AccountId}/statements/{StatementId}/transactions:
    get:
      summary: Get Statement Transactions
      description: Get Statement Transactions related to an account
      operationId: GetAccountStatementTransactions
      x-api-path-slug: accountsaccountidstatementsstatementidtransactions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Statement
      - Transactions
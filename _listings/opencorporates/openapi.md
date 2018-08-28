---
swagger: "2.0"
x-collection-name: OpenCorporates
x-complete: 1
info:
  title: OpenCorporates
  description: the-api-for-managing-opencorporates-data-
  termsOfService: https://opencorporates.com/info/licence
  version: v.04
host: api.opencorporates.com
basePath: v0.4/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /placeholders/:id/statements:
    get:
      summary: Placeholders  ID Statements
      description: nThis returns the statements associated with a given placeholder
      operationId: placeholders--id-statements
      x-api-path-slug: placeholdersidstatements-get
      responses:
        200:
          description: OK
      tags:
      - Businesses
      - Placeholders
      - Statements
---
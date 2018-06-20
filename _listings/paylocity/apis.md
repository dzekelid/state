---
name: Paylocity
x-slug: paylocity
description: ""
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: State
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/paylocity/apis.md
specificationVersion: "0.14"
apis:
- name: Paylocity Add/update non-primary state tax
  x-api-slug: paylocity
  description: Sends new or updated employee non-primary state tax information directly
    to Web Pay.
  image: ""
  humanURL: http://paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/employees/{employeeId}/nonprimaryStateTax
  tags: V2,Companies,CompanyId,Employees,EmployeeId,NonprimaryStateTax
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidnonprimarystatetax-put-openapi.md
- name: Paylocity Add/update primary state tax
  x-api-slug: paylocity
  description: Sends new or updated employee primary state tax information directly
    to Web Pay.
  image: ""
  humanURL: http://paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/employees/{employeeId}/primaryStateTax
  tags: V2,Companies,CompanyId,Employees,EmployeeId,PrimaryStateTax
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidprimarystatetax-put-openapi.md
- name: Paylocity
  x-api-slug: paylocity
  description: ""
  image: ""
  humanURL: http://paylocity.com
  baseURL: https://api.paylocity.com//api
  tags: State
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/paylocity/openapi.md
x-common:
- type: x-blog
  url: https://www.paylocity.com/resources/blog/
- type: x-github
  url: https://github.com/Paylocity
- type: x-integrations
  url: https://www.paylocity.com/partnerships/integrations/
- type: x-twitter
  url: https://twitter.com/Paylocity
- type: x-website
  url: http://paylocity.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---
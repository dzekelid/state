---
name: OpenCorporates
x-slug: opencorporates
description: OpenCorporates is a website which shares data on corporate entities as
  open data under the share-alike attribution Open Database License. It was created
  by Chris Taggart and Rob McKinnon, under the auspices of their company, Chrinon
  Ltd, and launched on 20 December 2010. It has the aims of creating a URL with such
  data for every corporate entity in the world, importing government data relating
  to companies and matching it to specific companies. The site also shows groups of
  companies which are legally part of the same conglomerate. Basic company information
  is available as open data in XML or JSON format.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/OpenCorporates.jpg
x-kinRank: "9"
x-alexaRank: ""
tags: State
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/opencorporates/apis.md
specificationVersion: "0.14"
apis:
- name: OpenCorporates Placeholders  ID Statements
  x-api-slug: opencorporates
  description: nThis returns the statements associated with a given placeholder
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/OpenCorporates.jpg
  humanURL: https://opencorporates.com/
  baseURL: ://api.opencorporates.com/v0.4///placeholders/:id/statements
  tags: Businesses,Placeholders,Statements
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/opencorporates/placeholdersidstatements-get-openapi.md
- name: OpenCorporates
  x-api-slug: opencorporates
  description: OpenCorporates is a database of corporate data. OpenCorporates offers
    users the ability to search for information on 30 million corporations from around
    the world. Users can also search by type of corporation. The OpenCorporates API
    allows developers to access and integrate the data and functionality of OpenCorporates
    with other applications. Some example API methods include searching and retrieving
    information on corporation by type, jurisdiction, and company ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/OpenCorporates.jpg
  humanURL: https://opencorporates.com/
  baseURL: ://api.opencorporates.com/v0.4/
  tags: State
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/opencorporates/openapi.md
x-common:
- type: x-base
  url: https://api.opencorporates.com/
- type: x-blog
  url: http://blog.opencorporates.com/
- type: x-blog-rss
  url: http://blog.opencorporates.com/feed/
- type: x-developer
  url: http://api.opencorporates.com/
- type: x-github
  url: https://github.com/openc
- type: x-pricing
  url: https://opencorporates.com/info/pricing
- type: x-status
  url: http://status.opencorporates.com/
- type: x-terms-of-service
  url: https://opencorporates.com/info/licence
- type: x-twitter
  url: https://twitter.com/opencorporates
- type: x-website
  url: https://opencorporates.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---
---
name: Google App Engine
x-slug: google-app-engine
description: 'Build modern web and mobile applications on an open cloud platform:
  bring your own language runtimes, frameworks, and third party libraries. Google
  App Engine is a fully managed platform that completely abstracts away infrastructure
  so you focus only on code. Go from zero to planet-scale and see why some of today&rsquo;s
  most successful companies power their applications on App Engine.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-app-engine-icon.png
x-kinRank: "9"
x-alexaRank: ""
tags: State
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/google-app-engine/apis.md
specificationVersion: "0.14"
apis:
- name: Google App Engine Admin API Get State
  x-api-slug: google-app-engine-admin-api
  description: Gets the latest state of a long-running operation. Clients can use
    this method to poll the operation result at intervals as recommended by the API
    service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-app-engine-icon.png
  humanURL: https://cloud.google.com/appengine/
  baseURL: ://appengine.googleapis.com////v1/apps/{appsId}/operations/{operationsId}
  tags: State
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/google-app-engine/v1appsappsidoperationsoperationsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/google-app-engine/v1appsappsidoperationsoperationsid-get-openapi.md
- name: Google App Engine Admin API
  x-api-slug: google-app-engine-admin-api
  description: Use this RESTful API with any programming language to manage your App
    Engine applications.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-app-engine-icon.png
  humanURL: https://cloud.google.com/appengine/
  baseURL: ://appengine.googleapis.com//
  tags: State
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/google-app-engine/openapi.md
x-common:
- type: x-code-page
  url: https://cloud.google.com/appengine/docs/admin-api/client-libraries
- type: x-developer
  url: https://cloud.google.com/appengine/docs/admin-api/
- type: x-documentation
  url: https://cloud.google.com/appengine/docs/admin-api/apis
- type: x-getting-started
  url: https://cloud.google.com/appengine/docs/admin-api/getting-started/
- type: x-how-to-guides
  url: https://cloud.google.com/appengine/docs/admin-api/how-to
- type: x-launcher
  url: https://cloud.google.com/launcher/
- type: x-pricing
  url: https://cloud.google.com/pricing/
- type: x-sla
  url: https://cloud.google.com/appengine/sla
- type: x-website
  url: https://cloud.google.com/appengine/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---
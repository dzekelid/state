---
name: Google Play
x-slug: google-play
description: 'The Google Play Developer API allows you to perform a number of publishing
  and app-management tasks. It includes two components: The Subscriptions and In-App
  Purchases API lets you manage in-app purchases and subscriptions. The Publishing
  API lets you upload and publish apps, and perform other publishing-related tasks.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
x-kinRank: "9"
x-alexaRank: "0"
tags: State
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/google-play/apis.md
specificationVersion: "0.14"
apis:
- name: Google Play Get State Keys
  x-api-slug: google-play
  description: Lists all the states keys, and optionally the state data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https://///states
  tags: Application State
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/google-play/states-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/google-play/states-get-openapi.md
- name: Google Play Delete State Key
  x-api-slug: google-play
  description: Deletes a key and the data associated with it. The key is removed and
    no longer counts against the key quota. Note that since this method is not safe
    in the face of concurrent modifications, it should only be used for development
    and testing purposes. Invoking this method in shipping code can result in data
    loss and data corruption.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https://///states/{stateKey}
  tags: Application State
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/google-play/statesstatekey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/google-play/statesstatekey-delete-openapi.md
- name: Google Play Get State Key
  x-api-slug: google-play
  description: Retrieves the data corresponding to the passed key. If the key does
    not exist on the server, an HTTP 404 will be returned.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https://///states/{stateKey}
  tags: Application State
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/google-play/statesstatekey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/google-play/statesstatekey-get-openapi.md
- name: Google Play Update State Key
  x-api-slug: google-play
  description: Update the data associated with the input key if and only if the passed
    version matches the currently stored version. This method is safe in the face
    of concurrent writes. Maximum per-key size is 128KB.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https://///states/{stateKey}
  tags: Application State
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/google-play/statesstatekey-put-openapi.md
- name: Google Play Clear State Key
  x-api-slug: google-play
  description: Clears (sets to empty) the data for the passed key if and only if the
    passed version matches the currently stored version. This method results in a
    conflict error on version mismatch.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https://///states/{stateKey}/clear
  tags: Application State
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/google-play/statesstatekeyclear-post-openapi.md
- name: Google Play
  x-api-slug: google-play
  description: 'The Google Play Developer API allows you to perform a number of publishing
    and app-management tasks. It includes two components: The Subscriptions and In-App
    Purchases API lets you manage in-app purchases and subscriptions. The Publishing
    API lets you upload and publish apps, and perform other publishing-related tasks.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: State
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/state/master/_listings/google-play/openapi.md
x-common:
- type: x-blog
  url: https://blog.google/products/google-play/
- type: x-blog-rss
  url: https://blog.google/products/google-play/rss
- type: x-developer
  url: https://developers.google.com/android-publisher/
- type: x-facebook
  url: https://www.facebook.com/GooglePlay
- type: x-getting-started
  url: https://developers.google.com/android-publisher/getting_started
- type: x-twitter
  url: https://twitter.com/GooglePlay
- type: x-website
  url: https://play.google.com/store
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---